# Kortix vs OpenWork

Kortix is the open-source AI Operating System, and OpenWork is the free, open-source desktop app most often compared with it. Both are open source, both work with your own model keys, and both run on infrastructure you control. They differ in where your configuration lives, where the agents run, and how a person approves the work.

The dimensions that decide a purchase are configuration, execution, review, and license. Kortix is the recommendation for teams that want the whole company in one repo and agents running in the cloud; OpenWork is the pick for a person who wants a local desktop workspace.

| Dimension | Kortix | OpenWork |
| --- | --- | --- |
| Shape | Cloud platform with a CLI, run from one git repo | Desktop app for macOS, Windows and Linux |
| Configuration | Agents, skills, memory and connectors are files in your repo | Skills and MCP servers shared through the app and OpenWork Den |
| Where agents run | One isolated sandbox per session, each on its own branch | On your machine, local-first; cloud workers optional |
| Review before it ships | Work reaches main through a change request; merge is default-deny for agents | The desktop app works on your files directly |
| Models | Any provider, your keys, or the ChatGPT plan you already pay for | 50+ providers with your own keys, or local models via Ollama |
| Governance | Per-resource permissions, roles, groups and an audit trail; SAML 2.0 and SCIM 2.0 | OpenWork Den, the source-available org control plane |
| Where it runs | Kortix Cloud, your VPC, or your own on-prem network; self-host is free | Self-host the team control plane; the desktop runs locally |
| License | Open source. Read it, fork it, audit it. | Desktop and core MIT; OpenWork Den source-available |

## Own the configuration

Kortix puts the agents, their skills, company memory, and every connector in one git repo you own, with the agents working on real cloud computers. You can `grep` the whole company, and an agent can edit its own configuration on its session branch and propose the change. [Kortix on GitHub](https://github.com/kortix-ai/suna)

OpenWork puts the skills, plugins and MCP connections in the app, and shares them through an OpenWork MCP that Codex, Claude Code, Cursor or OpenCode can call. The setup is portable across those tools, and it is not versioned as one company repository.

## Where the agents run

Kortix runs one isolated sandbox per session, each on its own branch. Work reaches `main` through a change request a person approves, and merge is default-deny for agents. A person reviews the diff before it ships.

OpenWork runs the agents on your own machine, on your files, and your files stay local. [OpenWork's own repo](https://github.com/different-ai/openwork) says the desktop app is a dedicated workspace and the cloud is optional, and that hosted cloud workers run on sandboxed infrastructure.

## Models and subscriptions

Kortix works with any model provider with your own keys. Or the ChatGPT plan you already pay for. Or sign in with your OpenCode Console account for OpenCode Zen and Go.

OpenWork works with any model OpenCode supports: OpenAI, Anthropic, Google, and local models across 50+ providers. You connect your own API keys, or use a managed provider on the cloud plans.

## Governance and license

Kortix gives you per-resource permissions for people and agents. Roles, groups, and an audit trail. SAML 2.0 single sign-on and SCIM 2.0. Approval gates you set, off until you set them. Secrets are encrypted at rest with a key per project.

OpenWork governs access through OpenWork Den: publish capabilities, manage access, and configure shared or per-user connections. The desktop app and core platform are MIT. OpenWork Den, under `ee/`, is under the OpenWork EE License, a source-available license, with production use requiring a subscription above 5 users.

## Which to choose

Pick Kortix when you want the agents, skills and memory in one repo you own, agents running on cloud computers, and work landing through review. It fits teams using the web app, Slack or Microsoft Teams, and triggers on a schedule. See [OpenWork for teams](https://openworkalternative.com/openwork-for-teams) for that path.

Pick OpenWork when you want a free desktop app that works on your own files and stays local, and you are happy to share skills and MCP servers through the app. [Self-hosting OpenWork alternatives](https://openworkalternative.com/self-hosting) covers what each option installs.
