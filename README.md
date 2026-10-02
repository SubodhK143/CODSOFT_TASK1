# 🤖 Rule-Based Chatbot using Python

A simple **rule-based chatbot built with Python** that interacts with users through the command line. The chatbot recognizes basic keywords and provides predefined responses for greetings, introductions, well-being questions, and exit commands.

This project is ideal for beginners learning **Python functions, conditional statements, loops, string handling, and user input**.

---

## 📌 Project Overview

The chatbot uses a simple **keyword-matching approach** to understand user messages.

For example:

* User: `Hello`

* Chatbot: `Hello How can I assist you?`

* User: `What is your name?`

* Chatbot: `I'm a simple chatbot. I don't have a name, but you can call me Chatbot.`

* User: `Bye`

* Chatbot: `Goodbye. Have a great day.`

The chatbot continues interacting with the user until `bye` or `goodbye` is entered.

---

## ✨ Features

* 🤖 Simple rule-based chatbot
* 💬 Interactive command-line conversation
* 👋 Greeting recognition
* 🏷️ Basic chatbot identity response
* 😊 "How are you?" response
* 👋 Goodbye handling
* 🔤 Case-insensitive user input
* 🐍 Built completely with Python
* ⚡ Lightweight and easy to understand

---

## 🛠️ Technologies Used

| Technology                | Purpose               |
| ------------------------- | --------------------- |
| 🐍 Python                 | Programming language  |
| 🔤 String Handling        | Process user input    |
| 🔀 Conditional Statements | Match user queries    |
| 🔁 While Loop             | Maintain conversation |
| ⌨️ CLI                    | User interaction      |

---

## 📂 Project Structure

```text
rule-based-chatbot/
│
├── chatbot.py
└── README.md
```

---

## ⚙️ How It Works

The chatbot follows a simple processing flow:

```text
        ┌─────────────────┐
        │   Start Chatbot │
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │  Get User Input │
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │ Convert to Lower│
        │      Case       │
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │ Match Keywords  │
        └────────┬────────┘
                 │
          ┌──────┴───────┐
          ▼              ▼
    Keyword Found    No Match
          │              │
          ▼              ▼
    Return Response  Default Response
          │              │
          └──────┬───────┘
                 ▼
        ┌─────────────────┐
        │ Continue Chat?  │
        └────────┬────────┘
                 │
          ┌──────┴──────┐
          │             │
         Yes            No
          │             │
          ▼             ▼
      Continue          Exit
```

---

## 💻 Code

Create a file named `chatbot.py`:

```python
def chatbot_response(user_input):
    user_input = user_input.lower()

    if "hello" in user_input or "hi" in user_input:
        return "Hello How can I assist you?"

    elif "name" in user_input:
        return "I'm a simple chatbot. I don't have a name, but you can call me Chatbot."

    elif "who are you" in user_input:
        return "I am a chatbot designed to help with basic queries. What would you like to know?"

    elif "bye" in user_input or "goodbye" in user_input:
        return "Goodbye! Have a great day."

    elif "how are you" in user_input:
        return "I'm just a program, so I don't have feelings, but I'm fine."

    else:
        return "I'm not sure how to respond to that. Can you ask something else."


def main():
    print("Chatbot: Hi there. Type 'bye' to exit.")

    while True:
        user_input = input("You: ")

        if user_input.lower() in ["bye", "goodbye"]:
            print("Chatbot: Goodbye. Have a great day.")
            break

        response = chatbot_response(user_input)
        print(f"Chatbot: {response}")


if __name__ == "__main__":
    main()
```

---

## 🚀 How to Run

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/rule-based-chatbot.git
```

### 2️⃣ Navigate to the Project

```bash
cd rule-based-chatbot
```

### 3️⃣ Run the Chatbot

```bash
python chatbot.py
```

Or, depending on your Python installation:

```bash
python3 chatbot.py
```

---

## 🧪 Example Conversation

```text
Chatbot: Hi there. Type 'bye' to exit.

You: Hello
Chatbot: Hello How can I assist you?

You: What is your name?
Chatbot: I'm a simple chatbot. I don't have a name, but you can call me Chatbot.

You: Who are you?
Chatbot: I am a chatbot designed to help with basic queries. What would you like to know?

You: How are you?
Chatbot: I'm just a program, so I don't have feelings, but I'm fine.

You: Bye
Chatbot: Goodbye. Have a great day.
```

---

## 🧠 Concepts Demonstrated

This project demonstrates several fundamental Python concepts:

* Variables
* Functions
* `if / elif / else`
* `while` loops
* User input
* String manipulation
* `.lower()` method
* Keyword matching
* `return` statements
* `break` statement
* Python `__name__ == "__main__"` pattern

---

## 🔄 Possible Improvements

The current chatbot is intentionally simple. It can be extended with:

* 🧠 More conversation patterns
* 🗂️ Response dictionaries
* 🔍 Improved keyword matching
* 🎯 Intent detection
* 🧹 Input validation
* 💾 Conversation history
* 🧪 Unit testing
* 🌐 Flask/FastAPI web interface
* 🐳 Docker containerization
* ☁️ AWS deployment
* 🤖 Integration with an AI/LLM API

---

## 🎯 Learning Objective

The primary objective of this project is to understand how a basic chatbot can process user input and generate responses using predefined rules.

It provides a foundation for progressing from **rule-based chatbots → NLP → Machine Learning → Generative AI applications**.

---

## 📈 Future Architecture

```text
Rule-Based Chatbot
       │
       ▼
Keyword Matching
       │
       ▼
Intent Detection
       │
       ▼
NLP / Machine Learning
       │
       ▼
LLM / Generative AI
       │
       ▼
Production AI Application
```

---

## 👨‍💻 Author

**Subodh Kumar**

🐍 Python | ☁️ AWS | 🚀 DevOps | 🤖 AI & Cloud

🔗 **GitHub:** https://github.com/SubodhK143

🔗 **LinkedIn:** https://www.linkedin.com/in/subodh-kumar-aws-certified/

---

## ⭐ Support

If you find this project useful for learning Python or chatbot fundamentals, consider giving the repository a ⭐ **Star**.

**Happy Co**
