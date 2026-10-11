# OpenWork alternatives FAQ

Kortix is the open-source AI Operating System, and these are the questions that come up when a person or a team decides to move off OpenWork.

## Is Kortix open source?

Yes. Kortix is open source: you can read it, fork it, and audit it. [Kortix on GitHub](https://github.com/kortix-ai/suna) holds the code, and self-hosting it is free.

## Is OpenWork open source?

OpenWork splits its license. Everything outside `ee/` is MIT, which covers the desktop app and the core platform. Everything under `ee/`, which is OpenWork Den, the org control plane, is under the OpenWork EE License, a source-available license. Production use of that part requires a subscription except for organizations of up to 5 users, a 30-day evaluation, and development or testing.

## What is the main difference between Kortix and OpenWork?

Kortix runs from one git repository and runs the agents on cloud computers. OpenWork is a desktop app that runs the agents on your own machine. In Kortix, agents, skills, company memory and connectors are files in the repo, each session gets an isolated sandbox on its own branch, and session work reaches `main` through a change request a person approves. The [Kortix vs OpenWork](kortix-vs-openwork.md) guide has the full comparison.

## Which models do they work with?

Kortix works with any model provider with your own keys. Or the ChatGPT plan you already pay for. Or sign in with your OpenCode Console account for OpenCode Zen and Go. OpenWork works with any model OpenCode supports, across 50+ providers, through your own API keys or local models via Ollama.

## Can I self-host both?

Kortix self-hosts with one command, `kortix self-host start`, which runs a single Docker Compose stack. OpenWork's desktop app runs locally with no server, and its team control plane can be self-hosted on your own infrastructure. The [self-hosting guide](self-hosting.md) covers both.

## How does work reach production?

In Kortix, session work reaches `main` through a change request a person approves, and merge is default-deny for agents. OpenWork's desktop app works on your files directly, so the review step is whatever your team adds around it.

## Does Kortix work in Slack and Microsoft Teams?

Slack and Microsoft Teams are live in Kortix, and email is experimental, per project. A message in a Slack thread or a Teams chat starts a session, and the agent replies in the same thread. Follow-ups stay in the same session.

## What does Kortix cost?

Self-host is free. The managed cloud has a free tier and a paid team plan; the current numbers are on the [Kortix pricing page](https://kortix.com/pricing). The [OpenWork alternatives FAQ](https://openworkalternative.com/faq) covers the OpenWork side.
