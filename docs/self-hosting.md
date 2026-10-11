# Self-hosting open-source OpenWork alternatives

Kortix is open source, and self-hosting it is free. If you are leaving OpenWork's desktop-first model and want the platform on your own infrastructure, the difference is what each option installs and what it asks of you.

## Kortix

Kortix has a single command from a fresh machine:

```bash
curl -fsSL https://kortix.com/install | bash
kortix self-host start
```

`kortix self-host start` runs one Docker Compose stack on your own box. The first run asks six things and no model key. GitHub connects in the dashboard under Settings → Git, and models are bring-your-own-key in the app. The stack has no Redis and no separate worker, so there is less to operate than a typical platform install. The full host path is in the [Kortix documentation](https://kortix.com/docs).

Kortix also runs on Kortix Cloud and in your own VPC. The same product runs in all three places, so a team can start on the managed cloud and move the same repository onto their own network later. Connector credentials are brokered server-side and never enter the machine, which matters when the platform sits inside your perimeter.

## OpenWork

OpenWork's desktop app runs on macOS, Windows and Linux with no server to stand up, and your files stay on your machine. For a team, the OpenWork Den control plane can be self-hosted on your own infrastructure; the [OpenWork repo](https://github.com/different-ai/openwork) documents the path. The desktop app needs no OpenWork account to run locally. The team control plane, under `ee/`, is a source-available license with production use requiring a subscription above 5 users.

## The other options

- **Open WebUI** installs with pip or Docker, or on Kubernetes, and can run fully offline. It centers on chat and retrieval over your own documents.
- **OpenHands** runs on a laptop, in Docker, on a VM, or on a server in the cloud, and can connect to several agent backends from one control center.
- **AnythingLLM** ships as a desktop app and a Docker image, and runs locally by default with zero setup.
- **Eigent** deploys a local backend with local model support and needs no cloud account.
- **OpenClaw** installs its Gateway on your own hardware, where state, memory and credentials live.
- **Hermes** supports seven terminal backends, including local, Docker, SSH, Modal, Daytona and Vercel Sandbox.

## What self-hosting changes

Self-hosting moves the operational load onto your team: the machine, the updates, the model keys, and the access control. For Kortix that is one Compose stack and bring-your-own model keys. For a desktop-first tool it is a machine-by-machine install plus a separate path for the team control plane. Decide which of those two you are signing up for before you pick. The [OpenWork self-hosting guide](https://openworkalternative.com/self-hosting) has the OpenWork-specific steps.
