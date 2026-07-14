# AI-Powered Market Intelligence & Automation for Wayfair Rugs

n8n automation suite built during the [Extern](https://www.extern.com/) remote externship with **Wayfair** (10/2025 – 01/2026). Four LLM-powered agents turn raw market data into pricing, trend, and marketing decisions for Wayfair's rug category.

📄 Full project documentation: [`wayfair .pdf`](./wayfair%20.pdf) · Externship certificate: [`Extern CERTI.pdf`](./Extern%20CERTI.pdf)

## The four agents

### 1. Moodboard Generator
Converts short design prompts (e.g., *"Bohemian rugs, neutral tones"*) into AI-curated visual moodboards, helping the team explore emerging rug styles, palettes, and visual directions.

### 2. Competitor Monitoring & Pricing Comparison
Compares Wayfair rug prices against Amazon: builds a price-comparison table, calculates gaps ($ and %), classifies each SKU as *Cheaper / Parity / Premium*, and outputs one concrete pricing action per gap (e.g., "Lower SKU X to $199") as an HTML report.

### 3. Marketing Content Automation
Scrapes Amazon product data (pricing, features, styles) → GPT-4o analysis → trend insights (e.g., "Washable Farmhouse Rugs") and ready-to-publish marketing assets: blog posts, Instagram captions, HTML reports.

### 4. Market Intelligence Orchestrator
Synchronizes product, pricing, and trend data between Google Sheets (control layer) and Supabase (database), giving all agents structured access to shared data for pattern analysis and real-time decision support.

## Stack

**n8n** (workflow orchestration) · **OpenAI GPT-4o** (analysis & generation) · **Google Sheets** (control) · **Supabase** (storage) · web scraping · HTML reporting

## What I learned

Designing multi-agent n8n workflows around real business questions: prompt design with strict output contracts, keeping LLM outputs decision-ready (tables, classifications, actions — not prose), and syncing spreadsheet-driven control with a proper database.
