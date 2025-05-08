🌍 Identification of Place Names from a Natural Language Sentence



This project extracts geographical place names (cities, countries, landmarks, etc.) from natural language sentences using NLP techniques. It's useful for applications in geographic information systems (GIS), data mining, chatbots, and more.

🧠 What It Does
Given a sentence like:

"I traveled from Paris to Berlin and then visited the Eiffel Tower."

The model extracts:

css
Copy
Edit
["Paris", "Berlin", "Eiffel Tower"]
🔧 Features
Named Entity Recognition (NER) to extract location entities

Supports input as plain text or batch files

Uses spaCy, NLTK, or custom models

(Optional) Can integrate with geocoding APIs to fetch coordinates

🛠️ Technologies Used
Python 3.10+

NLP Libraries:

spaCy

NLTK

Optional:

GeoPy or Google Maps API

📁 Project Structure
bash
Copy
Edit
place-name-extractor/
├── main.py                # Main script to process text
├── utils.py               # Helper functions
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
└── sample_inputs.txt      # Example sentences
🚀 Getting Started
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/place-name-extractor.git
cd place-name-extractor
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the extractor:

bash
Copy
Edit
python main.py
💬 Example Usage
python
Copy
Edit
from extractor import extract_places

text = "I was in Tokyo last week and will visit New York next month."
print(extract_places(text))
Output:

css
Copy
Edit
['Tokyo', 'New York']
📦 API Integration (Optional)
You can link with services like Google Maps API to fetch details:

python
Copy
Edit
from geopy.geocoders import Nominatim

geolocator = Nominatim(user_agent="geoapi")
location = geolocator.geocode("Paris")
print(location.latitude, location.longitude)
📌 Future Enhancements
Use transformer-based models (BERT, RoBERTa) for improved accuracy

Multilingual support

Web interface for demo

📜 License
This project is licensed under the MIT License.
