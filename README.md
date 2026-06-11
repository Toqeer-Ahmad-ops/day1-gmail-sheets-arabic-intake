Qoton Urgency Bot - Dubai 🇦🇪
Automated Arabic rush-order alerts for retail print ops

Built: June 2025 | Learning AI since: April 2025
Stack: n8n, Gemini 2.5 Flash, Google Sheets, Gmail API, WhatsApp API
ROI: 12.5 AED saved per urgent order → 1,250 AED/mo projected

🎯 Problem
At Qoton Printing Dubai, rush orders marked عاجل in Arabic notes were missed.
15min delay = 12.5 AED loss per order.

⚡ Solution
n8n workflow reads Arabic notes → Gemini 2.5 flags عاجل/ضروري → Instant Gmail + WhatsApp alert

Flow: Google Sheets → Gemini NLP → IF urgent → Gmail + WhatsApp → Mark processed

📊 Results
4/5 orders flagged correctly in test
8 seconds end-to-end latency
12.5 AED saved per order
100% Arabic عاجل detection
🚀 Demo
Loom video: [Coming after Day 4 WhatsApp integration]

🛠️ Setup
Import qoton-urgency-bot.json to n8n
Add Gemini API key + Gmail OAuth
Connect Google Sheet with Order_ID | Product | Arabic_Note
Status: Day 3 complete. Day 4: Adding WhatsApp API. Day 5: Write-back to Sheet.
