# ETF Navigator: An AI Agent for Sustainable Investment Discovery

> **DIC 2025 Finance Track (Track 04) – Stage 1 Submission**  
> Team: DIC04-AI_Finance
> Repository: `DIC04-AI_Finance`  
> Live Demo: contemporary demo site: [https://etf-navigator-f8d67fe2.base44.app/](https://etf-navigator-f8d67fe2.base44.app/)
> **Current prototype**：https://etf-navigator-f8d67fe2.base44.app/

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
| **Data Sourcing**         | Public financial data retrieved via LLM with internet access         |
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

- This repository is **private** and shared with `NYUSH_DIC` and team members as requested.  

© [DIC04-AI_Finance], 2025. For DIC 2025 competition use only.

---


README-ZH


---


# ETF Navigator：面向可持续投资发现的 AI Agent

> **DIC 2025 金融赛道（赛道 04）– 第一赛段提交**  
> 团队：DIC04-AI_Finance  
> 代码仓库：`DIC04-AI_Finance`  
> 在线演示：暂定的演示地址：https://etf-navigator-f8d67fe2.base44.app/

---

## 🎯 项目概述

**ETF Navigator** 是一个由 AI 驱动的投资研究平台，帮助用户发现、分析和监控**可持续型 ETF**（例如清洁能源、ESG 主题基金）。

与传统金融仪表盘不同，本系统围绕一个**AI Agent**构建，具备以下能力：
- 获取并整合实时市场数据  
- 用通俗语言总结新闻与趋势  
- 突出展示与可持续发展目标对齐的投资机会  
- 同时支持美国与中国市场  

本项目直接响应赛道主题：  
**“AI Agent 解锁可持续发展的金融潜力”**。

---

## 🤖 AI Agent 设计

ETF Navigator 的核心是一个**自主运行的 AI Agent**，通过 Base44 平台的 LLM 集成层实现，其工作流程如下：

1. **感知（Perception）**  
   接收用户查询或定时触发指令（例如：“显示今日市场简报”）。

2. **推理与数据获取（Reasoning & Data Retrieval）**  
   使用结构化提示（prompt）调用具备联网能力的大语言模型（LLM，启用 `add_context_from_internet: true`），指令 LLM：  
   - 从可信金融信源（如美联社 AP News、基金公司官网）搜索信息  
   - 提取结构化数据（指数、ETF 价格、板块表现）  
   - 识别与可持续性相关的类别（如“清洁能源”、“低碳”）

3. **行动与透明度（Action & Transparency）**  
   返回经校验的 JSON 数据驱动前端界面。  
   所有推荐均包含**数据来源引用**（如源链接），确保可审计性与透明度。

---

## 🔧 技术实现

| 组件 | 技术与方法 |
|------|-----------|
| **前端与 Agent 逻辑** | 基于 [Base44](https://app.base44.com/) 构建 —— 一个面向 AI 原生应用的低代码平台 |
| **数据获取** | 通过 LLM 联网获取公开金融数据 |
| **可持续聚焦** | 专设“清洁能源 ETF”、“ESG 分析”、“中国绿色金融”等模块 |
| **伦理设计** | - 不收集用户任何财务或身份信息<br>- 所有输出标注“仅限信息参考，不构成投资建议”<br>- 在脚注中披露数据来源 |

> 🔐 **说明**：在线演示托管于 Base44，用于快速原型开发。**所有自定义逻辑（页面组件、提示词、数据模型）均已手动导出，并完整包含在本代码仓库中**，以确保透明度与评审可查性。

---

## 📁 代码仓库结构

- `/pages` – 核心页面组件（Dashboard、Research、Watchlist 等）  
- `/components` – 可复用 UI 模块（MarketOverview、PopularETFs 等）  
- `/entities` – 数据模型（ETF、WatchlistItem）  
- `/integrations` – 核心 LLM 调用逻辑（`Core.js`）  
- `proposal.pdf` – 完整第一赛段提案  
- `demo.mp4` – 3 分钟演示视频

---

## 📜 提交合规性声明

- 本仓库为**私有仓库**，并已按要求邀请 `NYUSH_DIC` 与其他参赛队员为协作者。  

© DIC04-AI_Finance，2025。仅供 DIC 2025 竞赛使用。
