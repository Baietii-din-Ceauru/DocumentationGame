# DocumentationGame

This repository stores all documentation for the game project. It uses a **[Hugo](https://gohugo.io/)** static site generator and follows a strict branching and deployment flow.

## 📄 Official Documentation

- **Production Docs**: [https://documentation.baietiidinceauru.top](https://documentation.baietiidinceauru.top)
- **Staging Docs**: [https://staging.documentation.baietiidinceauru.top](https://staging.documentation.baietiidinceauru.top)

---

## 📌 Contribution Guidelines

### 🚧 Branching Workflow

- All changes **must originate from a feature branch** (naming convention TBD).
- Your feature branch should be based off of `staging`, **not** `main`.
- Once your feature is complete:
  1. Run the Hugo server locally to preview.
  2. Submit a PR **into `staging`**.
  3. Once approved, your changes will be deployed to the staging docs.
  4. Only maintainers may merge `staging` into `main`.

> 🔒 PRs directly into `main` are **not allowed** and will be blocked by policy or automation.

---

## 🛠️ Running Hugo Locally

### 1. Install Hugo

Follow the official installation guide for your platform:
➡️ [https://gohugo.io/getting-started/installing/](https://gohugo.io/getting-started/installing/)

For Homebrew (macOS):
```bash
brew install hugo
```

On Windows (scoop):

```powershell
scoop install hugo
```
2. Start Local Server
Once inside your Hugo documentation folder:

```bash
hugo server -D
```

-D includes drafts in your local preview.

Then open http://localhost:1313 to preview.

🧪 Testing Before You Push
Always preview your documentation locally.

Push to a feature branch and create a PR into staging.

Only once staging docs are verified, a maintainer will promote changes to main.