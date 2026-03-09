<p align="center">
  <img src="https://raw.githubusercontent.com/dojops/dojops/main/packages/api/public/icons/official-dojops-icon.png" alt="DojOps" width="120" />
</p>

<h1 align="center">DojOps</h1>

<p align="center">
  <strong>Enterprise-grade AI DevOps Automation Engine</strong><br />
  Generate, validate, and execute infrastructure &amp; CI/CD configurations safely — with structured output enforcement, sandboxed execution, approval workflows, and hash-chained audit trails.
</p>

<p align="center">
  <a href="https://dojops.ai">Website</a> &nbsp;&middot;&nbsp;
  <a href="https://docs.dojops.ai">Documentation</a> &nbsp;&middot;&nbsp;
  <a href="https://hub.dojops.ai">Tool Marketplace</a> &nbsp;&middot;&nbsp;
  <a href="https://github.com/dojops/dojops">Get Started</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.3-00e5ff?style=flat-square" alt="Version" />
  <img src="https://img.shields.io/badge/node-%3E%3D20-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node" />
  <img src="https://img.shields.io/badge/typescript-5.4+-3178c6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" alt="License" />
</p>

---

## What is DojOps?

DojOps is an AI-powered DevOps automation engine that turns natural language into production-ready infrastructure configurations. It supports 13 DevOps tools, 6 LLM providers, 16 specialist agents, 10 security scanners, and a full REST API with a web dashboard — all with structured output enforcement, sandboxed execution, and approval workflows.

```bash
# Install
npm i -g @dojops/cli

# Generate a GitHub Actions CI pipeline
dojops "Create a CI pipeline for a Node.js app with tests and Docker build"

# Plan + execute with approval
dojops --execute "Set up Terraform for AWS S3 with versioning"
```

## Highlights

| | |
|---|---|
| **13 DevOps Tools** | GitHub Actions, Terraform, Kubernetes, Helm, Ansible, Docker Compose, Dockerfile, Nginx, Makefile, GitLab CI, Prometheus, Systemd, Jenkinsfile |
| **6 LLM Providers** | OpenAI, Anthropic, Ollama, DeepSeek, Google Gemini, GitHub Copilot |
| **16 Specialist Agents** | Intelligent routing to domain-specific agents + custom agent support |
| **10 Security Scanners** | npm-audit, pip-audit, Trivy, Gitleaks, Checkov, Hadolint, ShellCheck, Trivy SBOM, Trivy License, Semgrep |
| **20 API Endpoints** | REST API + web dashboard for team integration |
| **Sandboxed Execution** | Policy engine, approval workflows, write allowlists, audit trails |
| **Tool Marketplace** | Publish, discover, and install community tools via [DojOps Hub](https://hub.dojops.ai) |
| **No Telemetry** | Zero data leaves your machine except to your configured LLM provider |

## Repositories

| Repository | Description |
|---|---|
| [`dojops`](https://github.com/dojops/dojops) | Core monorepo — CLI, API, all `@dojops/*` packages |
| [`dojops-doc`](https://github.com/dojops/dojops-doc) | Documentation site (Next.js + Nextra) |
| [`dojops-hub`](https://github.com/dojops/dojops-hub) | Tool marketplace (Next.js + PostgreSQL + Prisma) |
| [`dojops.ai`](https://github.com/dojops/dojops.ai) | Marketing website |
| [`homebrew-tap`](https://github.com/dojops/homebrew-tap) | Homebrew formula for macOS/Linux |

## Install

```bash
# npm (recommended)
npm i -g @dojops/cli

# Shell script
curl -fsSL https://raw.githubusercontent.com/dojops/dojops/main/install.sh | sh

# Docker
docker run --rm -it ghcr.io/dojops/dojops "your prompt"

# Homebrew
brew tap dojops/tap && brew install dojops
```

## Contributing

We welcome contributions across all repositories. Each repo includes a `CONTRIBUTING.md` with setup instructions and guidelines. Check the issues in any repo to find something to work on.

## License

All DojOps repositories are licensed under the [MIT License](https://github.com/dojops/dojops/blob/main/LICENSE).
