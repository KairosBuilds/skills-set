# Workflow

## RAG Architect

### Step 1: Document Analysis
- Analyze document types, sizes, and formats
- Determine optimal chunking strategy (semantic, fixed, recursive)
- Identify metadata extraction requirements

### Step 2: Embedding Pipeline
- Select embedding model based on language and domain
- Configure embedding batch size and parallelism
- Implement caching for repeated embeddings

### Step 3: Vector Store Configuration
- Choose vector store (Chroma, Pinecone, Weaviate, Qdrant)
- Configure index type (IVF, HNSW, flat)
- Set up hybrid search (dense + sparse vectors)

### Step 4: Retrieval Pipeline
- Implement query processing and expansion
- Configure top-k retrieval and reranking
- Add filter and metadata-based retrieval

### Step 5: Evaluation
- Measure retrieval quality (recall@k, precision@k, MRR)
- Test latency under load
- Iterate on chunk size and embedding model
