# AI-Ensemble Web (Layer 2)

This repository implements the **role-aware web interface** for AI-Ensemble.

## Purpose

The web app provides a **three-pane role-playing learning interface** that connects users to a single AI reasoning engine through distinct roles:

- **Scenario** — drives the learning narrative and decision points
- **Expert** — provides technical support (statistics, genetics, coding)
- **Manager** — provides strategic and process guidance

All roles interact with the same backend AI engine, but each request is explicitly tagged with a role to enforce knowledge separation and response framing.

## Architecture

- Framework: Django
- App: `game`
- UI: Single page with three independent chat panels
- Backend: External FastAPI service
- Backend endpoint:
