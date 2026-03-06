# AI Tweet Generator Workflow

An AI-powered tweet generation workflow built using **n8n automation** and **Groq LLM inference**.  
The workflow captures user input through a form trigger, processes it using a language model, and returns AI-generated tweet content.

This project demonstrates how **large language models can be integrated into low-code automation pipelines** to build AI-powered content generation tools.

---

# Project Overview

This workflow implements an automated pipeline for generating tweet-style content using an LLM integrated within **n8n**.

The system collects input through a form interface, sends it to a **Basic LLM Chain**, and uses a **Groq Chat Model** to generate tweet content.  
The generated response is then returned through the workflow output node.

### Core Components

- Form Submission Trigger  
- Basic LLM Chain  
- Groq Chat Model  
- Generated Output Node  

---

# Workflow Details

## Form Submission Trigger
- Captures user input through an n8n form interface  
- Initiates workflow execution  
- Passes collected input to the LLM processing stage  

## Basic LLM Chain
- Processes the input prompt  
- Sends the prompt to the connected language model  
- Generates tweet-style content  

## Groq Chat Model
- Provides the language model used for generation  
- Performs LLM inference  
- Returns generated response  

## Output Node
- Returns generated tweet content  
- Completes workflow execution  

---

# 🖥 Workflow Interface

The workflow runs inside the **n8n automation editor**.

### Features

- Interactive form-based input  
- AI-generated tweet output  
- Real-time workflow execution  
- Node-based workflow architecture  

Screenshots of the workflow structure and configuration are included in the repository.

---

# 🛠 Tech Stack

- n8n  
- Groq LLM API  
- Basic LLM Chain  
- Workflow Automation  

---

# Repository Structure

```
N8N-AI-Tweet-Generator
│
├── workflow.json
├── screenshots
│
└── README.md
```

---

# ▶ How to Run

## 1. Install Node.js

Make sure **Node.js (v18 or higher)** is installed.

Download from:  
https://nodejs.org

---

## 2. Install n8n

Install n8n globally using npm:

```bash
npm install -g n8n
```

Start the n8n server:

```bash
n8n start
```

Open the editor in your browser:

```
http://localhost:5678
```

---

## 3. Import Workflow

1. Open the n8n editor  
2. Click **Import Workflow**  
3. Upload the workflow file from this repository  
4. Save the workflow  

---

## 4. Configure Groq Credentials

1. Create an account on **Groq**  
2. Generate an **API Key**  
3. Add the API key in **n8n Credentials**  
4. Connect the credentials to the **Groq Chat Model node**

---

## 5. Run the Workflow

1. Trigger the **Form Submission node**  
2. Enter the required input  
3. The LLM chain processes the prompt  
4. Generated tweet content is returned as output  

---

