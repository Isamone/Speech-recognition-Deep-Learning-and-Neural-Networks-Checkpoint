Speech-Enabled Chatbot
An interactive Streamlit web application that allows users to interact with a chatbot via text or speech. It leverages transformers for natural language understanding, NLTK for preprocessing, and SpeechRecognition to handle voice input.

📌 Features
🔊 Speech-to-Text conversion using Google's Speech Recognition API

💬 Question Answering with pre-trained transformer models from Hugging Face

📄 Loads knowledge from a custom text file (data_science_guide.txt)

🧠 Tokenizes and preprocesses data using NLTK

📥 Allows users to submit suggestions via sidebar

🖼️ Clean and intuitive Streamlit interface

🚀 How to Run
1. Clone the Repository
bash
Copy
Edit

2. Install Required Libraries
bash
Copy
Edit
pip install streamlit speechrecognition nltk transformers
📝 Note: You may need to install pyaudio for microphone access on some systems:

bash
Copy
Edit
pip install pyaudio
3. Download NLTK Resources
python
Copy
Edit
import nltk
nltk.download("punkt")
4. Run the App
bash
Copy
Edit
streamlit run chatbot.py
🧠 How It Works
Loads a text corpus from data_science_guide.txt

Preprocesses it using nltk.word_tokenize()

Accepts user input (text or voice)

Transcribes speech (if selected)

Uses a Hugging Face transformer model (question-answering) to find the most relevant answer

Displays and stores the full conversation

📂 File Structure
bash
Copy
Edit
├── chatbot.py                  # Main Streamlit app
├── data_science_guide.txt      # Knowledge base for chatbot
├── suggestions.txt             # Stores user feedback
└── README.md                   # Project documentation
