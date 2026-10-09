# URL Summarizer CLI (Groq)

A Python command-line tool that extracts readable text from a webpage and summarizes it using the Groq API.

> Note: If your internship task specifically requires the OpenAI API, this Groq version does not meet that particular requirement. Confirm with your mentor before submitting.

## Files

- `main.py` — fetches webpage text and requests a summary from Groq
- `requirements.txt` — Python dependencies
- `.gitignore` — excludes local environment files and secrets

## Setup (macOS/Linux)

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

## Configure the API key

```bash
export GROQ_API_KEY="YOUR_GROQ_API_KEY"
```

Never put your API key directly in source code or commit it to GitHub.

## Run

```bash
python main.py https://example.com
```

Optional model override:

```bash
python main.py https://example.com --model llama-3.1-8b-instant
```

## Example output

```text
Fetching webpage and generating summary...

SUMMARY
-------
Example Domain is a sample webpage used for examples and documentation.
- It provides a simple page for testing links and browser behavior.
```

The example output is illustrative. Actual output depends on the webpage and the API response.
