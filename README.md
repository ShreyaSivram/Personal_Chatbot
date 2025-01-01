# Personal_Chatbot
**Your own ChatGPT**
This repository contains a Streamlit-based web application that interacts with the Gemini Pro language model to provide responses to user queries. The application integrates the Google Generative AI API and demonstrates the use of streamlit, python-dotenv, and google-generativeai packages.

**Features**

**Streamlit UI:** An intuitive interface for user input and response display.

**Gemini Pro Integration:** Uses the google-generativeai library to connect to the Gemini Pro LLM.

**Chat History:** Maintains a session-based chat history for reference.

**Prerequisites**

Ensure you have the following installed:

Python 3.10 or higher

A Google API key with access to the Gemini Pro model

**Installation**

Clone the repository:

git clone https://github.com/ShreyaSivram/Personal_Chatbot.git
cd repo-name

**Set up a virtual environment:**

python3 -m venv .venv
source .venv/bin/activate

**Install dependencies:**

pip install -r requirements.txt

**Configure environment variables:**
Create a .env file in the project root with the following content:

GOOGLE_API_KEY=your-google-api-key

**Usage**

**Run the Streamlit application:**

streamlit run qachat.py

Open the provided local URL (usually http://localhost:8501) in your web browser.

Enter your questions in the input box and click "Ask the question" to receive responses from the Gemini LLM.

**Code Overview**

Main Files:

**qachat.py:** The main script containing the Streamlit app code.

Key Libraries:

**dotenv:** Loads environment variables from a .env file.

**streamlit:** Provides the UI framework for the web app.

**google-generativeai:** Handles the interaction with Gemini Pro.

**Functionality:**

get_gemini_response(question):

Loads the Gemini Pro model.

Sends user queries to the model and streams the response.

**Requirements**

Ensure the following Python packages are installed:

streamlit

google-generativeai

python-dotenv

To install these dependencies:

pip install -r requirements.txt

**Troubleshooting**

Environment Variable Issues:
Ensure the .env file is correctly set up with your Google API key.

**Dependency Errors:**
Run the following command to reinstall dependencies:

pip install --force-reinstall -r requirements.txt

**Port Conflict:**
If the default Streamlit port (8501) is in use, specify a different port:

streamlit run qachat.py --server.port=8502

License

This project is licensed under the MIT License. See the LICENSE file for details.

Contributing

Contributions are welcome! Please submit a pull request or open an issue for any suggestions or bugs.
