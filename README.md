# Dynamic Developer Portfolio Dashboard

A modern, responsive frontend single-page portfolio interface that connects directly to the live GitHub REST API to showcase verified public repositories. 

## 📂 Project Architecture

```text
github-portfolio/
├── .github/          # GitHub configuration and automation workflows
├── index.html        # Main dashboard interface, theme, and API logic
└── README.md         # Project portfolio documentation (This file)
```

## ✨ Key Features

- **Automated API Data Streaming:** Dynamically pulls live GitHub profile pictures, biographies, location status, and follower metrics.
- **Strict Quality Validation Gates:** Evaluates root directories asynchronously to **only display public projects that completely contain a `README`, a `LICENSE`, and a `.gitignore` file**.
- **Real-Time Client-Side Filtering:** Includes a live text-matching filter field to instantly narrow down visible repository cards by language or name.
- **Session Cache Optimization:** Implements a runtime `sessionStorage` credential gateway prompt to accept a local Personal Access Token to safely bypass unauthenticated browser rate limits.

## 🚀 Live Deployment Instructions

This portfolio is fully optimized for free static hosting using **GitHub Pages**:

1. Create a public repository on GitHub named exactly `portfolio` or `github-portfolio`.
2. Commit and push your local files (`index.html`, `.github/`, and `README.md`) to the `main` branch.
3. On your GitHub repository dashboard, navigate to **Settings ⚙️** -> **Pages** (under the "Code and automation" menu tab).
4. Change the deployment source dropdown to **Deploy from a branch**.
5. Set the Target Branch to **`main`**, leave the folder directory as **`/ (root)`**, and click **Save**.
6. Wait 60 seconds for the backend environment build pipeline to finish compiling. Your link will generate right at the top of the Page Settings menu screen!
