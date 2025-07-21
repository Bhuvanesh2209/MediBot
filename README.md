# MediBot
# Medical Chatbot 🤖

An AI-powered medical chatbot built with Streamlit that provides health advice, cures, and personalized tips based on user input. The chatbot uses semantic similarity matching with Sentence Transformers to understand user queries and Google Translate to support multiple languages.

---

## Features

- **Semantic Search:** Uses `sentence-transformers` to find the best matching disease and corresponding cure from a dataset.
- **Fallback Responses:** Provides predefined responses for common symptoms like fever, cough, headache, and cold.
- **Personalized Health Tips:** Offers categorized health tips related to sleep, energy, stress, and general wellness.
- **Multilingual Support:** Translates responses into multiple languages using Google Translate API.
- **Interactive UI:** Simple and intuitive interface built with Streamlit.


---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Bhuvanesh2209/MediBot
   cd medical-chatbot
Create and activate a virtual environment:

bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Usage
Run the Streamlit app:

bash
Copy
Edit
streamlit run chat.py
Enter your medical query in the input box.

Select your preferred language from the dropdown.

Click Get Response to receive suggested cures or advice.

Click Get a Personalized Health Tip for wellness tips.

Dataset
Your chatbot relies on a CSV dataset with the following columns:

disease: Name or description of the disease.

cure: Corresponding recommended cure or advice.

Make sure your dataset CSV file path is correctly set in chat.py:

python
Copy
Edit
df = pd.read_csv('/path/to/your/dataset - Sheet1.csv')
Dependencies
streamlit

pandas

sentence-transformers

googletrans==4.0.0-rc1

You can install all dependencies via:

bash
Copy
Edit
pip install streamlit pandas sentence-transformers googletrans==4.0.0-rc1
