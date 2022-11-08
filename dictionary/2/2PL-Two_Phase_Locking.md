# 2PL: Two-Phase Locking

## Name
- Two-Phase Locking

## Overview
- A concurrency control method that guarantees serializability.
- 2 phases
   - 1st phase: Locks are acquired (While the transaction is executing)
   - 2nd phase: Locks are released (At the end of the transaction)

## Description
- **Types of locks**
   - Write-lock (exclusive lock): A transaction needs to acquire a read-lock before executing a wirte operation on an object.
   - Read-lock (shared lock): A transaction needs to acquire a read-lock before executing a read operation on an object.
- **Common interactions between locks**

## See also

## Wiki
- [Two-phase locking](https://en.wikipedia.org/wiki/Two-phase_locking)

## References
