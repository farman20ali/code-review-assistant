# CodeSense — AI Code Review Assistant

## Overview & Approach (Summary)
CodeSense is a serverless AI Code Review Assistant built using HTML, CSS, and Vanilla JavaScript. It provides developers with instant, actionable feedback on code readability, structure, and maintainability. By running entirely client-side, it minimizes deployment overhead and ensures rapid interactions. The application dynamically routes prompts to major LLM providers (Groq, xAI, OpenAI, Gemini, Anthropic) based on user selection, enforcing strict structured JSON responses. This approach guarantees consistent outputs: exactly three improvements and one positive note. CodeSense prioritizes low latency and a sleek, developer-friendly interface, making it an ideal lightweight tool for immediate code analysis without complex backend infrastructure.

## Prerequisites 
To test this prototype locally, you will need to provide your own API key for the model you want to try:
* **Groq:** Get a free API Key at [console.groq.com](https://console.groq.com/) *(Recommended for fastest reviews)*
* **xAI (Grok):** Grab an API Key at [console.x.ai](https://console.x.ai/)
* **Google Gemini:** Get a free API key at [aistudio.google.com](https://aistudio.google.com/)
* **OpenAI:** Grab an API Key at [platform.openai.com](https://platform.openai.com/)
* **Anthropic:** Grab an API Key at [console.anthropic.com](https://console.anthropic.com/)

## How to Run
1. Clone this repository or download the folder.
2. Open `index.html` directly in any modern web browser.
3. Select your preferred provider from the dropdown.
4. Paste the respective API key in the input field.
5. (Optional) Click **"Fetch models"** to load the latest available models for that provider.
6. Choose a model from **model_list://** or type a custom one in **model://**.
7. Input your code snippet and click **"Review Code"**.

## Deployment & Publishing
This project is completely static (just an `index.html` file) and can be deployed anywhere instantly and for free.

### Option 1: GitHub Pages (Recommended)
1. Initialize a git repository: `git init`
2. Add files and commit: `git add . && git commit -m "Initial commit"`
3. Create a new repository on GitHub and push your code:
   `git remote add origin https://github.com/yourusername/your-repo-name.git`
   `git push -u origin main`
4. Go to your repository **Settings** > **Pages**.
5. Select the `main` branch as the source and click **Save**. Your site will be live in a few minutes!

### Option 2: Vercel or Netlify (Drag & Drop)
1. Go to [Vercel](https://vercel.com/) or [Netlify Drop](https://app.netlify.com/drop).
2. Simply drag and drop this project folder directly onto the dashboard.
3. It will instantly build and deploy the app, providing you with a public URL (e.g., `https://your-project.vercel.app`).
