# n8n-kitchen-assistant
A smart WhatsApp-based kitchen assistant using n8n, OpenRouter, Google Sheets, and Twilio
# 🏠 n8n WhatsApp Home Assistant 🤖

An AI-powered smart home assistant that works over WhatsApp! Built with:

- 🧠 AI (via OpenRouter)
- 📦 Inventory tracking (Google Sheets)
- 🍳 Recipe suggestions with macros (protein + calories)
- 📉 Nutrition logging
- ⚙️ Workflow automation with [n8n](https://n8n.io)
- 📲 WhatsApp via Twilio

---

## 🔧 Features

✅ Add groceries via WhatsApp:  
> “Add 1 kg rice”

✅ Log meals and auto-deduct from inventory:  
> “I had 3 eggs”

✅ Get recipe ideas based on what’s available:  
> “What can I eat for breakfast?”

✅ Track protein, fat, carbs, and calories to Google Sheets

✅ All interactions are WhatsApp-friendly (under 500 chars, with emojis)

---

## 🧠 Stack

| Tool         | Purpose                          |
|--------------|----------------------------------|
| n8n          | Workflow orchestration           |
| OpenRouter   | AI agent (LLM prompt interpreter)|
| Google Sheets| Inventory + Nutrition DB         |
| Twilio       | WhatsApp messaging               |
| ngrok        | Tunnel for localhost access      |

---

## 📁 Files

- `workflow.json` – n8n workflow export (can be imported into your n8n instance)
- `README.md` – this file
![image](https://github.com/user-attachments/assets/c9c7b63d-abdc-4354-80e2-986fdc80c6f3)


---

## 🚀 Setup

1. Clone this repo or upload files to your n8n instance
2. Import `workflow.json` into n8n
3. Set up:
   - Google Sheets API credentials
   - OpenRouter API key
   - Twilio WhatsApp sandbox (or live)
4. Use ngrok to expose webhook:
ngrok http 5678

css
Copy
Edit
5. Connect Twilio webhook to:
https://<your-ngrok-subdomain>.ngrok.io/webhook/whatsapp-home-assistant

yaml
Copy
Edit

---

## 📸 Demo
![image](https://github.com/user-attachments/assets/528aaf04-9a13-4cc1-8aee-c50fd2e707a9)

![image](https://github.com/user-attachments/assets/734851c3-4c58-4e2f-9285-545412977c04)


---

## 🙌 Author

Built by Pritheevi Raj Narashimhan
Want to connect? Drop me a DM on LinkedIn or follow my projects 🚀

---

