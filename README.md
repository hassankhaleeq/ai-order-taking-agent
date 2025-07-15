# ai-order-taking-agent
AI-powered voice ordering assistant built with Vapi, Twilio, OpenAI, and n8n. Takes customer orders via voice call and sends confirmations via WhatsApp to customer and even sends email to owner that cutomer has placed order.


This is an AI-powered voice ordering system that allows customers to place food orders simply by making a phone call.  
No app, no buttons — just speak, and the system will understand the order, process it, and send a confirmation via WhatsApp.

---

## 🛠️ Tech Stack

- **Vapi** – Voice AI platform to handle phone calls
- **Twilio** – For receiving and routing phone calls
- **OpenAI** – Processes natural language and generates replies
- **n8n** – Automation platform to handle the entire workflow
- **Wassenger** – Sends WhatsApp confirmation messages to customers
- **Pinecone (optional)** – For RAG (retrieval-augmented generation) if menu/FAQ data is needed

---

## 💡 How It Works

1. **Customer makes a phone call** to your Twilio number
2. **Vapi listens** to the call and forwards the query to OpenAI
3. **OpenAI generates a smart response** based on customer input (like a food order)
4. **n8n receives the response**, handles logic, stores info, and sends the order data **and even tells ,suggest or anaswer any menu releated question by using rag**
5. **Wassenger sends an order confirmation** to the customer via WhatsApp

---

## 📦 Features

- Fully voice-driven: no typing, no apps
- Real-time order processing using OpenAI
- Order confirmation via WhatsApp with dynamic message content
- Easy to modify for other use-cases like bookings, support, FAQs
- Built with no-code and low-code tools — great for indie developers

---

## 📲 How to Use

> You’ll need working API keys and accounts for:
> - Vapi
> - Twilio
> - OpenAI
> - Wassenger
> - n8n Cloud or Self-hosted

1. Set up the **n8n workflow** (JSON file included in this repo) **and you can also download zip file for extra information which include all promts which will be helpfull to setup your agent**
2. Connect your Twilio number to Vapi
3. Set Vapi to forward calls to your n8n webhook
4. Customize the logic for your restaurant’s menu and flow
5. Test by making a phone call to your Twilio number

---

## 📁 Project Files

- `workflow.json` – Complete n8n automation flow
- `menu+faq.pdf` – Menu and FAQs used for context (RAG)
- `README.md` – This file

---

## 🎯 Use Cases

- Restaurant voice ordering
- Hotel bookings
- Voice support agents
- WhatsApp auto-replies
- Birthday reminder bots

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♂️ About the Creator

**Hassan Khaleeq** – Indie automation and AI developer from Pakistan 🇵🇰  
I specialize in building voice-based AI agents using tools like n8n, Twilio, Vapi, and OpenAI.

Follow me on GitHub and feel free to reach out for freelance or collaborations!

