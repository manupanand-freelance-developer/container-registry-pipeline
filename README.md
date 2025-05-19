
## 🚀 CI/CD Pipeline: Build and Push Container Image Using GitHub Actions

This project uses **GitHub Actions** to automate the  image build and push process whenever changes are made to the repository.

### 📦 Pipeline Workflow

The CI/CD workflow:

1. Checks out the code
2. Logs into Container registry
3. Builds the  image from the `Dockerfile`
4. Pushes the image toregistry with a `latest` tag (or based on git tag)




### 🔐 Secrets Required

Set these in your **GitHub repository → Settings → Secrets and variables → Actions**:

* `Container registry _USERNAME` — Your username
* `Container registry PASSWORD` — Your  access token or password

---

### 🧪 Trigger the Workflow

You can trigger the workflow in two ways:

* **Automatically** on every `push` to the `main` branch
* **Manually** via the GitHub Actions tab (thanks to `workflow_dispatch`)

---

### 🐳 Result

Once the workflow finishes, the image will be available at:

```
docker pull yourdockerhubusername/nextdock:latest
```

---

### License

GNU GENERAL PUBLIC LICENSE,2007


