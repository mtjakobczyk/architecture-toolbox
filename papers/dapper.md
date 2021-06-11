###  Dapper, a Large-Scale Distributed Systems Tracing Infrastructure
Google Technical Report dapper-2010-1, April 2010
https://research.google/pubs/pub36356/

#### Goal
> "We built Dapper to provide Google’s developers with more information about the behavior of complex distributed systems."

#### Fundamental requirements
> "two fundamental requirements for Dapper: ubiquitous deployment, and continuous monitoring."

1. ubiquity (omnipresence, *Allgegenwart*)
> "the usefulness of a tracing infrastructure can be severly impacted if even small parts of the system are not being monitored."
2. continuity (*Kontinuität*)
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

##### Low overhead & Scalability
> Making the system scalable and reducing performance overhead was facilitated by the use of adaptive sampling

> we have found that a sample of just one out of thousands of requests provides sufficient information for many common uses of the tracing data

##### Application-level transparency
> was achieved by restricting Dapper’s core tracing instrumentation to a small corpus of ubiquitous threading, control flow, and RPC library code


#### Trace trees and spans
> We tend to think of **a Dapper trace as a tree of nested RPCs**. However, our core data model is not restricted to our particular RPC framework; we also trace activities such as SMTP sessions in Gmail, HTTP requests from the outside world, and outbound queries to SQL servers.

##### Spans
> In a Dapper trace tree, the tree nodes are basic units of work which we refer to as spans. The edges indicate a casual relationship between a span and its parent span.

![image](https://user-images.githubusercontent.com/6499023/121695074-02423f80-cacb-11eb-92a1-22e6e77c9f00.png)

> **a span** is also a simple log of timestamped records which encode the span’s start and end time, any RPC timing data, and zero or more application-specific annotations

> Dapper records **a human-readable span name** for each span, as well as **a span id** and **parent id** in order to reconstruct the causal relationships between the individual spans in a single distributed trace. Spans created without a parent id are known as root spans. All spans associated with a specific trace also share a common **trace id**. All of these ids are probabilistically unique 64-bit integers.
