# Quality Checklist

## RAG Architect

### Design
- [ ] Document types analyzed and chunking strategy selected
- [ ] Embedding model chosen for domain
- [ ] Vector store configured with appropriate index
- [ ] Hybrid search strategy defined
- [ ] Reranking stage included if needed

### Implementation
- [ ] Chunking implemented with configurable parameters
- [ ] Embedding pipeline handles batch processing
- [ ] Retrieval includes metadata filtering
- [ ] Error handling for failed retrievals

### Evaluation
- [ ] Recall@k >= 0.85
- [ ] Precision@k >= 0.70
- [ ] p99 latency < 500ms
- [ ] Tested with diverse query types
- [ ] Benchmark against baseline retrieval method
