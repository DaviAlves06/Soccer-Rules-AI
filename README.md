### ⚽ Soccer Rules AI (RAG Notebook)

Este repositório contém um ambiente de experimentação em **IA Generativa** focado nas regras oficiais do futebol. O projeto utiliza a técnica de **RAG (Retrieval-Augmented Generation)** dentro de um Jupyter Notebook para permitir consultas semânticas a documentos técnicos (PDFs).

---

### 🎯 Proposta do Projeto

Diferente de uma IA comum, este notebook configura um pipeline que lê manuais de arbitragem e permite que o usuário tire dúvidas específicas. É uma prova de conceito (PoC) sobre como especializar LLMs em nichos com alta densidade de regras.

### 🛠️ Tecnologias e Frameworks

* **Linguagem:** Python (executado via Google Colab)
* **IA:** Google Gemini 1.5 Flash (via `langchain-google-genai`)
* **Orquestração RAG:** `LangChain`
* **Banco de Vetores:** `ChromaDB` (efêmero/em memória para o notebook)
* **Embeddings:** `HuggingFace` (Sentence Transformers)

---

### 🚀 Como utilizar (Passo a Passo)

1. **Abrir no Colab:** Clique no arquivo `.ipynb` e selecione "Open in Colab".
2. **Download da Base de Conhecimento:** Para que a IA funcione, ela precisa do manual oficial. Baixe a versão mais recente aqui:
   - [📥 Download Laws of the Game 24/25 (IFAB)] ([https://www.theifab.com/en/downloads/laws-of-the-game-2024-25/](https://www.theifab.com/laws-of-the-game-documents/?language=all&year=2024%2F25))
3. **Upload:** Envie o arquivo para o ambiente do Colab.
4. **Execução:** Siga as células do notebook inserindo sua `GOOGLE_API_KEY`.

---

### 🔬 O que este notebook demonstra?

* **Document Loading:** Extração de texto de PDFs complexos usando `PyPDFLoader`.
* **Text Splitting:** Divisão inteligente de parágrafos para manter o contexto das regras.
* **Vector Search:** Como transformar texto em vetores matemáticos para busca por significado (e não apenas palavras-chave).
* **Prompt Engineering:** Configuração de um sistema que atua como um árbitro oficial, citando trechos do manual.

---

### 👨‍💻 Sobre o Autor

**Davi Alves** Estudante de Engenharia de Software na FIAP. Este projeto faz parte do meu portfólio de estudos em **Inteligência Artificial Aplicada**.

---

### 💡 Dica para o seu Portfólio:

Como o PDF não está no GitHub, eu recomendo que você coloque um link no README para onde o recrutador pode baixar o PDF oficial (ex: site da IFAB ou CBF). Isso facilita muito para quem quiser testar seu código!

**Davi, agora que ajustamos para o formato Notebook, você quer que eu faça o mesmo ajuste para o seu projeto do Agente Farmacêutico?**
