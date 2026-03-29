# Swarm Notes Template

An automated AI research assistant and knowledge base template. It autonomously searches for new research papers, analyzes them using LLMs, saves the results into a markdown vault, and publishes a beautiful static website so you can intuitively browse your curated research.

## 🚀 How It Works

1. **Autonomous Tracker:** A GitHub Actions cron job runs daily (or manually), queries scholarly APIs (OpenAlex, Semantic Scholar, or arXiv), and uses AI agents to summarize papers and extract core concepts.
2. **Markdown Vault:** The curated notes are autonomously formatted and saved as structured Markdown files within the `vault/` directory of your repository.
3. **Static Website:** Another GitHub Action continuously builds and deploys the `swarm-notes-ui` (an Astro frontend) reading directly from your `vault/` directory and securely pushing it to GitHub Pages.

---

## 🛠️ Quick Start

### 1. Bootstrapping Your Repository
Click the green **Use this template** button at the top of this repository on GitHub to create your own copy.

### 2. Enable GitHub Pages
1. Navigate to your repository **Settings > Pages**.
2. Under "Build and deployment", change **Source** to **GitHub Actions**. *(This allows Astro to build your site without requiring a specific `gh-pages` branch).*

### 3. Add AI API Keys
The automated tracker needs an LLM to read and analyze the research papers.
Go to your repository **Settings > Secrets and variables > Actions** and click **New repository secret**.
Add your preferred key, for example:
- `GOOGLE_API_KEY` *(Default config uses Google Gemini via `google-gla:gemini-flash-lite-latest`)*
- `OPENAI_API_KEY`

Depending on the service you prefer, you just need one. The service is configured in `configs/[your-config].yaml`.

### 4. Configure Your Deployment Settings
Edit the `configs/site.json` file inside your repository to configure your site's deployment URL so internal links and headers correctly resolve:
```json
{
  "site": "https://yourusername.github.io",
  "base": "/your-repo-name/",
  "trailingSlash": "always",
  "github_url": "https://github.com/yourusername/your-repo-name"
}
```
*(Note: If you are deploying this to a custom top-level domain, set `"base"` to `"/"`)*

### 5. Configure Your Topics
Look inside `configs/config.ts.yaml` to configure what the AI swarm tracks:
- Modify `paper_search.keywords` for your specific research queries (e.g., `"trajectory prediction"`, `"large language models"`).
- Modify `llm_model` to point to a valid LiteLLM proxy string if you are not using Gemini. 

### 6. Run the Tracker Workflow!
1. Go to the **Actions** tab in GitHub.
2. Select **Autonomous Research Tracker** on the left.
3. Click **Run workflow** (you can leave the default config file path as `configs/config.ts.yaml`).
4. Wait for it to finish! The bot will automatically commit new markdown files into your `vault/` folder.
5. The **Deploy Astro site to Pages** action will trigger automatically once the tracker is done, publishing your live knowledge base! 🎉

### 7. Schedule the Tracker

1. In `.github/workflows/autonomous-tracker.yml`, uncomment the line `# - cron: "0 5 * * *"`.
2. Commit and push the changes.


---

## 📝 Manual Usage (Without the Swarm)

You don't *have* to use the autonomous agent tracker! The `swarm-notes-ui` uses a robust static site generator that gracefully turns any Markdown in your `vault/` folder into a fully searchable site.

You can manually add standard Obsidian-style markdown notes or markdown files with frontmatter inside the `vault/` directory.

### Running the Website Locally
If you want to view or tinker with the website locally:

```bash
# Navigate to the frontend directory
cd swarm-notes-ui

# Install dependencies (Node.js 22+ recommended)
npm install

# Start the Astro dev server
npm run dev
```

Then visit `http://localhost:4321` to view your knowledge base!
