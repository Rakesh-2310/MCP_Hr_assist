# 🚀 MCP_Hr_assist

### 🧠 AI-Powered HR Management System using MCP (Model Context Protocol)

MCP_Hr_assist is an intelligent HR automation system that leverages **Model Context Protocol (MCP)** to enable AI-driven interaction with HR operations such as employee onboarding, leave management, ticketing, meeting scheduling, and email automation.

---

## 🏗️ Project Architecture

```
MCP_Hr_assist/
│
├── HRMS/
│   ├── employee_manager.py
│   ├── leave_manager.py
│   ├── meeting_manager.py
│   ├── ticket_manager.py
│   ├── schemas.py
│
├── emails.py           # Email sending logic (SMTP)
├── utils.py            # Seed data setup
├── server.py           # MCP server (tools + prompts)
├── README.md
```

---

## ⚙️ Tech Stack

* Python
* FastMCP (Model Context Protocol)

---

## 🧠 MCP Concepts Used

* `@mcp.tool()` → Exposes backend functions to LLM
* `@mcp.prompt()` → Defines structured workflows
* Tool chaining via LLM reasoning
* Context-aware execution

---

## 🚀 Getting Started

### Clone the Repository

```bash
git clone https://github.com/your-username/MCP_Hr_assist.git
cd MCP_Hr_assist
```

---

### Setup Environment Variables

Create a `.env` file:

```
CB_EMAIL=your_email@gmail.com
CB_EMAIL_PWD=your_app_password
```

⚠️ Use **App Password**, not your actual Gmail password.

---

### Run the MCP Server

```bash
python server.py
```

---

## 🤖 Example AI Workflow

### Onboarding Prompt

```
Onboard a new employee:
- Name: Rak Sharan
- Manager: John
```

### What Happens Internally

* ✅ Employee is added
* ✅ Email is triggered
* ✅ Manager is notified
* ✅ Tickets are created
* ✅ Meeting is scheduled
