# 📝 LinkedIn Content Creator Workflow (n8n)

This repository contains an automated workflow built in **n8n** that generates professional LinkedIn post content using trending article data fetched from **Tevily**, managed via **Google Sheets**, and styled by **OpenAI GPT**.

---

## 📌 Features

- 🧠 **Reads topics** from a Google Sheet
- 🔍 **Fetches articles** via the Tevily Search API
- 🤖 **Summarizes and rewrites content** into 12–15 line LinkedIn-style posts using GPT
- ✍️ **Posts are written** with emojis, a hook, multiple paragraphs, and a call-to-action
- 🧾 **Updates the sheet** with the generated content and marks the status as "Created"

---

## 🔧 Workflow Overview

```plaintext
[Manual Trigger]
   ↓
[Google Sheet] → Get topics with "To Do" status
   ↓
[Tevily API] → Search 3 relevant articles
   ↓
[AI Agent] → Convert to 12–15 line engaging LinkedIn post
   ↓
[Google Sheet] → Save content + update status to "Created"
