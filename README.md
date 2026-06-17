# weather-assistant

> **Fully vibe coded** during the [5-Day AI Agents: Intensive Vibe Coding Course With Google](https://rsvp.withgoogle.com/events/google-x-kaggle-5-day-genai).
> No hand-written logic was harmed in the making of this project.

A simple ReAct agent for weather queries, scaffolded with `agents-cli` version `0.5.0`.

---

## Project Structure

```
weather-assistant/
├── app/                       # Core agent code
│   ├── agent.py               # Main agent logic
│   └── app_utils/             # App utilities and helpers
├── tests/                     # Unit, integration, and load tests
├── GEMINI.md                  # AI-assisted development guide
└── pyproject.toml             # Project dependencies
```

---

## Requirements

Before you begin, ensure you have:

- **uv** — Python package manager used for all dependency management. [Install](https://docs.astral.sh/uv/getting-started/installation/) · [Add packages](https://docs.astral.sh/uv/concepts/dependencies/) with `uv add <package>`
- **agents-cli** — Install with `uv tool install google-agents-cli`
- **Google Cloud SDK** — For GCP services. [Install](https://cloud.google.com/sdk/docs/install)

---

## Getting Started

Install `agents-cli` and its skills if not already installed:

```bash
uvx google-agents-cli setup
```

Install required packages:

```bash
agents-cli install
```

Test the agent with a local web server:

```bash
agents-cli playground
```

You can also use features from the [ADK](https://adk.dev/) CLI with `uv run adk`.

---

## Commands

| Command | Description |
|---|---|
| `agents-cli install` | Install dependencies using uv |
| `agents-cli playground` | Launch local development environment |
| `agents-cli lint` | Run code quality checks |
| `agents-cli eval` | Evaluate agent behavior (see `agents-cli eval --help`) |
| `uv run pytest tests/unit tests/integration` | Run unit and integration tests |

---

## Project Management

| Command | Description |
|---|---|
| `agents-cli scaffold enhance` | Add CI/CD pipelines and Terraform infrastructure |
| `agents-cli infra cicd` | One-command setup of entire CI/CD pipeline + infrastructure |
| `agents-cli scaffold upgrade` | Auto-upgrade to latest version while preserving customizations |

---

## Development

Edit your agent logic in `app/agent.py` and test with `agents-cli playground` — it auto-reloads on save.

---

## Deployment

```bash
gcloud config set project <your-project-id>
agents-cli deploy
```

To add CI/CD and Terraform, run `agents-cli scaffold enhance`.
To set up production infrastructure, run `agents-cli infra cicd`.

---

## Observability

Built-in telemetry exports to Cloud Trace, BigQuery, and Cloud Logging.

---

## Vibe Coded With

This project was built entirely through AI-assisted vibe coding as part of Google's 5-Day AI Agents Intensive. The agent logic, tooling setup, and project structure were all generated and iterated through natural language prompts — zero boilerplate written by hand.

---

## License

MIT — do whatever you want with it.
