# BASE: Basically Available, Soft state, Eventually consistent

## Name

## Overview
- A set of properties of distributed transactions intended to guarantee data validity despite errors, power failures, and other mishaps.
   - **Basically Available**: Basic reading and writing operations are available as much as possible (using all nodes of a database cluster), but without any kind of consistency guarantees (the write may not persist after conflicts are reconciled, the read may not get the latest write).
   - **Soft state**: Without consistency guarantees, after some amount of time, we only have some probability of knowing the state, since it may not yet have converged.
   - **Eventually consistent**: If the system is functioning and we wait long enough after any given set of inputs, we will eventually be able to know what the state of the database is, and so any further reads will be consistent with our expect.
- It guarantees availability over consistency.
- It is the opposite of [ACID](../A/ACID-Atomicity_Consistency_Isolation_Durability.md).

## Description

## See also

## Wiki
- [Eventual consistency](https://en.wikipedia.org/wiki/Eventual_consistency)

## References
- [Github | wuyichen24/system-design-knowledge](https://github.com/wuyichen24/system-design-knowledge/blob/master/concepts/Transaction.md#base-availability-over-consistency---eventual-consistency)
