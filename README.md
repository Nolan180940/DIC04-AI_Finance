# ETF Navigator: An AI Agent for Sustainable Investment Discovery

> **DIC 2025 Finance Track (Track 04) – Stage 1 Submission**  
> Team: DIC04-AI_Finance
> Repository: `DIC04-ETF-Navigator`  
> Live Demo: yet to publish
> 📅 Stage 1 Deadline: December 24, 2025

---

## 🎯 Overview

**ETF Navigator** is an AI-powered investment research platform that helps users discover, analyze, and monitor **sustainable ETFs** (e.g., Clean Energy, ESG-themed funds).  

Unlike traditional financial dashboards, our system is built around an **AI Agent** that:
- Fetches and synthesizes real-time market data
- Summarizes news and trends in plain language
- Highlights sustainability-aligned investment opportunities
- Supports both U.S. and Chinese markets

This project directly responds to the track theme:  
**“AI Agents Unlock Finance for Sustainability”**.

---

## 🤖 AI Agent Design

The core of ETF Navigator is an **autonomous AI Agent** implemented via Base44’s LLM integration layer. It operates as follows:

1. **Perception**:  
   Receives user queries or scheduled triggers (e.g., “Show today’s market update”).

2. **Reasoning & Data Retrieval**:  
   Uses structured prompts to invoke a large language model (LLM) with internet access (`add_context_from_internet: true`). The LLM is instructed to:
   - Search for credible financial sources (e.g., AP News, official fund websites)
   - Extract structured data (indices, ETF prices, sector performance)
   - Identify sustainability-relevant categories (e.g., “Clean Energy”, “Low Carbon”)

3. **Action & Transparency**:  
   Returns validated JSON responses that power the UI.  
   All recommendations include **data provenance** (e.g., source URLs) to ensure auditability.

---

## 🔧 Technical Implementation

| Component       | Technology / Approach                                                                 |
|-----------------|----------------------------------------------------------------------------------------|
| **Frontend & Agent Logic** | Built on [Base44](https://app.base44.com/) – a low-code platform for AI-native apps |
| **Data Sourcing**         | Public financial data retrieved via LLM with internet access (no private APIs)        |
| **Sustainability Focus**  | Dedicated sections for "Clean Energy ETFs", ESG analysis, and China's green finance   |
| **Ethical Design**        | - No user financial data collected<br>- All outputs labeled “for informational purposes only”<br>- Sources disclosed in footnotes |

> 🔐 **Note**: The live demo is hosted on Base44 for rapid prototyping. **All custom logic (page components, prompts, data models) has been manually exported and is included in this repository** for transparency and review.

---

## 📁 Repository Structure

- `/pages` – Core page components (Dashboard, Research, Watchlist, etc.)  
- `/components` – Reusable UI modules (MarketOverview, PopularETFs, etc.)  
- `/entities` – Data models (ETF, WatchlistItem)  
- `/integrations` – Core LLM invocation logic (`Core.js`)  
- `proposal.pdf` – Full Stage 1 proposal  
- `demo.mp4` – 3-minute demonstration video

---

## 📜 Submission Compliance

- This repository is **private** and shared with `NYUSH_DIC` as requested.  

© [DIC04-AI_Finance], 2025. For DIC 2025 competition use only.
