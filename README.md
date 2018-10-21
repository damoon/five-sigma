# five sigma

let's think about software design.

## Axioms

The purpose of software is to fullfil a use.

Lifetime is the most precious resource.

Every software will always have bugs.

Hardware is physical and will change over time.

### Logical conduction

Requirements will change. Example: Users change behavior, the data set changes, bugs get discovered.

Every hardware will fail at some point in time. Example: Hardware will physically break or needs downtime to be upgraded.

Later versions of a component may change properties away from the attributes we rely on. Example: Processor frequency per cpu core reduced after its peak https://queue.acm.org/detail.cfm?id=2181798 http://deliveryimages.acm.org/10.1145/2190000/2181798/horowitz_fig7.png

Software parts that are not used need to be removed to get rid of useless complexity, reduce the habitat of bugs, and minimize mental workload for developers.

Outside of exploratory learning phases nobody wants to spend more time using a paradigm then needed.

Source code of far more read then written.

Deployment should be possible at any time.

## sorted Priorities

- mutable source code / agility
- observability
- reliable
- correct
- comprehensible

### Reasoning

Not being able to adopt to new situations will lead to useless software. Being agile is more important then everything else.

To detect wrong behavior during production workloads and understand what features are actually used is more important then availability or a guaranteed bug free system.

A system needs to show the same behavior independent of external factors. A system acting on unknown inputs will behave flaky and never appear correct.

Incorrect systems need to get fixed or accept the reduced usefulness they provide. The correctness of a setup is in most cases more important then the ability to reason about it.

A system needs to actively remove unnecessary complexity and minimize necessary complexity or accept slowed down development speed.
