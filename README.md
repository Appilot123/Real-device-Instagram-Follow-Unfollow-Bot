# Real-Device Instagram Automation Bot — Free Core Actions

> 100% free, self-hosted **real device** automation for Instagram: **Follow, Unfollow, Share Reels, Share Posts**. Human-like pacing, dry-run, retries, and logs included.

---

## Introduction
A production-grade starter focused on **four core actions** so anyone can safely test real-device automation. Queue tasks, pace like a human, log everything, and scale from one phone to a farm.

---
<img width="1536" height="500" alt="Hero" src="./assets/hero.png" />

---

## Table of content
- [Overview](#overview)
- [Features](#features)
- [Try it for free](#try-it-for-free)
- [Workflow](#workflow)
- [Workflow image](#workflow-image)
- [Key Stats](#key-stats)
- [FAQ](#faq)
- [Contact us](#contact-us)
- [License](#license)
- [Footer image](#footer-image)

---

## Overview
This bot drives **real devices** via ADB/Appium to execute Instagram actions with rate limits, random jitter, and behavior rules. It supports campaign queues, error handling with retries, and structured logs so you can review every action and safely re-run failed steps. This repository is **limited to the four free actions** listed below; the full Pro suite (Likes, Comments, Stories, Posting, DMs, Scheduler, Farm Manager, etc.) lives in the main Pro repo.

---

## Features

| # | Feature | Description |
|---|---|---|
| 1 | Follow | Follow targets from lists/queries with human-like delays, per-action caps, and random jitter. |
| 2 | Unfollow | Unfollow by lists, FIFO/LIFO, or “non-followers only” with safe daily limits. |
| 3 | Share reels | Share any reel to DMs or to your story share queue (share action). |
| 4 | Share posts | Share feed posts to DMs or to your story share queue (share action). |

**Built-in mechanics:** rate limiter + jitter, retries with backoff, dry-run mode, JSON logs, screenshots on error, idempotent resumes.

---

## Try it for free
<img width="1536" height="500" alt="Try it Free" src="./assets/try-free.png" />

- **Included**: Follow, Unfollow, Share Reels, Share Posts  
- **Upgrade path**: Move to Pro for Likes, Comments, Stories, Posting, DMs, Scheduler, Device Farm Manager, and more

---

## Workflow

1) **Connect devices** (ADB/Appium) → verify health, proxy/SIM, storage.  
2) **Load campaign** (targets, limits, schedules).  
3) **Humanizer** applies dwell/scroll/jitter rules per action.  
4) **Executor** runs actions with retries + backoff; screenshots on error.  
5) **Logger** writes per-step JSON, aggregates run report.  
6) **Review** results; resume failed steps idempotently.

---

## Workflow image
<img width="1536" height="500" alt="Workflow" src="./assets/workflow.png" />

---

## Key Stats
- **Real devices**: Android (USB/Wi-Fi ADB) & iOS (via Appium)  
- **Pacing**: Rate-limit + random jitter; per-action caps  
- **Scale**: Designed for device farms (dozens+) with queues  
- **Reliability**: Retries + exponential backoff + crash recovery  
- **Observability**: JSON logs, screenshots on error, run summaries  
- **Extensible**: Same structure as Pro—upgrade without rewriting

---

## FAQ

Q: **Is this safe for my accounts?**  
A: No automation is “risk-free.” Use conservative limits, unique device fingerprints, quality proxies/SIMs, and warm accounts first.

Q: **Does this repo include DMs, Likes, Comments, or Posting?**  
A: This free repo includes **Follow, Unfollow, Share Reels, Share Posts**. Pro unlocks DMs, Posting, Likes, Comments, Stories, Scheduler, Farm Manager, etc.

Q: **Can it run on emulators?**  
A: Primary focus is **real devices**. Emulator support is possible but riskier. We recommend real hardware.

Q: **Does it support multiple devices/accounts?**  
A: Yes. Add devices to the pool; assign campaigns per device with schedules. (Farm orchestration is richer in Pro.)

Q: **How are limits enforced?**  
A: Global/per-action caps, token-bucket limiter, random jitter, cooldowns, and night-mode windows.

Q: **Compliance & responsibility**  
A: You are responsible for adhering to Instagram’s Terms and applicable laws. Use only with accounts you own/have permission to manage.

---

## Contact us
<p align="center">
  <a href="https://discord.gg/zX7frTbx">
    <img alt="Discord contact" src="https://img.shields.io/badge/Discord-Appilot-5865F2?logo=discord&logoColor=white&style=for-the-badge">
  </a>
  <a href="https://t.me/devpilot1">
    <img alt="Telegram contact" src="https://img.shields.io/badge/Telegram-@devpilot1-2CA5E0?logo=telegram&logoColor=white&style=for-the-badge">
  </a>
</p>

---

## License
MIT — see [LICENSE](./LICENSE)

---

## Footer image
<img width="1536" height="400" alt="Footer" src="./assets/footer.png" />
