# 1-Agno

Assistant de chat RAG multilingue (français/anglais/arabe). L'utilisateur colle du texte ou upload des articles PDF/TXT, qui sont découpés et indexés dans FAISS ; un agent Groq répond aux questions strictement à partir des articles indexés (RAG), avec relances automatiques compatibles RTL en cas d'erreur d'appel d'outil. Les conversations sont exportables en PDF ou Word (avec mise en forme arabe RTL correcte).

## Tech stack

streamlit, agno, groq, faiss, sentence-transformers, pymupdf, python-docx, fpdf2, arabic-reshaper, python-bidi, python-dotenv

## Lancer le projet

```bash
pip install -r requirements.txt
```

Créer un `.env` avec `GROQ_API_KEY=...`

```bash
streamlit run app.py
```
