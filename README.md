Flnk version of inventory item aggregator

```sh
docker-compose up
```

Note: the `flink_job` service currently fails until the `item` topic appears in Kafka.
Once items are generated, run `docker-compose start flink_job` tp start the job.

As new items appear in Kafka, insert and update entries will appear in the stdout log.
