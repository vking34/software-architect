# Solutions


## Memory Bottlneck

- Using a Key-Value store, instead of in-memory index

#
## CPU pressure


### Heap Optimization:
- Cleaning up unused data fields
- Reducing the number of long-living objects in favor of creating objects on demand
- Pool objects to reduce large allocation bursts
- References:
    - https://medium.com/swlh/memory-optimizations-for-go-systems-48d95cf64a13
    - https://www.youtube.com/watch?v=BYi9zzGGtDc
#
## Scale & Latency

### Parallelization

- Run independent services parallel

### Caching

- Implementing a local cache with TTL of minutes (depend on your business), to maintain a balance high traffic and data freshes

#

## Data Delay

### Real-Time Updates

- Stream Processing to update data (Kafka Stream, ...)