# Advanced RAG Workshop - Implementation Complete ✅

**Status:** All 11 demos implemented and ready for workshop delivery  
**Completion Date:** October 16, 2025  
**Framework:** LlamaIndex + Azure OpenAI

---

## Quick Start

### Prerequisites
- Python environment with `uv` package manager
- Azure OpenAI API credentials (GPT-4 and text-embedding-ada-002)
- Environment variables configured:
  - `AZURE_OPENAI_API_KEY`
  - `AZURE_OPENAI_ENDPOINT`

### Running the Demos

Each demo is a self-contained Jupyter notebook. Execute them in order for the best learning experience:

```bash
# Navigate to the workshop directory
cd RAG_graph_v5

# Open a demo in Jupyter
jupyter notebook demo_01_hyde_query_enhancement.ipynb
```

---

## Demo Overview

| # | Demo | File | Concepts | Status |
|---|------|------|----------|--------|
| 1 | HyDE Query Enhancement | `demo_01_hyde_query_enhancement.ipynb` | Hypothetical documents, semantic gap | ✅ |
| 2 | Multi-Query Decomposition | `demo_02_multi_query_decomposition.ipynb` | RAG-Fusion, RRF algorithm | ✅ |
| 3 | Hybrid Search | `demo_03_hybrid_search.ipynb` | Dense + Sparse retrieval, weighted fusion | ✅ |
| 4 | Hierarchical Retrieval | `demo_04_hierarchical_retrieval.ipynb` | Sentence windows, chunking dilemma | ✅ |
| 5 | Re-ranking with Cross-Encoders | `demo_05_reranking_cross_encoders.ipynb` | Two-pass retrieval, precision optimization | ✅ |
| 6 | Context Compression | `demo_06_context_compression.ipynb` | Token optimization, information distillation | ✅ |
| 7 | Corrective RAG | `demo_07_corrective_rag.ipynb` | Self-reflection, adaptive routing | ✅ |
| 8 | Self-RAG | `demo_08_self_rag.ipynb` | Reflection tokens, meta-reasoning | ✅ |
| 9 | Agentic RAG | `demo_09_agentic_rag.ipynb` | ReAct framework, multi-source synthesis | ✅ |
| 10 | GraphRAG | `demo_10_graphrag.ipynb` | Knowledge graphs, multi-hop reasoning | ✅ |
| 11 | RAG Evaluation | `demo_11_rag_evaluation.ipynb` | 5 core metrics, automated testing | ✅ |

---

## Workshop Structure

### Phase 1: Pre-Retrieval Optimization (Demos 1-3)
**Duration:** ~2 hours  
**Focus:** Query transformation and hybrid search strategies

Learn how to:
- Bridge the semantic gap with HyDE
- Increase recall with query decomposition
- Combine dense and sparse retrieval

### Phase 2: Post-Retrieval Refinement (Demos 4-6)
**Duration:** ~2 hours  
**Focus:** Context optimization and quality enhancement

Learn how to:
- Separate retrieval granularity from generation context
- Re-rank with cross-encoders for precision
- Compress context while preserving information

### Phase 3: Adaptive Systems (Demos 7-8)
**Duration:** ~2 hours  
**Focus:** Self-reflective and corrective mechanisms

Learn how to:
- Build self-correcting RAG systems
- Implement adaptive retrieval decisions
- Use reflection tokens for meta-reasoning

### Phase 4: Advanced Architectures & Evaluation (Demos 9-11)
**Duration:** ~2 hours  
**Focus:** Complex systems and production practices

Learn how to:
- Route queries across heterogeneous data sources
- Leverage knowledge graphs for multi-hop reasoning
- Evaluate and monitor RAG systems in production

---

## File Structure

```
RAG_demo/
├── README.md                                    # This file
├── WORKSHOP_COMPLETION_SUMMARY.md               # Detailed completion report
├── workshop_demo_plan.md                        # Technical implementation plan
│
├── demo_01_hyde_query_enhancement.ipynb         # HyDE implementation
├── demo_02_multi_query_decomposition.ipynb      # RAG-Fusion implementation
├── demo_03_hybrid_search.ipynb                  # Dense + Sparse retrieval
├── demo_04_hierarchical_retrieval.ipynb         # Sentence Window Retrieval
├── demo_05_reranking_cross_encoders.ipynb       # Two-pass re-ranking
├── demo_06_context_compression.ipynb            # Context optimization
├── demo_07_corrective_rag.ipynb                 # Self-reflective retrieval
├── demo_08_self_rag.ipynb                       # Reflection tokens
├── demo_09_agentic_rag.ipynb                    # ReAct agents
├── demo_10_graphrag.ipynb                       # Knowledge Graph RAG
├── demo_11_rag_evaluation.ipynb                 # Evaluation framework
│
└── data/                                        # Demo datasets
    ├── ml_concepts/                             # Machine learning documents
    ├── tech_docs/                               # Technical documentation
    ├── long_form_docs/                          # Long-form articles
    └── finance_docs/                            # Business documents
```

---

## Technical Stack

- **Framework:** LlamaIndex (llama-index-core)
- **LLM:** Azure OpenAI GPT-4
- **Embeddings:** Azure OpenAI text-embedding-ada-002
- **Re-ranking:** sentence-transformers (ms-marco-MiniLM-L-6-v2)
- **Graph Processing:** NetworkX
- **Data Analysis:** pandas, numpy, scikit-learn

---



## Troubleshooting

### Common Issues

**Issue:** Azure OpenAI authentication error  
**Solution:** Verify environment variables are set:
```bash
echo $AZURE_OPENAI_API_KEY
echo $AZURE_OPENAI_ENDPOINT
```

**Issue:** Missing dependencies  
**Solution:** Install required packages:
```bash
pip install llama-index-core llama-index-llms-azure-openai llama-index-embeddings-azure-openai
pip install llama-index-retrievers-bm25 sentence-transformers networkx
```

**Issue:** Data files not found  
**Solution:** Ensure you're running notebooks from the `RAG_graph_v5` directory

---

## Citations and References

All demos cite their source materials from:
- Academic papers (e.g., Self-RAG - arXiv:2310.11511)
- Industry best practices (Microsoft, Google Cloud, IBM)
- Technical blogs (LangChain, Weights & Biases, Neo4j)
