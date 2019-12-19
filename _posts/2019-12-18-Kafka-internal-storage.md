---
layout: post
title: Kafka - Internal storage
edited: true
---
## Log storage

Kafka log directory structure:

```
parent
|-- my-topic-0
    |-- 00000000000000069679.index
    |-- 00000000000000069679.timeindex
    |-- 00000000000000069679.log
    |-- 00000000000000069679.snapshot
    |-- leader-epoch-checkpoint/
|-- my-topic-1
|-- my-topic-2
```

### Topic

- Topic is the logical grouping
- Each topic is assigned with at least 1 partition (in this case, `my-topic` has two partitions, hence `my-topic-0,1,2`)

### Partition

![](https://miro.medium.com/max/1296/1*9W02uviSfU_QSHjaNTnNXQ.png)

- *Partition* is a storage unit in Kafka
- **Partition** includes multiple segments (`xxxxx.log`) with corresponding index (`xxxxx.index`)

### Segment

- Partition is splitted into segments for faster retention operation (instead of operating delete on the whole partition, Kafka
could run on segments one-by-one leaving out the active one)
- Messages are stored in the `xxxxx.log` file

### How Kafka brokers store published messages



# References

- [Travis Jeffery - How Kafka’s Storage Internals Work](https://thehoard.blog/how-kafkas-storage-internals-work-3a29b02e026)

- [Durga Perla - A Practical Introduction to Kafka Storage Internals](https://medium.com/@durgaswaroop/a-practical-introduction-to-kafka-storage-internals-d5b544f6925f)
