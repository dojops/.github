<p align="center">
  <img src="https://raw.githubusercontent.com/dojops/dojops/main/packages/api/public/icons/official-dojops-icon.png" alt="DojOps" width="120" />
</p>

<h1 align="center">DojOps</h1>

<p align="center">
  <strong>AI automation engine</strong><br />
  Describe what you want in plain English. DojOps generates the config, validates it against a schema, and writes it to disk only after you approve.
</p>

<p align="center">
  <a href="https://dojops.ai">Website</a> &nbsp;&middot;&nbsp;
  <a href="https://doc.dojops.ai">Docs</a> &nbsp;&middot;&nbsp;
  <a href="https://hub.dojops.ai">Skill marketplace</a> &nbsp;&middot;&nbsp;
  <a href="https://github.com/dojops/dojops">Get started</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-2.0.0-00e5ff?style=flat-square" alt="Version" />
  <img src="https://img.shields.io/badge/node-%3E%3D20-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node" />
  <img src="https://img.shields.io/badge/typescript-5.4+-3178c6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" alt="License" />
</p>

---

## What does it do?

You give DojOps a prompt. It picks the right specialist agent, generates config files (Terraform, Kubernetes, GitHub Actions, Dockerfiles, etc.), validates them against Zod schemas, and writes them only after you approve. Every operation is logged in a hash-chained audit trail.

```bash
npm i -g @dojops/cli

# Generate a GitHub Actions CI pipeline
dojops "Create a CI pipeline for a Node.js app with tests and Docker build"

# Plan multiple files, review, then apply
dojops --execute "Set up Terraform for AWS S3 with versioning"
```

## What's included

| | |
|---|---|
| 35 built-in skills | GitHub Actions, Terraform, Kubernetes, Helm, Ansible, Docker Compose, Dockerfile, Nginx, Makefile, GitLab CI, Prometheus, Systemd, Jenkinsfile, Pulumi, ArgoCD, CloudFormation, Grafana, OTel Collector, Packer, and more |
| 53 skills total | 35 built-in + community skills across CI/CD, containers, monitoring, and security |
| 7 LLM providers | OpenAI, Anthropic, Ollama, DeepSeek, Mistral, Google Gemini, GitHub Copilot |
| 32 specialist agents | Keyword-based routing to the right agent for each prompt, plus custom agents |
| 10 security scanners | npm-audit, pip-audit, Trivy, Gitleaks, Checkov, Hadolint, ShellCheck, Trivy SBOM, Trivy License, Semgrep |
| REST API + dashboard | 20+ endpoints, web UI for teams |
| Sandboxed execution | Policy engine, approval workflows, write allowlists, audit trails |
| Skill marketplace | Publish and install community skills via [DojOps Hub](https://hub.dojops.ai) |
| No telemetry | Nothing leaves your machine except requests to your configured LLM provider |

## Repositories

| Repository | What's in it |
|---|---|
| [`dojops`](https://github.com/dojops/dojops) | Main monorepo. CLI, API server, all `@dojops/*` packages |
| [`dojops-dops-skills`](https://github.com/dojops/dojops-dops-skills) | All `.dops` skill files, organized by category |
| [`dojops-connectors`](https://github.com/dojops/dojops-connectors) | Connector SDK + GitHub, GitLab, Jira implementations |
| [`dojops-doc`](https://github.com/dojops/dojops-doc) | Documentation site (Next.js + Nextra) |
| [`dojops-hub`](https://github.com/dojops/dojops-hub) | Skill marketplace (Next.js + PostgreSQL + Prisma) |
| [`dojops.ai`](https://github.com/dojops/dojops.ai) | Marketing website |
| [`homebrew-tap`](https://github.com/dojops/homebrew-tap) | Homebrew formula for macOS and Linux |

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

Every repo has a `CONTRIBUTING.md` with setup instructions. Check the issues in any repo to find something to pick up.

## License

MIT. See [LICENSE](https://github.com/dojops/dojops/blob/main/LICENSE).
