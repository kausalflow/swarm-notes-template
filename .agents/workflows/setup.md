---
description: Run this workflow to help the user set up and configure the Swarm Notes Template.
---

When the user executes this workflow, follow these steps sequentially:

1. **Ask for basic info**: Ask the user for their GitHub username, the repository name, and a few research topics or keywords they want to track. Stop and wait for their response.
2. **Update `configs/site.json`**:
   - Set `site` to `https://<username>.github.io`
   - Set `base` to `/<repo-name>/`
   - Set `github_url` to `https://github.com/<username>/<repo-name>`
3. **Update `configs/config.ts.yaml`**: Replace the `keywords` list with the research topics they provided.
4. **Enable Tracker**: Open `.github/workflows/autonomous-tracker.yml` and uncomment the cron schedule `cron: "0 5 * * *"`.
5. **Final Guidance**: Give them a short message reminding them to enable GitHub Pages (Actions source) and add their LLM API keys to GitHub Secrets.
