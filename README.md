# AI Text Summarizer — Technical Interview
**Goal:** Finish a simple web app that summarizes a paragraph using Ollama.

Most of the project is already provided. Complete **only TODO 0–5** in `app.py` and `frontend/app.js`.

## Project structure

```text
AI-Summarizer-Interview/
├── app.py
├── requirements.txt
├── run.bat
└── frontend/
    ├── index.html
    ├── style.css
    └── app.js
```

## Setup before the interview

Install [Ollama](https://ollama.com/) and download the model:

```bash
ollama pull llama3.2:3b
```

Create a virtual environment (optional but recommended):

```bash
python -m venv .venv
```

On Windows Command Prompt:

```cmd
.venv\Scripts\activate.bat
```

On Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

Run the app:

```bash
python app.py
```

Or double-click `run.bat` on Windows. Open <http://127.0.0.1:8000>.

> Make sure Ollama is running. On some installations you may need to start it with `ollama serve` in a separate terminal.

## Candidate Tasks

Complete the missing sections marked **TODO** in the project.

1. **TODO 0 — Model Initialization:** Initialize and configure the Ollama language model using `llama3.2:3b` with a temperature of `0`.

2. **TODO 1 — Prompt Engineering:** Create a prompt that instructs the AI to summarize the user's text in 1–2 sentences.

3. **TODO 2 — LLM Integration:** Send the prompt to the language model and retrieve the generated response.

4. **TODO 3 — FastAPI:** Return the generated summary to the frontend through the API.

5. **TODO 4 — JavaScript Request:** Implement the communication between the frontend and the backend to send the user's text.

6. **TODO 5 — Display Results:** Process the API response and display the generated summary on the webpage.
## Example input

> Python is a programming language used for web development, data science, automation, and artificial intelligence. It is popular because it is easy to learn and has many useful libraries.

## Expected behavior

After clicking **Summarize**, a short summary appears under the button. The precise words will vary depending on the model.

