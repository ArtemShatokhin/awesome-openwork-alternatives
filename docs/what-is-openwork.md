# What is OpenWork?

Kortix is the open-source AI Operating System, and OpenWork is the project people most often put next to it. Defining OpenWork precisely matters because the name covers a desktop app, a managed cloud, and an organization control plane, and each part has a different shape.

OpenWork is a free, open-source desktop application for macOS, Windows, and Linux where AI agents do work on your own files. [OpenWork on GitHub](https://github.com/different-ai/openwork) describes it as the open-source alternative to Claude Cowork and Codex, built on OpenCode, working with any model: 50+ providers, your own API keys, or local models through Ollama. It is maintained by Different AI.

Three parts make up OpenWork:

- The desktop app, where a person runs agents against a folder on their machine. Your files stay local and the cloud is optional.
- OpenWork Cloud, a managed option for teams. The [OpenWork site](https://openworklabs.com) says the Team plan includes the first 5 seats, then $10 per seat per month, and adds SSO, API access and an extension marketplace. Enterprise adds SCIM, desktop policies and bring-your-own inference.
- OpenWork Den, the organization control plane. It publishes skills and plugins through marketplaces, assigns them to a team or specific people, and controls which models and app versions a team can use.

## The license, in two parts

The repository uses a directory-split license, which the project compares to GitLab's. Everything outside `ee/` is MIT, covering the desktop app and the core platform, free for any use. Everything under `ee/`, which is OpenWork Den, is under the OpenWork EE License, a source-available license: the code is public, and production use requires a subscription except for organizations of up to 5 users, a 30-day evaluation at any size, and development or testing. Each `ee/` release converts to MIT two years after publication.

## Where OpenWork fits

OpenWork fits a person who wants a point-and-click desktop workspace and does not want to touch a terminal, and it fits a team that wants to share skills and MCP servers without each person rebuilding their setup. The desktop app is the free path. The team features live in OpenWork Den and in the managed cloud.

## How Kortix differs

Where OpenWork installs on each desktop, Kortix runs from one git repository. Agents, skills, company memory, and connectors are files in that repository, versioned and reviewed like code. Each session runs on its own cloud computer, an isolated sandbox on its own branch, and session work reaches `main` through a change request a person approves. Kortix runs on Kortix Cloud, in your VPC, or on your own on-prem network, and self-host is free.

Both are open source and both work with your own model keys. OpenWork keeps the work on your machine; Kortix runs the agents on cloud computers and keeps the whole company in one repo you own. The [Kortix vs OpenWork](kortix-vs-openwork.md) guide compares them across configuration, execution, models, governance and license.
