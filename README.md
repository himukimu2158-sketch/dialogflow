# 💰 Finance Assistant Advanced – AI Chatbot using Dialogflow

![Dialogflow](https://img.shields.io/badge/Dialogflow-Essentials-orange)
![HTML](https://img.shields.io/badge/Frontend-HTML-blue)
![JavaScript](https://img.shields.io/badge/JavaScript-Enabled-yellow)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

# 📌 Introduction

Finance Assistant Advanced is an AI-powered chatbot developed using Dialogflow Essentials.  
The chatbot helps users perform financial activities such as:

- 🏦 Loan Eligibility Checking
- 📊 EMI Calculation
- 📈 Investment Guidance
- 💡 Risk-based Financial Advice

The chatbot uses Natural Language Processing (NLP) to understand user queries and respond intelligently.

---

# 🎯 Objectives

The main objectives of this project are:

- Automate financial guidance
- Reduce manual financial consultation
- Provide instant financial support
- Improve customer interaction experience
- Demonstrate AI chatbot integration using Dialogflow

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Dialogflow Essentials | NLP & Chatbot Development |
| Google Cloud Platform | Backend Services |
| HTML5 | Frontend |
| CSS3 | Styling |
| JavaScript | Integration |
| Dialogflow Messenger | Chat Interface |

---

# 🚀 Features

## ✅ Loan Eligibility Checking

The chatbot can determine approximate loan eligibility based on user salary.

### Example Queries

```text
I earn 50000 can I get loan?
My salary is 70000
Can I get loan of 20 lakh?
Loan eligibility for 60000 income
```

### Sample Response

```text
Based on your income, you may be eligible for a loan between ₹12–15 lakhs.
```

---

# 📊 EMI Calculation

The chatbot calculates EMI based on:
- Principal Amount
- Interest Rate
- Loan Tenure

---

## EMI Formula

\[
EMI = \frac{P \times R \times (1+R)^N}{(1+R)^N - 1}
\]

Where:

| Symbol | Meaning |
|---|---|
| P | Principal Loan Amount |
| R | Monthly Interest Rate |
| N | Loan Duration in Months |

---

# 📈 Investment Advice System

The chatbot provides investment guidance based on risk level.

| Risk Level | Suggestions |
|---|---|
| Low | FD, PPF, Government Bonds |
| Medium | Mutual Funds |
| High | Stocks, Crypto, Equity |

---

# 🧠 Dialogflow Intents

The chatbot contains multiple intents.

| Intent Name | Purpose |
|---|---|
| Default Welcome Intent | Welcome Message |
| Default Fallback Intent | Unknown Query Handling |
| EMI_Calculation | EMI Estimation |
| Investment_Advice_Intent | Basic Investment Advice |
| Investment_Advice_Advanced | Risk-based Suggestions |
| Loan_Eligibility_Advanced | Loan Eligibility |

---

# 📸 Screenshots

---

## 🔹 Dialogflow Messenger Integration

![Google Form](integration.png)

---

## 🔹 Intents Created

![Google Form](intents.png)

---

## 🔹 Training Phrases

![Google Form](training_phrase.png)

---

## 🔹 Parameters Configuration

![Google Form](parameter.png)

---

## 🔹 Chatbot Output

![Google Form](chatbox.png)

---

# 🌐 Frontend Code

# 📄 index.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Finance Assistant Advanced</title>

    <link rel="stylesheet" href="css/style.css">
</head>
<body>

    <div class="container">
        <h1>💰 Finance Assistant Advanced</h1>
        <p>AI Powered Financial Chatbot using Dialogflow</p>

        <div class="features">
            <div class="card">
                <h2>🏦 Loan Eligibility</h2>
                <p>Check loan eligibility based on salary.</p>
            </div>

            <div class="card">
                <h2>📊 EMI Calculator</h2>
                <p>Calculate EMI instantly.</p>
            </div>

            <div class="card">
                <h2>📈 Investment Advice</h2>
                <p>Get investment guidance based on risk level.</p>
            </div>
        </div>
    </div>

    <!-- Dialogflow Messenger -->
    <script src="https://www.gstatic.com/dialogflow-console/fast/messenger/bootstrap.js?v=1"></script>

    <df-messenger
      intent="WELCOME"
      chat-title="Finance_Assistant_Advanced"
      agent-id="YOUR_AGENT_ID"
      language-code="en">
    </df-messenger>

</body>
</html>
```

---

# 🎨 CSS Styling

# 📄 css/style.css

```css
body {
    margin: 0;
    padding: 0;
    background: #f4f7fc;
    font-family: Arial, sans-serif;
}

.container {
    text-align: center;
    padding: 50px;
}

h1 {
    color: #1e3c72;
    font-size: 42px;
}

p {
    color: #555;
    font-size: 18px;
}

.features {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 40px;
}

.card {
    background: white;
    padding: 25px;
    width: 250px;
    border-radius: 12px;
    box-shadow: 0px 4px 12px rgba(0,0,0,0.1);
}

.card h2 {
    color: #2a5298;
}
```

---

# ⚡ JavaScript

# 📄 js/script.js

```javascript
console.log("Finance Assistant Advanced Loaded Successfully");

function welcomeMessage() {
    alert("Welcome to Finance Assistant Advanced");
}

welcomeMessage();
```

---

# 🤖 Dialogflow Messenger Integration Code

```html
<script src="https://www.gstatic.com/dialogflow-console/fast/messenger/bootstrap.js?v=1"></script>

<df-messenger
  intent="WELCOME"
  chat-title="Finance_Assistant_Advanced"
  agent-id="YOUR_AGENT_ID"
  language-code="en">
</df-messenger>
```

---

# 🔧 Steps to Setup Project

---

## Step 1: Create Dialogflow Agent

1. Open Dialogflow Console
2. Click Create Agent
3. Enter:
   - Agent Name
   - Default Language
   - Time Zone

---

## Step 2: Create Intents

Create the following intents:

```text
Default Welcome Intent
Default Fallback Intent
EMI_Calculation
Investment_Advice_Intent
Investment_Advice_Advanced
Loan_Eligibility_Advanced
```

---

## Step 3: Add Training Phrases

Example:

```text
I earn 50000
Can I get loan
I want investment advice
Calculate EMI
```

---

## Step 4: Configure Parameters

| Parameter | Entity |
|---|---|
| income | @sys.number |
| loan_amount | @sys.number |
| risk_level | @sys.any |

---

## Step 5: Add Responses

Example:

```text
You may be eligible for a loan based on your income.
```

---

## Step 6: Enable Dialogflow Messenger

Go to:

```text
Integrations → Dialogflow Messenger
```

Enable the integration.

---

# 📈 Future Enhancements

- ✅ Voice-enabled chatbot
- ✅ Real-time Banking APIs
- ✅ Firebase Database Integration
- ✅ User Authentication
- ✅ Multi-language Support
- ✅ AI-based Financial Predictions
- ✅ Personalized Financial Planning

---

# 🔒 Security Features

- Input Validation
- Secure Dialogflow Integration
- User Query Sanitization
- Cloud-based Deployment

---

# 📊 Advantages of Project

- Fast customer interaction
- 24/7 financial support
- User-friendly interface
- AI-based automation
- Easy integration into websites

---

# 📚 Learning Outcomes

By building this project, you can learn:

- Dialogflow NLP
- Chatbot Design
- Intent Management
- Entity Extraction
- Frontend Integration
- Conversational AI

---

# 👨‍💻 Author

## Himanshu Goyal

MBA Finance + AI Chatbot Developer

---

# 📄 License

This project is developed for educational and learning purposes.

---

# ⭐ Support

If you like this project:

⭐ Star the repository  
🍴 Fork the project  
📢 Share with others

---

# 🙌 Acknowledgement

Special thanks to:

- Google Dialogflow
- Google Cloud Platform
- Open Source Community

---
