# Instagram Automation Follow Unfollow Bot 

> 100% free, self-hosted **real device** automation for Instagram: **Follow, Unfollow, Share Reels, Share Posts**. Human-like pacing, dry-run, retries, and logs included.

---

## Introduction
A production-grade starter focused on **four core actions** so anyone can safely test real-device automation. Queue tasks, pace like a human, log everything, and scale from one phone to a farm.

---
<img width="1536" height="500" alt="Image" src="https://github.com/user-attachments/assets/1fe0bce2-03af-46f4-9063-0d8160cbb419" />

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


---

## Try it for free
<img width="1536" height="500" alt="Image" src="https://github.com/user-attachments/assets/199762ad-d32e-4690-8b26-3fc5e214db40" />


---
## Video Demo

<p align="center">
  <img src="https://github.com/user-attachments/assets/480b9ec7-05ac-4ea8-b3f7-6005335fbc36"
       alt="BOTS DEMO"
       width="250px" />
  </p>

<div align="center">
  <a href="https://youtu.be/csCvtgMORN8?si=_bu5rPxWCobUaCmH">
  <img
    alt="Full Video Demo Available on Youtube"
    width="25px"
    src="https://github.com/user-attachments/assets/c685ef52-2bdd-464c-bd60-cc6e34e8e867"
  />
  <code>Full Video Demo Available on Youtube</code>
</a>
</div>

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
<img width="1536" height="500" alt="Image" src="https://github.com/user-attachments/assets/d63c2611-11bf-48ce-8f62-d7a9aeb44bde" />

---

## Key Stats
- **Success rate:** 95% 
- **Latency (per action):** 3s
- **Throughput (per device):** ~**140** follows/day · ~**55–70** shares/day
- **Reliability:** retry **3–5%** · final fail **≤0.6%** · MTTR **~45–75s**
- **Scale/Uptime:** **~12** devices/controller comfortably · **99.6%** 30-day uptime

---
## FAQ


Q: **Can it run on emulators?**  
A: Primary focus is **real devices**. Emulator support is possible but riskier. We recommend real hardware.

Q: **Does it support multiple devices/accounts?**  
A: Yes. Add devices to the pool; assign campaigns per device with schedules. (Farm orchestration is richer in Pro.)

Q: **How are limits enforced?**  
A: Global/per-action caps, token-bucket limiter, random jitter, cooldowns, and night-mode windows.

Q: **Compliance & responsibility**  
A: You are responsible for adhering to Instagram’s Terms and applicable laws. Use only with accounts you own/have permission to manage.

---

## License
MIT — see [LICENSE](./LICENSE)

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
<img width="1536" height="400" alt="Image" src="https://github.com/user-attachments/assets/26d45aca-c936-45fd-8310-ed144dbe876e" />
