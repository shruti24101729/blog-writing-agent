# 📝 Blog Writing Agent (LangGraph + LLM)

An **AI-powered Blog Writing Agent** that automatically plans,
researches, writes, and assembles high‑quality blog posts using
**LangGraph, LangChain, and LLMs**.

The system follows a **multi-agent workflow** including routing,
research, task orchestration, content generation, and image placement.

It also provides a **Streamlit UI** where users can generate blogs
interactively and export them as Markdown + images.

------------------------------------------------------------------------

# 🚀 Features

-   Automatic **blog planning and task decomposition**
-   Intelligent **research routing (closed-book / hybrid / open-book)**
-   Multi-agent **parallel content generation**
-   Automatic **image generation and placement**
-   Blog export as **Markdown + ZIP bundle**
-   Interactive **Streamlit web interface**

------------------------------------------------------------------------

# 🏗️ Architecture

User Input → Router Agent → Research Agent → Planner → Worker Agents
(Parallel) → Reducer → Final Blog Output

------------------------------------------------------------------------

# 📂 Project Structure

blog-writing-agent/

-   bwa_backend.py --- LangGraph multi-agent workflow\
-   bwa_frontend.py --- Streamlit UI\
-   agent.ipynb --- Notebook for experimentation\
-   .env --- Environment variables\
-   README.md

------------------------------------------------------------------------

# ⚙️ Tech Stack

-   Python
-   LangGraph
-   LangChain
-   OpenAI / LLM APIs
-   Streamlit
-   Pydantic
-   Pandas

------------------------------------------------------------------------

# 💻 Installation



## 1. Create Virtual Environment

python -m venv venv

Activate environment

Windows: venv`\Scripts`{=tex}`\activate`{=tex}

Mac/Linux: source venv/bin/activate

## 2. Install Dependencies

pip install -r requirements.txt



## 3. Setup Environment Variables

Create `.env` file:

OPENAI_API_KEY=your_api_key_here

------------------------------------------------------------------------

# ▶️ Running the Application

streamlit run bwa_frontend.py

Then open:

http://localhost:8501

------------------------------------------------------------------------

# 🧠 Example Usage

Topic: How Transformers Work in Machine Learning\
Audience: Beginners\
Tone: Educational

The agent will: 1. Plan blog structure 2. Research if needed 3. Generate
sections 4. Insert images 5. Export blog as Markdown

------------------------------------------------------------------------

# 📦 Export Options

Generated blog can be downloaded as:

-   Markdown file
-   ZIP bundle (markdown + images)

------------------------------------------------------------------------

# 🧪 Notebook

`agent.ipynb` can be used for:

-   testing LangGraph workflow
-   debugging agents
-   experimenting with prompts

------------------------------------------------------------------------


# 📜 License

MIT License
