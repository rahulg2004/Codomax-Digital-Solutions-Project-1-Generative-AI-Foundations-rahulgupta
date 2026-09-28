# 🤖 Generative AI Foundations

A practical Generative AI project developed as part of my **Generative AI Internship at Codomax Digital Solutions**. This project focuses on understanding the fundamentals of Generative AI, Large Language Models, prompt engineering, responsible AI, and practical AI application development using the **Google Gemini API**.

The project combines theoretical learning with hands-on experiments and an interactive chatbot powered by **Gemini 3.6 Flash**.

---

## 📌 Project Overview

Generative AI is a branch of Artificial Intelligence that enables machines to generate new content such as text, images, audio, video, and code.

This project was developed to build a strong foundation in Generative AI concepts while gaining practical experience with an LLM through API-based development.

The project covers:

* Generative AI fundamentals
* Large Language Models
* Tokens and context windows
* Transformer architecture
* Attention mechanisms
* Prompt Engineering
* Few-shot prompting
* AI hallucinations
* AI bias and limitations
* Responsible AI
* Generative AI application architecture
* Google Gemini API integration
* Interactive AI chatbot development
* AI model experimentation

---

## 🎯 Objectives

The main objectives of this project are:

1. Understand the fundamentals of Generative AI.
2. Learn how Large Language Models work at a conceptual level.
3. Understand tokens, context windows, Transformers, and attention.
4. Explore different prompt engineering techniques.
5. Experiment with AI-generated responses.
6. Understand hallucinations and AI limitations.
7. Learn responsible AI principles.
8. Integrate the Google Gemini API with Python.
9. Build a reusable AI interaction function.
10. Develop an interactive conversational AI chatbot.
11. Gain practical experience in building Generative AI applications.

---

## 🧠 Topics Covered

### 1. Generative AI

Generative AI refers to AI systems capable of creating new content based on learned patterns.

Examples include:

* Text generation
* Image generation
* Code generation
* Audio generation
* Video generation
* Conversational AI

---

### 2. Large Language Models

Large Language Models (LLMs) are AI models trained on large amounts of text data to understand and generate human-like language.

The project explores:

* How LLMs process text
* Tokenisation
* Context windows
* Text generation
* LLM applications
* Limitations of LLMs

---

### 3. Tokens

Tokens are smaller units of text processed by language models.

For example:

```text
Generative AI is powerful
```

may be divided into multiple tokens before being processed by an LLM.

Understanding tokens helps explain how language models process and generate text.

---

### 4. Context Windows

A context window represents the amount of information a model can consider during a particular interaction.

It affects:

* Conversation history
* Long documents
* Prompt size
* Model input and output
* Context-aware responses

---

### 5. Transformers

Transformers are a fundamental architecture behind modern Large Language Models.

The project explores:

* Transformer architecture
* Attention mechanism
* Self-attention
* Context understanding
* Sequence processing

---

## ✨ Prompt Engineering

Prompt Engineering involves designing effective instructions to guide an AI model towards useful and relevant outputs.

The project experiments with several prompting techniques.

### Basic Prompting

```text
Explain Generative AI in simple words.
```

### Role-Based Prompting

```text
You are a computer science teacher.

Explain Generative AI to a beginner.
Use simple language and two real-world examples.
```

### Structured Prompting

The model is instructed to organise its response into predefined sections.

### Few-Shot Prompting

Examples are provided to demonstrate the expected output format.

### Summarisation

The model is given a piece of text and instructed to generate a concise summary.

These experiments demonstrate how changing the structure and specificity of a prompt can influence the generated response.

---

## 🔍 Hallucination Awareness

Generative AI models can sometimes produce information that appears convincing but may not be factually correct.

The project includes a hallucination-awareness experiment using a fictional historical claim.

The experiment demonstrates the importance of:

* Fact verification
* Reliable sources
* Critical evaluation
* Distinguishing generated content from verified information
* Avoiding fabricated references

AI-generated information should not automatically be treated as verified information.

---

## 🛡️ Responsible AI

Responsible AI principles explored in this project include:

