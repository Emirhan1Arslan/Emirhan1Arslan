# Emirhan Arslan

Computer Engineering graduate (November 2026) based in Ankara, Türkiye. I build full-stack products and applied AI systems, and I run them on my own server.

[emirhanarslan.com](https://www.emirhanarslan.com) · [LinkedIn](https://www.linkedin.com/in/emirhan1arslan)

## T-Rage Studios

My own software studio, since October 2025. These products are live on my server. Their code is private, so this page describes them.

| Product | What it is | Stack |
|---|---|---|
| [**KUTRA ERP**](https://kutra.tragestudios.com) | Multi-tenant ERP: CRM, proposals, purchasing and RFQs, stock, invoicing, accounting, HR, projects and contracts, on a backend of 40+ modules | Go (Fiber), PostgreSQL, Next.js, TanStack Query, Zustand, AG Grid |
| [**BUDUN CRM**](https://budun.tragestudios.com) | No-code, multi-tenant CRM: each workspace defines its own objects and fields; deal Kanban, automations, reports, API keys and webhooks | Go, PostgreSQL, Flutter (web and mobile) |
| [**BİTİG**](https://bitig.tragestudios.com) | Generates the paperwork of a software sale (project scope, contracts, NDA, delivery record, KVKK notice) from editable templates | Next.js, Drizzle ORM, Tiptap |
| [**HukukBot**](https://hukukbot.tragestudios.com) | AI assistant for Turkish law, built for my B.Sc. thesis: agentic RAG, streaming answers with law and article citations, multi-user chat history | Next.js 15, Auth.js, Prisma, FastAPI, ChromaDB, PostgreSQL, OpenRouter |

For HukukBot I first compared four approaches on Qwen2.5-32B-Instruct (RAG, two LoRA fine-tunes and the base model) on a 30-question test set scored by an LLM judge and human judges. RAG clearly won, so the product is built on it.

**Infrastructure.** Everything runs on my own Ubuntu server as Docker Compose stacks behind an nginx reverse proxy (about 20 subdomains), with shared PostgreSQL, Redis and Meilisearch. Pushes to GitHub deploy automatically through my own webhook server, and a small FastAPI service logs every HTTP request to PostgreSQL.

## Public projects

- [**dual-sim-messenger**](https://github.com/Emirhan1Arslan/dual-sim-messenger): default SMS app for dual-SIM Android phones, written in Kotlin and Jetpack Compose. I use it every day.
- [**PhoneOS**](https://github.com/Emirhan1Arslan/PhoneOS): experimental bare-metal operating system for a Huawei P8 Lite, in C and AArch64 assembly. Runs in QEMU; on the real phone it does not get past the boot logo yet.
- [**online_clipboard**](https://github.com/Emirhan1Arslan/online_clipboard): clipboard sync between devices with Flutter and Firebase, live on the [web](https://onlineclipboard.bbclub.space) and [Google Play](https://play.google.com/store/apps/details?id=com.bbclub.onlineclipboard).
- [**Hidden Pairs**](https://hiddenpairs.tragestudios.com): a Unity memory game that runs in the browser (WebGL).

## Published tools

- [**Easy Code Cleaner**](https://marketplace.visualstudio.com/items?itemName=EmirhanArslan.easy-code-cleaner) (Visual Studio Marketplace, 180+ installs): a VS Code extension that removes comments, emojis, blank lines and debug statements across a workspace, and shows code statistics for the project.
- [**Editor Terminal for Unity**](https://assetstore.unity.com/packages/package/382850) (Unity Asset Store): I first built it to run Claude Code without leaving the Unity Editor, then published it as a general-purpose terminal. It runs a real interactive PowerShell or cmd session inside the Editor, built on the Windows ConPTY API. A small native helper running outside Unity's job object keeps the shell alive across script recompiles. Published under T-Rage Studios.

## Experience

- **Happencode Yazılım**, long-term intern (2026): 3D product configurator with Unity and Three.js, e-commerce front-ends with Next.js
- **İba Valresa**, project engineer (2025-2026): factory-wide web apps and a 6-module maintenance management system (CMMS)
- **Forel Teknoloji**, software developer intern (2024-2025): asset management web app aligned with ISO 27001

## How I work

Claude Code is my main coding tool: the T-Rage Studios products and dual-sim-messenger were built with it. I set projects up with CLAUDE.md instructions, custom commands, skills and hooks, and I wrote my own MCP server. I also use Cursor.

**Languages:** TypeScript, Python, Go, C#, Kotlin, Dart, C
