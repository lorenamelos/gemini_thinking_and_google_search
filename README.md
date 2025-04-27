# Exploring Gemini Thinking with Structured Prompts and Google Search

This Python script demonstrates how to use Google's Gemini AI models (like Gemini 1.5 Flash) to generate structured content about a specific subject. It utilizes a detailed prompt template **based on techniques recommended by Google for guiding the AI's thinking process (see [Google AI Thinking Prompt Guide](https://ai.google.dev/gemini-api/docs/thinking#prompt-guide)) and leverages the Google Search tool to enable the AI to perform research and present information in a predefined format.

## Purpose

The goal of this script is to provide a clear example of:

1.  **Structured Prompting:** Creating detailed instructions for the AI to follow, ensuring consistent output format. This script specifically uses a prompt structure that encourages the AI to perform internal "thinking" steps (like research and analysis) before generating the final output, aligning with best practices outlined in the  [Google AI Thinking Prompt Guide](https://ai.google.dev/gemini-api/docs/thinking#prompt-guide).
2.  **AI-Powered Research:** Enabling the AI to use external tools (Google Search) to gather current information.
3.  **Content Generation:** Automatically creating summaries, lists, or other structured text based on the prompt and research.

This is particularly useful for tasks like generating educational summaries, comparing entities, or extracting key information in a standardized way.

## Features

*   **Structured Output:** Generates content following a specific template defined in the prompt.
*   **Research Capability:** Uses the integrated Google Search tool to find relevant, up-to-date information.
*   **Customizable Subject:** Easily change the `subject` variable to generate content on different topics.
*   **Clear Prompting Strategy:** Demonstrates how to guide the AI's analysis and presentation process within the prompt itself (e.g., asking for research steps).
*   **Model Flexibility:** Can be adapted to use different Gemini models (e.g., `gemini-1.5-flash`, `gemini-1.5-pro`).

## Prerequisites

*   **Python 3.x:** Ensure you have Python installed.
*   **Google Colab acess or Jupyter Notebook installed.
*   **Google Gemini API Key:**
    *   You need an API key from Google AI Studio or Google Cloud. Get one here: [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)
    *   **Crucially**, set this key as an environment variable named `GEMINI_API_KEY`.
        *   **Linux/macOS:** `export GEMINI_API_KEY="YOUR_API_KEY"`
        *   **Windows (Command Prompt):** `set GEMINI_API_KEY=YOUR_API_KEY`
        *   **Windows (PowerShell):** `$env:GEMINI_API_KEY="YOUR_API_KEY"`
        *   Alternatively, you can manage this through system settings or `.env` files (using libraries like `python-dotenv`).

## Customization

*   **Change the Subject:** Modify the `subject` variable for different topics.
*   **Edit the Prompt:** Adjust the `prompt_template` to change the output structure, request different information, or alter the AI's persona.
*   **Select a Different Model:** Change the `model_name` in `genai.GenerativeModel()` to use other Gemini models like `gemini-1.5-pro` (check availability and pricing).