* **Fairness**
* **Privacy**
* **Security**
* **Transparency**
* **Accountability**
* **Human Oversight**

The project highlights the importance of using AI systems responsibly and evaluating their outputs before relying on them for important decisions.

---

# 🔗 Technology Stack

| Technology         | Purpose                         |
| ------------------ | ------------------------------- |
| Python             | Application development         |
| Google Gemini API  | Generative AI model interaction |
| Gemini 3.6 Flash   | AI text generation              |
| Google GenAI SDK   | Gemini API integration          |
| Google Colab       | Development and experimentation |
| NLP                | Natural language processing     |
| Prompt Engineering | Controlling AI responses        |

---

# 🏗️ Project Architecture

The basic application workflow is:

```text
User
  ↓
User Interface
  ↓
Prompt Handling
  ↓
Generative AI Application
  ↓
Google Gemini API
  ↓
Gemini 3.6 Flash
  ↓
Generated Response
  ↓
Response Processing
  ↓
User
```

---

# 📂 Project Structure

```text
Generative-AI-Foundations/
│
├── app.py
├── requirements.txt
├── .env
├── .env.example
├── .gitignore
└── README.md
```

### File Description

| File               | Description                                               |
| ------------------ | --------------------------------------------------------- |
| `app.py`           | Main Generative AI application                            |
| `requirements.txt` | Required Python dependencies                              |
| `.env`             | Stores API credentials locally                            |
| `.env.example`     | Example environment configuration                         |
| `.gitignore`       | Prevents sensitive/unnecessary files from being committed |
| `README.md`        | Project documentation                                     |

---

# ⚙️ Installation

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repository.git
```

Navigate into the project:

```bash
cd Generative-AI-Foundations
```

---

## 2. Create a Virtual Environment

### Windows

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### macOS/Linux

```bash
python3 -m venv venv
```

```bash
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 API Configuration

The application requires a Google Gemini API key.

Create an API key through **Google AI Studio** and store it securely.

For local development, create a `.env` file:

```env
GEMINI_API_KEY=your_api_key_here
```

Do not publish your actual API key on GitHub.

The `.env` file should be included in `.gitignore`.

Example:

```gitignore
.env
__pycache__/
venv/
*.pyc
```

---

# 🧪 Google Colab Setup

The practical experiments can also be performed in Google Colab.

Install the Google GenAI SDK:

```python
!pip -q install -U google-genai
```

Retrieve the API key securely from Colab Secrets:

```python
from google import genai
from google.colab import userdata

API_KEY = userdata.get("GEMINI_API_KEY")

if not API_KEY:
    raise ValueError(
        "GEMINI_API_KEY was not found. "
        "Add it to Google Colab Secrets and run this cell again."
    )

client = genai.Client(api_key=API_KEY)

print("Gemini API configured successfully.")
```

---

# 🤖 Gemini Model

This project uses:

```python
MODEL_NAME = "gemini-3.6-flash"
```

The project is designed around **Gemini 3.6 Flash** for the practical API experiments and chatbot.

---

# 💻 Basic Gemini API Usage

A simple request can be made using:

```python
response = client.models.generate_content(
    model="gemini-3.6-flash",
    contents="Explain Generative AI in simple words."
)

print(response.text)
```

---

# 🔄 Retry Handling

Temporary server-side availability issues can occur when working with cloud AI APIs.

The project therefore uses retry handling for temporary `503` or `UNAVAILABLE` errors.

Example:

```python
import time
from google.genai import errors

def generate_with_retry(prompt, max_retries=3):
    last_error = None

    for attempt in range(max_retries):
        try:
            response = client.models.generate_content(
                model="gemini-3.6-flash",
                contents=prompt
            )

            return response

        except errors.ServerError as error:
            last_error = error
            message = str(error)

            if (
                "503" in message
                or "UNAVAILABLE" in message
                or "high demand" in message
            ):
                wait_seconds = 2 ** attempt
                time.sleep(wait_seconds)
                continue

            raise

    raise RuntimeError(
        f"Gemini 3.6 Flash is currently unavailable. "
        f"Last error: {last_error}"
    )
```

---

# 💬 Interactive AI Chatbot

