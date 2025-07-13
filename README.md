# 💰 Personal Finance Analyzer — AI + Automation

Automatically track, categorize, and chat with your expenses using your bank statement, OpenAI, and Google Sheets — all powered by n8n.

No more manual Excel wrangling. No more forgotten subscriptions. Just smart insights delivered instantly.

---

## 🧩 Features

### ✅ Workflow 1: Categorize Your Monthly Expenses
- 🔁 Watches a Google Drive folder for new `.xls` bank statements
- 🧹 Cleans and extracts only valid transaction rows
- 🧠 Sends to GPT (via OpenAI) to categorize each transaction into:
  - Food & Dining, Shopping, Transport, Entertainment, Health, Utilities, etc.
- 📄 Saves structured results in a Google Sheet

### 💬 Workflow 2: Chat With Your Expenses
- 🤖 Ask natural questions like:
  - “Where did I spend on entertainment?”
  - “How much peer transfer did I do last month?”
  - “List all unknown expenses”
- 🔍 Bot fetches relevant results from your categorized sheet
- 🧾 Returns neatly formatted bullet list + total summary

---

## 🛠️ Tech Stack

- [n8n](https://n8n.io/) – Open-source workflow automation
- [OpenAI GPT-4o](https://platform.openai.com/)
- Google Sheets & Google Drive

---

## 📁 Project Structure

- workflow1_personal_finance_parser.json # Handles bank statement parsing + categorization
- workflow2_expense_chat_assistant.json # Enables chat-based queries on expenses

  
---

## 🚀 Setup Instructions

1. **Connect n8n credentials**:
   - Google Drive (for file trigger)
   - Google Sheets (for data storage)
   - OpenAI (for categorization + chat)
2. **Create your Google Sheet**:
   - Columns: `date`, `description`, `amount`, `category`
3. **Import workflows** into n8n
4. **Update placeholder fields**:
   - Replace credential references with your own
   - Replace sheet and folder IDs
5. **Activate workflows**

---

## 🔐 Privacy

- No API keys or tokens are included in the workflows.
- Self-hosted n8n recommended for full control.
- Sensitive data never leaves your environment except via OpenAI call.

---

## 🧠 Real Example: How It Helped Me

> Discovered I was paying ₹59/month for a **YouTube channel membership** I forgot about.  
> Turns out I’d subscribed for a show that **stopped in February** —  
> Yet I kept paying… for **6 straight months**.  
> This tool caught it in seconds.  
> ₹354/year saved, instantly 💸

---

## 🤝 Credits

Created by [Aniket Rochwani](https://www.linkedin.com/in/aniket-rochwani/)  
Inspired by real pain. Built for real people.

---

## 📣 Suggested Hashtags

`#n8n #AItools #OpenAI #PersonalFinance #NoCode #Automation #ExpenseTracker #SmartMoney`

---

## 🙌 Want to Contribute?

Open an issue or submit a PR. Let's make personal finance smarter together.
