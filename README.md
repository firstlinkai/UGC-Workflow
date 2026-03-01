# n8n UGC Automation Workflow

An automated pipeline for generating high-converting User-Generated Content (UGC) marketing materials. This workflow uses AI to research products on TikTok, draft engaging scripts, and match them with appropriate AI avatars.

## 🚀 Overview
This workflow automates the creative process for social media ads (TikTok, Instagram, Facebook). It transforms a simple product name into a full marketing suite including scripts, captions, and avatar recommendations.

## ✨ Features
- **TikTok Scraper**: Uses Apify to research current trends and content associated with your product.
- **AI Copywriting**: Generates 30–45 second UGC-style scripts based on specific marketing angles (e.g., Emotional Benefit, Problem/Solution).
- **Structured Output**: Produces ready-to-use captions with emojis and hashtags.
- **Avatar Matching**: Uses a semantic search agent to find the best AI avatar and voice ID from your internal database.
- **Data Persistence**: Automatically logs all generated scripts and metadata to Google Sheets.

## 🛠️ Requirements
- **n8n** (v1.0+)
- **OpenRouter API Key** (supporting models like Qwen)
- **Apify API Key** (for TikTok scraping)
- **Google Sheets Credentials**

## 📝 Setup
1. Import the `UGC.json` file into your n8n instance.
2. Connect your **OpenRouter**, **Google Sheets**, and **Apify** credentials.
3. Configure the Google Sheet URL in the "Save UGC Info" and "Save URLs" nodes.
4. Trigger the workflow via the built-in n8n form.
