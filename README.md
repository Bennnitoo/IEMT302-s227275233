Chatbot Idea: Campus Info Assistant

Problem Addressed:
Many students struggle to quickly find information about campus services, lecture schedules, and general university updates. This chatbot can help answer common questions, guide students, and provide links or instructions for further actions.

Key Features:

Answer questions about lecture schedules, campus hours, or locations.

Provide contact information for departments (IT, library, administration).

Give reminders about upcoming events or deadlines.

Handle simple small-talk or greetings.

Use Spacy NLP to understand intent from natural language input.

Limitations:

Cannot understand queries outside predefined intents.

Misinterprets complex or ambiguous questions.

May fail to respond if a student uses slang or very casual language outside of its training examples.

Setup Instructions

Clone the repository

git clone <your-repo-url>
cd telegram-campus-bot


Create and activate a virtual environment

python -m venv venv
# Linux / Mac
source venv/bin/activate
# Windows
venv\Scripts\activate


Install dependencies

pip install -r requirements.txt


Download Spacy language model

python -m spacy download en_core_web_sm


Run the bot

python bot.py


Interact with the bot on Telegram

Start a chat with your bot using its token.

Try sample queries:

“When is the library open?”

“Who can I contact for IT support?”

“What lectures are today?”

Verifying Functionality

Send queries matching the intents listed in intents.json.

Verify that the bot responds accurately.

Test unexpected input to see fallback behavior and logging.
