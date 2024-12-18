# Gemini Application

A Streamlit-based application that integrates with Google Gemini Pro Vision to analyze images and answer questions about uploaded invoices.

---

## Features

- Upload an image (e.g., an invoice) in **JPEG** or **PNG** format.
- Enter a text prompt to guide the analysis.
- Uses Google Gemini Pro Vision (via Gemini-1.5-Flash model) for intelligent image processing and content generation.
- Outputs detailed responses based on the provided invoice and prompt.

---

## Requirements

### Prerequisites

Before running this project, ensure you have the following installed:

- **Python 3.8 or above**
- **pip** (Python package manager)

### Python Libraries

The following libraries are used in this project:

- `streamlit` – For building the web app.
- `Pillow` – For handling image uploads.
- `python-dotenv` – For loading API keys from environment variables.
- `google-generativeai` – For accessing Google Gemini Pro Vision models.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/gemini-application.git
   cd gemini-application

2. Set up a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt

4. Obtain a Google API key:
- Visit the [Google Cloud Console](https://console.cloud.google.com/).
- Create a new project (if you don’t have one).
- Enable the Google Generative AI API in your project.
- Generate an API key under APIs & Services > Credentials.

5. Save the API key in a .env file in the project root directory:
   ```bash
   GOOGLE_API_KEY = "your_google_api_key"

---

## Usage

1. Run the Streamlit application:
    ```bash
    streamlit run app.py

2. Open the app in your web browser (it will typically run on http://localhost:8501).

3. Follow these steps in the app:
- Upload an image (e.g., an invoice).
- Enter a descriptive prompt.
- Click on the "Tell me about the invoice" button to receive a response.

---

## File Structure
   .
    ```plaintext
    
    ├── app.py                # Main Streamlit app script
    ├── requirements.txt      # Dependencies for the project
    ├── .env                  # Environment file for storing the API key
    ├── README.md             # Project documentation

---

## Notes
- This application requires a valid Google API key for the Gemini Pro Vision service.
- Ensure that the uploaded images are clear and in supported formats (JPG, JPEG, or PNG) for optimal results.

---

## License
- This project is licensed under the MIT License. See the LICENSE file for details.

---

## Acknowledgments
- [Google Generative AI](https://developers.generativeai.google) for the Gemini Pro Vision API.
- [Streamlit](https://streamlit.io/) for building intuitive Python-based web applications.

