# Limitations

1. Query optimization is workload-specific — no universal solution
2. Indexing improves reads at the cost of writes
3. Cannot optimize around poorly designed application queries
4. Partitioning adds operational complexity
5. Schema changes require migrations and downtime consideration
6. ORMs may generate suboptimal queries that are hard to tune
7. Cloud-managed databases limit configuration access
8. Replication lag can cause read-after-write consistency issues
