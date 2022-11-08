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
   - Read-lock doesn't block other read-locks and only blocks other write-locks:
      - Several transactions are allowed to concurrently read the same object.
      - If transaction A has read an object and transaction B wants to write to that object, B must wait until A commits or aborts before it can continue.
   - Write-lock blocks both other read-locks and other write-locks:
      - If transaction A has written an object and transaction B wants to read that object, B must wait until A commits or aborts before it can continue.
      - If transaction A has written an object and transaction B wants to write that object, B must wait until A commits or aborts before it can continue.

## See also

## Wiki
- [Two-phase locking](https://en.wikipedia.org/wiki/Two-phase_locking)

## References
