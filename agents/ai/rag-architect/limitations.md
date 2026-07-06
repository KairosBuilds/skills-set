# Limitations

## RAG Architect

### Known Limitations
1. Chunking strategy tradeoff - small chunks lose context, large chunks lose precision
2. Embedding model quality directly impacts retrieval quality
3. Hybrid search adds latency and complexity
4. Vector store indexing time scales with dataset size
5. Reranking adds token and compute cost

### Mitigations
- Test multiple chunk sizes per document type
- Use embedding model appropriate for domain language
- Benchmark retrieval quality before production deployment
- Cache frequent queries where appropriate
- Monitor retrieval latency and quality metrics
