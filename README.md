# Hey there, I'm Ayush Shende 👋
### Full-Stack Architect • Systems Optimizer • Database Wrangler • Embedded C++ Tamer

 _________________________________________________________________________
/ "If it has a 7-query network waterfall, an accidental mobile horizontal \
\  scroll, or an atomic TOCTOU race condition... I will hunt it down."     /
 -------------------------------------------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||

[![GitHub followers](https://img.shields.io/github/followers/Shende-Ayush?style=social)](https://github.com/Shende-Ayush)
[![TypeScript](https://img.shields.io/badge/TypeScript-React_19_%26_TanStack-3178C6?logo=typescript&logoColor=white)](https://github.com/Shende-Ayush)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Single--Trip_CTEs-336791?logo=postgresql&logoColor=white)](https://github.com/Shende-Ayush)
[![FastAPI](https://img.shields.io/badge/FastAPI-Async_Engines-009688?logo=fastapi&logoColor=white)](https://github.com/Shende-Ayush)
[![ESP32](https://img.shields.io/badge/ESP32-FreeRTOS_%26_I2S_DMA-E7352C?logo=espressif&logoColor=white)](https://github.com/Shende-Ayush)

---

## 🛠️ The TL;DR On Me

I build and optimize real-world software across the entire computing spectrum — from **microcontrollers streaming raw I2S audio over FreeRTOS ringbuffers** to **high-concurrency hospitality booking engines** running single-roundtrip PostgreSQL CTEs and edge caches.

I don't just write code; I aggressively optimize systems until:
- Database waterfalls drop from 7 network trips to **1 bundled CTE JSON payload in ~20ms**.
- 17-field monolithic forms fold into **frictionless progressive-disclosure reservation flows**.
- UIs stop looking like *"an old Oracle website from 1998"* and start looking like luxury resorts.
- Mobile screens on 390px viewports have **exactly 0px of accidental horizontal scroll**.

---

## 🚀 Battle-Tested Projects & What Actually Happened

### 1. 🏰 [Blue Lawn (Luxury Villa ERP & Booking Platform)](https://github.com/Shende-Ayush/Bluelawn)
> *Stack: React 19, TanStack Start & Router, PostgreSQL, Drizzle ORM, Nitro RPC, Tailwind CSS*

A complete, high-concurrency property management system (PMS) and booking engine built for luxury country estates.
- ⚡ **The 7-Roundtrip Annihilation**: Replaced a 560ms 7-query sequential waterfall on drawer opening with a single bundled PostgreSQL query using `json_build_object` and `json_agg`. Latency dropped to **~30ms**.
- 🛡️ **Guarded Slide-Over Architecture**: Built safe slide-over drawers with explicit edit locks. Because hotel managers accidentally modifying blocked dates while scrolling is a recipe for tears.
- 📉 **The Index Rescue**: Found queries using `EXTRACT(YEAR FROM date)` that forced full-table sequential scans. Swapped them for indexed B-Tree range bounds (`>=` and `<`) for an immediate **10x–50x speedup**.
- 📱 **Mobile Warfare**: Squashed rogue 516px filter bars stretching mobile screens; transformed overwhelming 17-field booking dialogs into 3-step progressive reservations.
- 💼 **Held Revenue & Commission Engine**: Enforced financial reality by separating tentatively held bookings from confirmed cash in the bank, alongside automated partner commission calculations.

---

### 2. 🎵 [Lyric Sync (Real-time Ambient Audio Clock on ESP32)](https://github.com/cognida-ai/lyric-sync-prot)
> *Stack: Embedded C++, ESP32, FreeRTOS, I2S DMA, PlatformIO, FastAPI, ShazamIO*

Hardware-accelerated ambient audio capture and real-time lyric projection.
- 🧵 **Atomic TOCTOU Race Condition Exorcism**: Fixed a gnarly Time-of-Check to Time-of-Use race condition in a circular `RingBuffer` where simultaneous DMA hardware interrupts and HTTP network reads caused memory corruption.
- ⏱️ **Driftless Zero-Polling Protocol**: Designed an anchor timestamp sync protocol (`anchor_pos_ms`, `server_time_ms`) allowing resource-constrained microcontrollers to locally interpolate lyric playback with millisecond precision without spamming the network.
- 🎙️ **Streaming Audio Sink**: Ingested chunked HTTP PCM streams into FastAPI and converted raw audio into WAV payloads on the fly.

---

### 3. 🥦 [groc-bot (Autonomous Nutrition & E-Commerce Agent)](https://github.com/balkars/groc-bot)
> *Stack: Python, LangGraph, ContextVars, Telegram Bot API, PostgreSQL, Zepto API*

An autonomous assistant that turns dietary meal planning into automated grocery carts.
- 🔍 **Distributed Correlation ID Tracing**: Built asynchronous ContextVar propagation tracing requests across incoming Telegram updates, background worker queues, and external e-commerce dispatchers.
- ⚡ **Async LangGraph Refactoring**: Overhauled synchronous graph pipelines into fully asynchronous `ainvoke_graph` execution, preventing worker thread bottlenecks.
- 🌐 **Timezone Normalization Defense**: Created `UTCDateTime` wrappers to banish timezone-naive comparisons and prevent orders from accidentally traveling across date boundaries.

---

### 4. 🦙 [Clean Ollama Dashboard & Docker Orchestration](https://github.com/Shende-Ayush/clean_ollama_dashboard)
> *Stack: FastAPI, Docker Compose, Nginx, React, Ollama API, Alembic*

A streamlined, developer-first hub for orchestrating and monitoring local LLM inference fleets.
- 🔄 **Flask to FastAPI Modernization**: Re-engineered legacy synchronous backends into an async FastAPI engine with live health probes, non-blocking DB connection waiting, and structured logging.
- 📊 **Model Discovery & Live Pull Manager**: Built a debounced search UI with stream progress bars and live context window configuration for local model downloads.
- 🐳 **Production Docker Multi-Container Compose**: Containerized Nginx reverse proxies, rate limiters, and backend inference nodes into one clean `docker compose up`.

---

## 💬 Real Quotes From The Commit Trenches

> *"Improve the Enquiry tabs view, it looks like an old Oracle website"*  
> — **Resolution:** Replaced dated gray tables with a luxury CRM featuring hot/warm/cold lead badges, live % conversion funnels, and instant WhatsApp CTAs.

> *"There is horizontal scroll in mobile view all over the place and the booking form looks too complicated for a new user !!"*  
> — **Resolution:** Fixed flex wrappers, clamped root containers to 390px viewports, and collapsed 14 secondary fields behind progressive disclosure.

> *"I made a wrong payment entry and now I am not able to edit / change / delete it"*  
> — **Resolution:** Added transactional payment adjustments with automatic audit trails and live balance recalculation so nobody panics over a typo.

---

## 🧰 My Technical Arsenal

├── Languages :: TypeScript • JavaScript • Python • C/C++ • SQL ├── Frontend Mastery :: React 19 • TanStack Start • TanStack Router • TanStack Query • Tailwind CSS ├── Backend & Runtimes :: Node.js • Nitro RPC • FastAPI • FreeRTOS (ESP32) ├── Databases & Storage :: PostgreSQL (CTEs, Window Functions, json_agg) • Drizzle ORM • Supabase • Redis ├── Systems & DevOps :: Docker Compose • Nginx • Vercel Edge • Git • PlatformIO (I2S DMA) └── AI & Agents :: LangGraph • Ollama Orchestration • Multi-Agent Pipelines



---

## 📈 Engineering Truths I Live By

1. **If your query takes more than 1 network hop to render a modal, you're doing it wrong.** (PostgreSQL can return a single JSON tree faster than your network can send a second handshake).
2. **Never trust client-side dates without timezone guards.** (`UTCDateTime` or prepare to explain why a booking arrived yesterday).
3. **Progressive disclosure is king.** Don't show users 18 inputs when 3 will get the job done.
4. **Always test on a 390px mobile viewport.** If it scrolls sideways, it's not done.

---

<p align="center">
  <i>Want to talk high-performance database queries, microcontrollers, or web apps that feel like magic?</i><br>
  <b><a href="https://github.com/Shende-Ayush">Let's connect on GitHub!</a></b>
</p>
