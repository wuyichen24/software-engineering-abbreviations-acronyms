# ACID: Atomicity, Consistency, Isolation, and Durability

## Name

## Overview
- A set of properties of database transactions intended to guarantee data validity despite errors, power failures, and other mishaps.
   - **Atomicity**: Each transaction is treated as a single unit, which either succeeds completely, or fails completely.
   - **Consistency**: Each transaction can only bring the database from one valid state to another and always obey database invariants (rules).
   - **Isolation**: Concurrently executing transactions shouldn’t interfere with each other.
   - **Durability**: Once a transaction has committed successfully, any data it has written will not be forgotten, even if there is a hardware fault or the database crashes.
- It guarantees consistency over availability.
- It is the opposite of [BASE](../B/BASE-Basically_Available_Soft_State_Eventually_Consistent.md).

## Description

## See also

## Wiki
- [ACID](https://en.wikipedia.org/wiki/ACID)

## References
- [Github | wuyichen24/system-design-knowledge](https://github.com/wuyichen24/system-design-knowledge/blob/master/concepts/Transaction.md#acid-consistency-over-availability)
