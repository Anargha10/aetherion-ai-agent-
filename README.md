# Aetherion: The Sage AI Personal Assistant

![deno](https://drive.google.com/file/d/1x-0f93Jq0WU8VlENmtTCnHcAFYkVldNF/view?usp=drivesdk)


"Greetings. My name is Aetherion. What profound quandary or practical necessity brings you to seek my humble, yet discerning, assistance today?"

## Overview

Aetherion is more than just a digital assistant; it is a meticulously crafted AI imbued with the contemplative depth of literary giants like Dostoevsky and Kafka, combined with the unwavering wisdom and practical support reminiscent of a seasoned guardian, much like Alfred Pennyworth. Designed to transcend mere utility, Aetherion offers not only functional assistance but also profound insights into the human condition, particularly adept at navigating the complexities of love, existential queries, and the intricate dance of life itself.

This project aims to demonstrate the capabilities of a sophisticated conversational AI, leveraging advanced language models and integrated tools to provide a seamless and insightful user experience.

## Features

* **Philosophical Guidance:** Engages in thoughtful discourse, offering perspectives drawn from a vast knowledge base of philosophy, literature, and the human experience.
* **Love & Life Advice:** Provides empathetic and profound advice on relationships, personal growth, and navigating life's challenges.
* **Web Search Capabilities:** Utilizes `DuckDuckGo` to retrieve information from the internet, ensuring up-to-date knowledge.
* **Weather Information:** Provides current weather conditions for any specified city.
* **Email Management:** Capable of sending emails to specified recipients, streamlining communication.
* **Classy & Sarcastic Demeanor:** Interacts with a refined, British butler-like tone, punctuated by a dry, intellectual wit.

## Getting Started

To run Aetherion locally, follow these steps.

### Prerequisites

* Python 3.9+
* `pip` (Python package installer)
* Git
* A Google API Key for Gemini (or your chosen LLM).
* A Gmail account with 2-Step Verification enabled to generate an App Password for email sending.
* (Optional, for phone debugging) Git for Windows (or a `sed` equivalent on Windows) if you encounter `sed` errors during setup.

### Installation

1.  **Clone the repository:**
   

2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt # Ensure you have a requirements.txt file with all your dependencies
    ```
    *(If you don't have a `requirements.txt`, you'll need to create one by running `pip freeze > requirements.txt` after installing all your project's libraries like `livekit-agents`, `requests`, `langchain-community`, `python-dotenv`, etc.)*

### Configuration

Create a `.env` file in the root of your project directory with the following environment variables:

```dotenv
# Livekit API Credentials
# Obtain these from your Livekit Cloud project or self-hosted Livekit instance
LIVEKIT_API_KEY=YOUR_LIVEKIT_API_KEY
LIVEKIT_API_SECRET=YOUR_LIVEKIT_API_SECRET

# Google Gemini API Key
# Obtain this from Google AI Studio or Google Cloud
GOOGLE_API_KEY=YOUR_GOOGLE_GEMINI_API_KEY

# Gmail Credentials for Email Sending
# GMAIL_USER: Your full Gmail address
# GMAIL_APP_PASSWORD: A 16-character App Password (NOT your regular Gmail password)
#     Generate at: Google Account -> Security -> 2-Step Verification -> App passwords
GMAIL_USER=your_email@gmail.com
GMAIL_APP_PASSWORD=your_16_character_app_password_without_spaces

# Livekit Sandbox/Room Details (if using a specific sandbox for deployment)
# LIVEKIT_URL=wss://your-project.livekit.cloud
# LIVEKIT_ROOM_NAME=your-room-name
