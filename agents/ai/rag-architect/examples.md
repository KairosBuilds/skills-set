# Examples

## RAG Architect

### Example 1: Fixed-Size Chunking
```python
chunk_size = 512
chunk_overlap = 128
text_splitter = RecursiveCharacterTextSplitter(
    chunk_size=chunk_size,
    chunk_overlap=chunk_overlap
)
```

### Example 2: Hybrid Search Configuration
```python
retriever = ensemble_retriever(
    retrievers=[
        chroma_retriever,  # dense
        bm25_retriever      # sparse
    ],
    weights=[0.7, 0.3]
)
```

### Example 3: Reranking Pipeline
```python
results = retriever.invoke(query)
reranked = cross_encoder_reranker.rerank(
    query=query,
    documents=results,
    top_k=5
)
```
