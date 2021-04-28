# Solution Architectural

This is my note, my experience for architectural principles, patterns and solutions.

## Principles

- Use local memory to handle high concurrency transaction

- Non blocking architecture

- Trade-offs consistency vs eventual consistency

- Reliable replication

- Authority: each service owns its problems

## Practises

- Cache:

    - Cache data in local memory

    - Subscribe change event to invalid cache

- Non blocking http web server

- Compress to reduce payload size


## Technologies

- Guava

- Gridgo - Async IO & event driven framework

- Compress:
    - Single: gzip
    - Multiple: Snappy