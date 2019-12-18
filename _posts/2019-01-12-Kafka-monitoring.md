---
layout: post
title: Kafka - Monitoring
edited: true
---

# Introduction

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

## Topic

- Topic is the logical grouping

- Each topic is assigned with at least 1 partition (in this case, `my-topic` has two partitions, hence `my-topic-0,1,2`)

## Partition

![]()

- Partition is a storage unit in Kafka
