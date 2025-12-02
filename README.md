# **AI Workout Routine Builder 🏋️‍♂️**

A Python-based conversational agent that builds simple workout routines, tracks your progress, and explains exercises using AI.

**⚠️ WORK IN PROGRESS**

Please note that this project is currently in development. While the bot can handle conversation flow and explain specific exercises using the Anthropic API, **the external API integration for generating dynamic workout plans has not yet been implemented.**

Currently, the bot provides workouts from a static, hardcoded library of exercises and routine templates.

## **Features**

* **Interactive Chat Interface:** Simple command-line conversational flow.  
* **Customizable Difficulty:** Supports 'Beginner' and 'Intermediate' fitness levels.  
* **Time-Based Routines:** Generates routines based on available time (15, 30, or 45 minutes).  
* **AI-Powered Explanations:** Uses the Anthropic (Claude) API to provide detailed, beginner-friendly instructions for specific exercises.  
* **Progress Tracking:** Persists a simple workout count to a local workout\_count.txt file to track consistency.

## **Prerequisites**

* Python 3.7+  
* An Anthropic API Key

## **Installation**

1. Clone the repository or download the script.  
2. Install the required dependency:

pip install anthropic

## **Configuration**

You must set your Anthropic API key as an environment variable before running the script.

**Mac/Linux:**

export ANTHROPIC\_API\_KEY='your-api-key-here'

**Windows (Command Prompt):**

set ANTHROPIC\_API\_KEY=your-api-key-here

## **Usage**

Run the script directly from your terminal:

python workout\_builder.py

The script currently runs a main() function that simulates a conversation flow for demonstration purposes. To use it interactively, modify the main() function to accept user input via input().

## **Roadmap**

* \[ \] **Dynamic Workout Generation:** Replace the hardcoded self.routines dictionary with an API call to generate unique, non-repetitive workouts based on user constraints.  
* \[ \] **Interactive Mode:** Switch from the demo loop to a while True input loop for real-time chatting.  
* \[ \] **Profile Storage:** Save user level and preferences between sessions.
