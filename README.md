# Day 1: Gmail → Google Sheets Arabic Order Intake

**Part 1 of 4**: Foundation for Arabic عاجل → Telegram Bot system

**Built**: June 2025 | **For**: Qoton Printing Dubai

## 🎯 Problem

Qoton Printing Dubai receives 50+ Arabic orders/day via Gmail. Manual copy-paste to Sheets takes 2hrs/day. Rush orders marked **عاجل** in Arabic notes were missed. 15min delay = 12.5 AED loss per order.

## ⚡ Solution — Day 1

**n8n workflow**: Gmail → Google Sheets automation

**Flow**: Gmail trigger → Extract Order_ID, Product, Arabic_Note → Append to Sheet

**Result**: 50+ emails/day → Structured data in Sheets. Zero manual entry.

## 📊 Results

- **Time saved**: 2 hours/day manual work → 0 seconds
- **Data structure**: Order_ID | Product | Arabic_Note columns
- **Foundation set**: Feeds Day 2 Gemini NLP for urgency detection

## 🛠 Tech Stack

**n8n** | **Gmail API** | **Google Sheets API**

## 🚀 Evolution

This Day 1 intake feeds the full system:
1. **Day 2**: Gemini detects عاجل/ضروري from Arabic_Note
2. **Day 3**: n8n routes if urgent = true 
3. **Day 4**: Telegram sends instant Arabic alert

**See complete system**: [arabic-urgency-telegram-bot](https://github.com/Toqeer-Ahmad-ops/arabic-urgency-telegram-bot)

## Setup

1. Import workflow: `/workflows/day1-gmail-sheets.json`
2. Add Gmail OAuth + Google Sheets credentials
3. Connect Sheet with headers: Order_ID | Product | Arabic_Note

---
**Status**: Day 1 Complete → Upgraded to Day 4 production system
**Next**: See Day 4 repo for live Telegram alerts + $0 cost proof
