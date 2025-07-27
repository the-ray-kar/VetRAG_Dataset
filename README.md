# Everything About Dogs: Agentic RAG Dataset

This repository contains a structured dataset for building Retrieval-Augmented Generation (RAG) and agentic AI applications focused on canine health, care, and knowledge. The data is extracted and processed from the public domain book **"Everything About Dogs" by A.L.G. Eberhart**.

### In Memory of Caspu
<img src="https://github.com/the-ray-kar/VetRAG_Dataset/blob/fa0621aad162fe121563058ebc91df5e0008b601/caspu.jpg?raw=true" width="400" />
Dogs can't speak but they can express their pain. However this expression is often misunderstood or ignored.
<br>My I aim to build a retrieval engine from trusted resources which can provide answers to me everything about dogs.


## Dataset Overview

- **Source**: "Everything About Dogs" by A.L.G. Eberhart (public domain)
- **Format**: Cleaned text, chapter-wise files, disease-specific JSON, embeddings, and reference mappings
- **Purpose**: To enable advanced question answering, knowledge retrieval, and agentic workflows for dog-related topics

## Folder Structure

- `ChaptersRaw/` — Raw chapter text files as extracted from the book
- `ChaptersCleaned/` — Cleaned and preprocessed chapter files, including:
  - Individual chapter texts
  - `everything_about_dogs_diseases.json`: Disease name to description mapping
  - `everything_about_dogs_diseases_references.json`: Disease cross-references
  - `everything_about_dogs_diseases_master.json`: Disease details (description, references, symptoms, when to approach a vet, food recommendations)
  - `index.json`: Summaries of each chapter
- `Final Data/` — Processed datasets with embeddings for downstream ML/RAG tasks
- `diseases_embedding_model/` — SentenceTransformer model for generating embeddings
- `everythingaboutdogs.pdf` — Original book (if available)

## Key Features

- **Disease Knowledge Graph**: Each disease is mapped to its description, references to other diseases, symptoms, vet-visit triggers, and dietary advice.
- **Chapter Summaries**: Each chapter is summarized for quick retrieval and context.
- **Embeddings**: Text chunks and disease entries are embedded for semantic search and RAG pipelines.
- **Agentic RAG Ready**: Data is structured for use with agentic frameworks (e.g., Pydantic AI, Gemini, etc.)

## Example Use Cases

- Build a chatbot to answer dog health questions using RAG
- Retrieve disease symptoms, treatments, and references programmatically
- Explore relationships between diseases and chapters
- Fine-tune or evaluate LLMs on veterinary knowledge

## Citation

> Eberhart, A.L.G. (Year). Everything About Dogs. [Public Domain Book]

## License

This dataset is derived from a public domain source. All code and data processing scripts are released under the MIT License.

