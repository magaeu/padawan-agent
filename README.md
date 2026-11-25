# padawan-agent

A personal profile-card project built using agentic engineering during Agentics 101.

## What It Is?

**padawan-agent** is a responsive HTML profile card that presents a frontend developer's identity, profession, contact details, and professional keywords. The repository contains a semantic, accessible implementation built with HTML, CSS, and inline SVG, with no external runtime dependencies.

## What This Demonstrates

- **Specification writing:** Converting requirements into precise instructions
- **AI supervision:** Directing GitHub Copilot to generate code from specifications
- **Human-in-the-loop review:** Maintaining quality through verification
- **Safety protocols:** Operating AI within bounded parameters
- **Professional documentation:** Creating maintainable projects
- **Accessible frontend development:** Building semantic, responsive HTML with inline SVG

## The Workflow

Specification → Agent Generation → Human Review → Production

1. Write detailed requirements in `specs/`.
2. GitHub Copilot generates code matching the specifications.
3. A human verifies the output for accuracy and quality.
4. Approved code is committed and deployed.

## Built With

**Development Tools**

- **Markup:** HTML5
- **Styling:** CSS
- **Graphics:** Inline SVG
- **AI Agent:** GitHub Copilot
- **Version Control:** Git
- **Deployment:** GitHub Pages

**Approach**

- **Method:** Specification-driven development
- **Human Role:** Supervisor, reviewer, and quality control
- **Agent Role:** Code generation and implementation
- **Safety Model:** Human-in-the-loop review

## Repository Structure

```text
padawan-agent/
├── .devcontainer/
│   └── devcontainer.json   # Development container configuration
├── .github/
│   └── dependabot.yml      # Dependency update configuration
├── specs/
│   ├── card-spec.md        # Profile card specification
│   └── readme-spec.md      # README specification
└── src/
│   └── index.html          # Responsive profile card implementation
├── README.md               # Document the project and its setup
└── SAFETY.md               # Agent's approved and prohibited actions
```

## Quick Start

1. Download or clone the repository:

   ```bash
   git clone git@github.com:magaeu/padawan-agent.git
   cd padawan-agent
   ```

2. Start a local static server:

   ```bash
   python3 -m http.server 8000
   ```

3. Open `http://localhost:8000/src/index.html` in a browser.

## Key Learnings

- Precise specifications reduce AI ambiguity.
- Directive feedback produces more accurate results than vague requests.
- Manual review builds practical error-detection skills.
- Safety protocols keep AI-assisted changes within a controlled scope.

## Safety Features

- Human approval is required for all changes.
- Agent scope is bounded to specific folders.
- Git history provides rollback capability.
- Safety procedures are documented in `SAFETY.md`.

## Live Demo

[View the live demo](https://magaeu.github.io/padawan-agent/src/)


**Course:** Agentics 101 | Bradley Ross, Nicholas Ruest, The Agentics Foundation

<p align="center">Made with ❤</p>