The project includes an interactive chatbot that accepts user questions and generates responses using Gemini 3.6 Flash.

Example workflow:

```text
User enters question
        ↓
Prompt sent to Gemini
        ↓
Gemini 3.6 Flash processes prompt
        ↓
AI generates response
        ↓
Response displayed to user
```

Example:

```text
🤖 Gemini 3.6 Flash Chatbot
Type 'exit' to stop.

You: What is a Transformer?

AI: ...
```

The chatbot continues accepting questions until the user enters:

```text
exit
```

---

# 🧪 Experiments

The project contains multiple practical experiments.

### Experiment 1: Basic Prompt

```text
Explain Generative AI in simple words.
```

### Experiment 2: Role Prompt

The AI is given a specific role such as a computer science teacher.

### Experiment 3: Structured Prompt

The AI is instructed to generate information using predefined sections.

### Experiment 4: Few-Shot Prompting

Examples are provided before requesting a new output.

### Experiment 5: Text Summarisation

A paragraph is provided and the model generates a concise summary.

### Experiment 6: Hallucination Awareness

The model is tested with a fictional claim to encourage separation between generated information and verified facts.

### Experiment 7: Responsible AI

The model explains important Responsible AI principles with practical examples.

---

# 📊 AI Model Comparison

A manual comparison experiment can be performed by using the same prompt with multiple AI assistants.

Example prompt:

```text
Explain Transformers to a first-year computer science student
using a simple real-world analogy.
```

The responses can be compared based on:

* Clarity
* Detail
* Structure
* Relevance
* Accuracy observations
* Ease of understanding

The Gemini API experiments in this project use **Gemini 3.6 Flash**.

---

# 📚 Learning Outcomes

Through this project, I gained practical understanding of:

* Generative AI
* Large Language Models
* Tokens
* Context windows
* Transformers
* Attention mechanisms
* Prompt Engineering
* Few-shot prompting
* NLP
* AI hallucinations
* Responsible AI
* AI application architecture
* API integration
* Conversational AI
* Python-based AI development

---

# 🛠️ Skills Gained

* Python
* Generative AI
* Large Language Models
* Prompt Engineering
* Google Gemini API
* Natural Language Processing
* Conversational AI
* Responsible AI
* AI Application Development
* Google Colab

---

# 🔐 Security Considerations

API keys should never be hardcoded into publicly shared source code.

Avoid:

```python
API_KEY = "your-real-api-key"
```

Instead, use environment variables or secure notebook secrets.

For Google Colab, use:

```python
userdata.get("GEMINI_API_KEY")
```

For local development, use:

```env
GEMINI_API_KEY=your_api_key_here
```

Also make sure `.env` is included in `.gitignore`.

---

# 🚀 Future Improvements

Possible future improvements include:

* Adding a Streamlit interface
* Adding conversation memory
* Supporting document-based question answering
* Adding Retrieval-Augmented Generation (RAG)
* Adding PDF and document processing
* Adding chat history
* Adding response export
* Adding multiple AI application modules
* Integrating additional AI capabilities
* Improving prompt management and evaluation

---

# 📁 Project Deliverables

The project includes:

* 📓 Google Colab Notebook
* 📝 Generative AI Learning Notes
* 🤖 Gemini API Experiments
* 💬 Interactive AI Chatbot
* 🧪 Prompt Engineering Experiments
* 🛡️ Responsible AI Analysis
* 🔍 Hallucination Awareness Experiment
* 📖 Project Documentation
* 📋 Requirements File

---

# 🏢 Internship Information

**Organisation:** Codomax Digital Solutions
**Internship:** Generative AI Internship
**Project:** Generative AI Foundations
**Project Number:** 1

This project was completed as part of my practical learning and development journey in Generative AI.

---

# 👨‍💻 Author

**Rahul Gupta**

B.Sc. (Hons) Computer Science

### Connect with me

🔗 LinkedIn: [https://www.linkedin.com/in/rg-rr2004/](https://www.linkedin.com/in/rg-rr2004/)

---

# 📜 License

This project is created for **educational and internship purposes**.

You are welcome to explore the code and concepts for learning purposes.