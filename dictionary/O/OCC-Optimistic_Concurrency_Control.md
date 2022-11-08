# OCC: Optimistic Concurrency Control

## Name

## Overview
- A collection of concurrency control methods based on assumption that multiple transactions can frequently complete without interfering with each other.
- It is the opposite of PCC.

## Description
- **Phases of OCC**
   - **Begin**: Record a timestamp marking the transaction's beginning.
   - **Modify**: Read database values, and tentatively write changes.
   - **Validate**: Check whether other transactions have modified data that this transaction has used (read or written). This includes transactions that completed after this transaction's start time, and optionally, transactions that are still active at validation time.
   - **Commit/Rollback**: If there is no conflict, make all changes take effect. If there is a conflict, resolve it, typically by aborting the transaction

## See also

## Wiki
- [Optimistic concurrency control](https://en.wikipedia.org/wiki/Optimistic_concurrency_control)

## References
