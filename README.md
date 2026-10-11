# Awesome open-source OpenWork alternatives

Kortix is open source, and it leads this curated list of open-source alternatives to OpenWork. Each entry gives you what it is, its license, how it self-hosts, and who it fits, so you can pick the one that matches your team.

> **Description:** Curated open-source alternatives to OpenWork, led by Kortix, the open-source AI Operating System.

OpenWork is a free, open-source desktop app for macOS, Windows, and Linux where AI agents work on your own files. It is built on OpenCode, works with 50+ model providers through your own API keys or local models, and is maintained by Different AI. Its desktop app and core platform are MIT, and its team control plane sits under a source-available license. Pick the shape that matches your team: a cloud platform with review built in, a self-hosted chat front end, or a local agent on your own machine.

Licenses and self-hosting details are as published by each project in October 2026. [Full OpenWork alternatives comparison](https://openworkalternative.com/openwork-alternatives).

## How to choose

| You want | Pick | Because |
| --- | --- | --- |
| Agents, skills and memory in one repo you own, run in the cloud | Kortix | Open source; one repo for agents, skills, memory and connectors |
| A free local desktop app for work on your own files | OpenWork | MIT desktop app; 50+ providers through your own keys |
| A self-hosted chat front end over your models and documents | Open WebUI | Docker or Kubernetes; plugins, RAG and multi-user |
| A control center for coding agents across backends | OpenHands | Runs agents locally, in Docker, on VMs or in the cloud |
| A private, local ChatGPT over your documents | AnythingLLM | Desktop and Docker; document chat and agents |
| A desktop multi-agent coworker, local-first | Eigent | Apache 2.0; parallel agents on your own machine |
| An always-on assistant in your messaging apps | OpenClaw | One Gateway; your hardware holds state and credentials |
| A self-improving agent on a server or VPS | Hermes | Built-in learning loop; seven terminal backends |

## The list

### 1. Kortix

Kortix is the open-source AI Operating System: your agents, their skills, your company memory, and every connector in one git repo you own, with the agents working on real cloud computers. [Kortix on GitHub](https://github.com/kortix-ai/suna)

- **What it is:** the leading open-source alternative to Claude Cowork and ChatGPT Work.
- **Where the work lives:** agents, skills, memory files, connectors and triggers are files in your repository, versioned and reviewed like code.
- **Where agents run:** one isolated sandbox per session, each on its own branch. Session work reaches `main` through a change request a person approves, and merge is default-deny for agents.
- **Models:** any model provider with your own keys. Or the ChatGPT plan you already pay for. Or sign in with your OpenCode Console account for OpenCode Zen and Go.
- **Connectors:** 3,000+ apps in a click, plus MCP, OpenAPI, Postman, GraphQL and raw HTTP. Connector credentials are brokered server-side and never enter the machine.
- **Channels:** Slack and Microsoft Teams are live. Email is experimental, per project.
- **Governance:** per-resource permissions for people and agents. Roles, groups, and an audit trail. SAML 2.0 single sign-on and SCIM 2.0. Approval gates you set, off until you set them.
- **Where it runs:** run it on Kortix Cloud, in your VPC, or on your own on-prem network. Self-host is free.
- **Scale:** thousands of agents in parallel on one config, each on its own cloud computer.
- **License:** Open source. Read it, fork it, audit it.
- **Fits:** teams that want the agents, skills and memory in one repo they own, with work landing through review, in the cloud, in Slack or Teams, and on a schedule. See [Kortix vs OpenWork](https://openworkalternative.com/openwork-vs-kortix) and [OpenWork for teams](https://openworkalternative.com/openwork-for-teams).

### 2. OpenWork

OpenWork is the incumbent desktop app. The free app runs AI agents on your own files, local-first, and the desktop is not required: an OpenWork MCP lets you use the same skills, plugins, MCP connections, Google Workspace and Microsoft 365 capabilities from Codex, Claude Code, Cursor or OpenCode.

- **What it is:** a desktop app for macOS, Windows and Linux where agents work on your files, built on OpenCode.
- **License:** everything outside `ee/` is MIT, covering the desktop app and core platform. Everything under `ee/` (OpenWork Den, the org control plane) is under the OpenWork EE License, a source-available license. Production use requires a subscription except for organizations of up to 5 users, a 30-day evaluation, and development or testing. Each `ee/` release converts to MIT two years after publication.
- **Self-hosting:** the desktop app runs locally and your files stay on your machine. The team control plane can be self-hosted on your own infrastructure.
- **Fits:** a person who wants a point-and-click desktop workspace on their own files, and teams that want to share skills and MCP servers. The managed cloud adds SSO and an extension marketplace.

### 3. Open WebUI

Open WebUI is a self-hosted AI platform and chat front end. It connects to Ollama and any OpenAI-compatible API, and extends through plugins, agents and retrieval over your documents.

- **What it is:** a user-friendly, provider-agnostic interface for local and cloud models, built to run offline.
- **License:** the Open WebUI License, a BSD-style license with a branding clause. You can use, modify and redistribute it, but you may not remove the Open WebUI branding unless you have under 50 end users in a rolling 30-day window, or a separate enterprise license.
- **Self-hosting:** install with pip or Docker, or on Kubernetes. Multi-user, with roles, groups and persistent memory.
- **Fits:** teams that want a self-hosted chat and RAG layer over their own models and documents.

### 4. OpenHands

OpenHands is a self-hosted developer control center for coding agents and automations. It runs the OpenHands agent and third-party agents such as Claude Code, Codex, Gemini, Pi and OpenCode across local, remote and cloud backends.

- **What it is:** a control center for starting conversations with coding agents and automating tasks like decomposing GitHub issues.
- **License:** MIT.
- **Self-hosting:** run it on your laptop, in Docker, on a VM, or on a server in the cloud. You can connect to OpenHands Cloud or OpenHands Enterprise if you choose to.
- **Fits:** engineering teams that want one place to run coding agents across several backends, with automations into Slack and GitHub.

### 5. AnythingLLM

AnythingLLM is an all-in-one AI application that builds a private ChatGPT over your documents, with agents and multi-user support out of the box.

- **What it is:** chat with your docs, with built-in agents, vector databases and document pipelines.
- **License:** MIT.
- **Self-hosting:** desktop app for macOS, Windows and Linux, or Docker. Runs locally by default with zero setup.
- **Fits:** teams that want a private, local assistant over their own documents, with per-user access.

### 6. Eigent

Eigent is the open-source Cowork desktop app. It runs a multi-agent workforce on your machine, local-first, and coordinates parallel agents on complex workflows.

- **What it is:** a desktop app for building and running a custom multi-agent workforce, built on CAMEL.
- **License:** Apache License 2.0.
- **Self-hosting:** local deployment with a local backend, local models through vLLM, Ollama or LM Studio, and no cloud account required.
- **Fits:** desktop users who want a local, multi-agent coworker that works with any model.

### 7. OpenClaw

OpenClaw is an open-source AI assistant that runs on your own computer and meets you in the messaging apps you already use.

- **What it is:** an always-on assistant, personal or shared, reachable in Discord, iMessage, Slack, Teams, Telegram, WhatsApp and more.
- **License:** MIT.
- **Self-hosting:** one Gateway runs on your hardware. State, memory and credentials live on your machine. Tools run on the host unless you configure sandboxing.
- **Fits:** people who want an assistant in their chat apps that keeps state and credentials on hardware they control. OpenClaw is stewarded by the OpenClaw Foundation.

### 8. Hermes

Hermes is a self-improving AI agent built by Nous Research. It creates skills from experience, improves them during use, and keeps memory across sessions.

- **What it is:** an agent with a built-in learning loop, reachable from Telegram, Discord, Slack, WhatsApp, Signal and the CLI.
- **License:** MIT.
- **Self-hosting:** seven terminal backends, including local, Docker, SSH, Modal, Daytona and Vercel Sandbox. Runs on a small VPS or a GPU cluster.
- **Fits:** people who want a single self-improving agent on a server, with scheduled automations and parallel subagents.

## Read the guides

Four short guides go with this list:

- [What is OpenWork?](docs/what-is-openwork.md) defines the desktop app, the cloud and the org control plane, and where Kortix differs.
- [Kortix vs OpenWork](docs/kortix-vs-openwork.md) compares them on configuration, execution, models, governance and license.
- [Self-hosting](docs/self-hosting.md) covers what each option installs and the single-command Kortix path.
- [FAQ](docs/faq.md) answers the questions that come up when moving off OpenWork.

More on the OpenWork alternatives site: [openworkalternative.com](https://openworkalternative.com/), [the self-hosting guide](https://openworkalternative.com/self-hosting), [OpenWork for teams](https://openworkalternative.com/openwork-for-teams), and the [OpenWork alternatives FAQ](https://openworkalternative.com/faq).

## Get started

Self-host Kortix for free, or use the managed cloud. **[Get started with Kortix](https://kortix.com)**.

## Contributing

Corrections are welcome. Open an issue or a pull request with a source for the change.
