# OCC vs. PCC
Optimistic Concurrency Control vs. Pessimistic Concurrency Control

## Same

## Differences
| | OCC | PCC |
|----|----|----|
| Assumption | Conflicts between transactions will happen infrequently. | Conflicts between transactions will happen frequently. |
| Lock-based (Use locks) | No | Yes |
| Degree of concurrency | High | Low |
| Will deadlock happen | No | Yes |
| Better for scaling | Yes | No |
| When to use | Few data conflicts. | More data conflicts. |
