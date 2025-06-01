# RAG over YouTube Videos (with LangChain)

Built a Retrieval-Augmented Generation pipeline using LangChain — but instead of PDFs or plain docs, I used **YouTube transcripts** as the knowledge source.

This notebook runs through:
- Pulling transcripts from a YouTube video
- Chunking + embedding them with OpenAI
- Storing them in a FAISS vector store
- Retrieving relevant chunks based on your question
- Passing those chunks into an LLM to get an actual answer

---

### Why I built this?

I wanted to try out RAG without relying on wrappers or black-box APIs. Also — YouTube videos are underrated data sources, and I was curious if I could build a chatbot that understands one.

---

### Stack

- LangChain
- FAISS
- OpenAI (embeddings + LLM)
- YouTubeTranscript API
- Jupyter

---

### Try it out!

1. Install deps  
   `pip install -r requirements.txt`

2. Open the notebook  
   `jupyter notebook chatbot.ipynb`

3. Drop in a YouTube link + OpenAI key  
   Ask it questions like:  
   > “What was the speaker's main argument in the first 10 mins?”

---

That’s it. Still improving this.
