# Non-Functional Requirements

## Availibility

- Availability is the __percentage of time__ system is __up__ in a defined timeframe.


## Scalability

- Scalability is __how the system resources can cope up with unpredictable customer demands__.

## Resiliency

- Resiliency is the ability of a system to __gracefully handle the failures__ and recover from failures as soon as it can.

## Data Management
- Data management plays a crucial role in scalability, availability, security and resiliency. Architectural decisions related to data management depends on what type of application you are building. Is it write heavy (more user transactions), read-heavy (reports), meant to do analytics (forecasting, customer segmentation), time series (log processing) or Datawarehouse (data analytics). 
- Few other factors that would influence are data consistency, data availability, data storage and archival strategy.

## Performace
- Scalability and performance are interrelated. If there are more users compared to what the system can handle, it is natural that the system would encounter performance issues. How to deal with this?

- In fact, we will sort out these performance issues when you sort out scalability issues. __Scalability can’t solve all the performance issues but can solve some issues__. For example, if the performance issues are the result of badly written DB query, scaling the resources without fine-tuning the query will prove to be a disastrous decision.

## Security
- Building secure systems gives an assurance to users that their data is in safe hands. Data integrity and data durability are equally important.
