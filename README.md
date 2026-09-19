# Prompt Basics

Two hands-on Colab notebooks teaching prompt engineering fundamentals to 2nd year Computer Science students. No prior AI/API experience needed.

## Notebooks

| Notebook | Covers | Open |
|---|---|---|
| [`promptBasic.ipynb`](promptBasic.ipynb) | Session 1: what a prompt is, being clear vs. vague, showing examples, "think step by step" | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/helloash-17/Prompt-Basics/blob/main/promptBasic.ipynb) |
| [`promptAdvanced.ipynb`](promptAdvanced.ipynb) | Session 2: chain-of-thought debugging, few-shot format control, role prompting, iterative refinement | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/helloash-17/Prompt-Basics/blob/main/promptAdvanced.ipynb) |

Do Session 1 first — Session 2 builds directly on it.

## Before you start

Both notebooks call [Groq](https://groq.com) (free, fast LLM API) using the `openai/gpt-oss-20b` model. You need a free API key:

1. Go to [console.groq.com/keys](https://console.groq.com/keys) and sign up / log in
2. Click **Create API Key** and copy it
3. In Colab, click the **🔑 key icon** on the left sidebar ("Secrets")
4. Click **Add new secret**, name it exactly `GROQ_API_KEY`, paste your key as the value, and turn on **Notebook access**

Then open a notebook using the badges above and run the cells top to bottom.

## Why Colab Secrets instead of typing the key in?

Earlier versions of these notebooks used a `getpass` prompt to type in the key each run. It works, but the input box occasionally freezes in Colab. Reading from Secrets is instant and only needs to be set up once per browser.
