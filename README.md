# udacity_kafka_spark_project
 
#### Question 1
It had a direct affect on the number of rows processed per second ```processedRowsPerSecond```. It either increased or decreased.

#### Question 2
Options:
```
spark.sql.shuffle.partitions                10
spark.streaming.kafka.maxRatePerPartition   10
spark.default.parallelism                   10000
```

By setting them to these values, I observed that the rows per second drastically increased. Namely, increasing maxOffsetPerTrigger also increased the throughput.