# YouTube Video RAG System

A Retrieval Augmented Generation (RAG) system that allows you to have intelligent conversations about YouTube video content using Large Language Models.

## 🌟 Features

- YouTube transcript extraction
- Text chunking and embedding generation
- Semantic search using vector stores
- Intelligent question answering using OpenAI's GPT-3.5
- Support for multiple vector store backends (DocArrayInMemorySearch, Pinecone)
- Translation capabilities for multilingual support

## 🛠️ Technology Stack

- Python 3.12+
- LangChain
- OpenAI GPT-3.5
- youtube-transcript-api
- DocArray/Pinecone for vector storage
- scikit-learn for similarity computations

## 🚀 Getting Started

1. Clone the repository:
bash
git clone <your-repo-url>
cd <your-repo-name>

2. Install dependencies:
bash
pip install -r requirements.txt

3. Set up environment variables:
bash
OPENAI_API_KEY=your_openai_api_key

4. Run the Jupyter notebook:
bash
jupyter notebook rag.ipynb

## 💡 Usage

1. Set your YouTube video URL:
python
YOUTUBE_VIDEO = "https://www.youtube.com/watch?v=your_video_id"

2. The system will automatically:
   - Extract the video transcript
   - Split it into manageable chunks
   - Generate embeddings
   - Store them in a vector database

3. Ask questions about the video content:
python
chain.invoke("What is synthetic intelligence?")

## 🌐 Advanced Features

### Translation Support
Query in one language and get responses in another:
python
translation_chain.invoke({
"context": "your_context",
"question": "your_question",
"language": "French"
})

### Vector Store Options
- In-memory storage using DocArrayInMemorySearch
- Cloud-based storage using Pinecone
- Easy extension to other vector store backends

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

Your Name - [your.email@example.com](mailto:your.email@example.com)

Project Link: [https://github.com/yourusername/your-repo-name](https://github.com/yourusername/your-repo-name)