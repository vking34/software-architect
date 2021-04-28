# Solution Architectural

This is my note, my experience for architectural principles, patterns and solutions.

## Principles

- Use local memory to handle high concurrency transaction

- Non blocking architecture

- Trade-offs consistency vs eventual consistency

- Reliable replication

- Authority: each service owns its problems

## Notes

- The more threads does mean the faster

## Practises

- Cache:

    - Cache data in local memory

    - Subscribe change event to invalid cache

- Non blocking http web server

- Compress to reduce payload size

- Single partition in Kafka:

    - All write request are routed to Kafka

    - Guaranteen ordering

    - Process exect one

    - When crash restore from last offset

- All changes in cache are flushed to DB asynchronously

- Non Blocking architecture using single thread business logic process

- Ring Buffer data structure to communicate between processors

## Technologies

- Guava

- Gridgo - Async IO & event driven framework

- Compress:
    - Single: gzip
    - Multiple: Snappy

- LMax/Ring Buffer

- ZeroMQ: return async message
