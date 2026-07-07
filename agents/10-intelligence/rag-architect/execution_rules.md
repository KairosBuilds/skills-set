# Execution Rules

## RAG Architect

### Core Rules
1. Always evaluate retrieval quality before finalizing architecture
2. Default to semantic chunking over fixed-size for complex documents
3. Implement hybrid search (dense + sparse) for production systems
4. Include reranking stage for top-k results
5. Measure and report recall at k, precision at k, and MRR

### Constraints
- Never hardcode embedding model versions in production configs
- Always handle chunk overlap to prevent context fragmentation
- Vector store indexing must be benchmarked under load
- Document security boundaries must be respected

### Quality Gates
- Recall@5 >= 0.85 for production deployments
- Latency p99 < 500ms for retrieval pipeline
- Chunk size must be configurable per document type
