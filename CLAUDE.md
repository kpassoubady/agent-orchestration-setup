# Agent Orchestration Setup

Standalone, student-facing pre-class setup repository for **Orchestration Fundamentals for Agentic Development**.

## Tech Stack

- **Version Control:** Git
- **Language/Runtime:** Python 3, Node.js
- **Agent:** Claude Code

## Project Structure

```
catalog/               Course outline and syllabus
install/               Installation guides for macOS and Windows
quickstart-project/    Verification script to confirm tooling is installed
llm-context/           Working context, notes, and generated reports for LLM agents
Welcome.md             Entry point message sent to students before class
```

## Key Commands

```bash
# Verify the setup environment
cd quickstart-project
python3 verify_setup.py
```

## Conventions

- **Standalone Setup Rule:** Student-facing content must not link to or name the primary, companion, book, or book-companion repositories.
- Use absolute GitHub URLs (`https://github.com/kpassoubady/agent-orchestration-setup/blob/main/...`) for all links in `Welcome.md`.
- Keep setup instructions platform-aware and safe to run before class.
