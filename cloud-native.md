# En route vers les applications Cloud native

## From mainframe to software defined

- More terminals, more powerfull, more generic
- Standard hardware
- Hardware turned into software logic
- Scale up no longer sufficient (cannot get more powerfull chips)
- Need to scale out (horizontal), brings new methods, complex developments
- Leads to distributed applications
- - Consistency, Availabilty, Partition tolerance (network issues)
- - Can only get two properties (formal validation 2002, brewer/CAP theorem)
- - Cloud providers provide guarantee in a region (scale down)
- - Cloud providers cannot garantee partition tolerance for a massive deployment !!!
- - Applications need to adapt to compensate for partition tolerance
- - Difference SLA cloud provider / SLA software owner
- From MTBF (maximizing time bon fonctionnement) to MTTR (minimal time to normal return)

## Design patterns

Monolithic pattern is the worst pattern for the cloud.

- Resilience
- - Allow degraded mode
- Disponibility
- Elasticity
- - Financial optimization
- Low coupling
- - Standard protocols
- Continuous
- - IAC / CAC
- Software patterns:
- - Retry
- - Partition tolerances failures
- - Circuit breaker:
- - Degraded service, acknowledging to client
- - Low coupling
- - Storing failed requests, replaying them when service is back
- - Table store (No SQL)
- - Command and Query Responsibility Segregation
- - Event sourcing (transactions)
- - Messaging
- - Queue
- - Pub/Sub
- - Low SLA coupling

## Moving to the cloud

- Lift & Shift
- - Application non stateless
- - IAAS
- Cloud ready
- - Application stateless
- - Application supports main design patterns
- Cloud native
- - Microservices
- - Containers
- - Serverless