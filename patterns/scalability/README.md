# Scalability

## Patterns

- __Load Balancer__ - a dispatcher determines which worker instance will handle a request based on different policies.

- __Scatter and Gather__ - a dispatcher multicasts requests to all workers in a pool. Each worker will compute a local result and send it back to the dispatcher, who will consolidate them into a single response and then send back to the client.

- __Result Cache__ - a dispatcher will first lookup if the request has been made before and try to find the previous result to return, in order to save the actual execution.

- __Shared Space__ - all workers monitors information from the shared space and contributes partial knowledge back to the blackboard. The information is continuously enriched until a solution is reached.

- __Pipe and Filter__ - all workers connected by pipes across which data flows.

- __MapReduce__ -  targets batch jobs where disk I/O is the major bottleneck. It use a distributed file system so that disk I/O can be done in parallel.

- __Bulk Synchronous Parallel__ - a  lock-step execution across all workers, coordinated by a master.

- __Execution Orchestrator__ - an intelligent scheduler / orchestrator schedules ready-to-run tasks (based on a dependency graph) across a clusters of dumb workers.


## References

- http://highscalability.com/blog/2010/12/1/8-commonly-used-scalable-system-design-patterns.html

- https://dzone.com/articles/scalable-system-design

