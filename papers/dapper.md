###  Dapper, a Large-Scale Distributed Systems Tracing Infrastructure
Google Technical Report dapper-2010-1, April 2010
https://research.google/pubs/pub36356/

#### Goal
> "We built Dapper to provide Google’s developers with more information about the behavior of complex distributed systems."

#### Fundamental requirements
> "two fundamental requirements for Dapper: ubiquitous deployment, and continuous monitoring."

1. ubiquity (omnipresence, *Allgegenwart*)
> "the usefulness of a tracing infrastructure can be severly impacted if even small parts of the system are not being monitored."
2. continuity
> monitoring should always be turned on, because it is often the case that unusual or otherwise noteworthy system behavior is difficult or impossible to reproduce."

#### Design goals
1. Low overhead: 
   > the tracing system should have negligible performance impact on running services.
2. Application-level transparency: 
   > programmers should not need to be aware of the tracing system.
3. Scalability:
   > it needs to handle the size of Google’s services and clusters for at least the next few years.
4. Enabling fast reaction:
   > tracing data to be available for analysis quickly after it is generated: ideally within a minute
