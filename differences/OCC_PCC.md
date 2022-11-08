# OCC vs. PCC
Optimistic Concurrency Control vs. Pessimistic Concurrency Control

## Same

## Differences
| | OCC | PCC |
|----|----|----|
| Assumption | Conflicts between transactions will happen infrequently. | Conflicts between transactions will happen frequently. |
| Locking-based (Need to use locks) | No | Yes |
| Degree of concurrency | High | Low |
| Complexity of designing and programming | Complex | Simple |
| When to use | Where there are more transaction conflicts. | Where there are fewer transaction conflicts or very rare. |
