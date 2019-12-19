---
layout: post
title: Kafka - Monitoring
edited: true
---

# Problem cases

Under this sections are details about cases happened and their actions

## 1. INVALID_FETCH_SESSION_EPOCH in Client logs

### Scenario

Error response from Kafka client happens intermittently on no specific topic.

```
[pool-1-thread-1] 2019-12-18 09:45:19,994 FetchSessionHandler.java (line 383) [Consumer clientId=consumer-1, groupId=my.consumer_19_1576578898213] Node 4 was unable to process the fetch request with (sessionId=759283615, epoch=469203): INVALID_FETCH_SESSION_EPOCH.
```

### Status

- [ ]  Reproducable (?)

- [x]  Posible actions

- [ ]  Verify 

### Actions

- Possibly effected by Kafka's issue [KAFKA-8052](https://github.com/apache/kafka/pull/6582)
  
  - **Description**:
    
    `When fetch response is processed by the heartbeat thread, polling thread may send new fetch request with the same epoch as the previous fetch request if heartbeat thread hasn't yet updated the epoch. `
    
    `This results in INVALID_FETCH_SESSION_EPOCH error. Even though the request is retried without any disconnections, it will be good to avoid this error. The PR tracks status of previous request in the session handler and sends next fetch request only after the response from the previous request is processed.`
  
  - Related external reported cases
    
    - [https://issues.apache.org/jira/browse/KAFKA-8052](https://issues.apache.org/jira/browse/KAFKA-8052)
    
    - [https://stackoverflow.com/questions/54823733/kafka-invalid-fetch-session-epoch](https://stackoverflow.com/questions/54823733/kafka-invalid-fetch-session-epoch)
    
    - [https://discuss.elastic.co/t/kafka-invalid-fetch-session-epoch/187441/3](https://discuss.elastic.co/t/kafka-invalid-fetch-session-epoch/187441/3)
  
  - Related documentation
    
    - [https://cwiki.apache.org/confluence/display/KAFKA/KIP-227%3A+Introduce+Incremental+FetchRequests+to+Increase+Partition+Scalability](https://cwiki.apache.org/confluence/display/KAFKA/KIP-227%3A+Introduce+Incremental+FetchRequests+to+Increase+Partition+Scalability)


