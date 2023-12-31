# Chatbot Project 

chatbot project that utilizes Django, a web framework, and Bootstrap, a CSS framework, along with the OpenAI API to create a chatbot interface.

## Project Overview

The chatbot project aims to provide an interactive chat interface where users can have conversations with an AI-powered chatbot. Django is used as the backend web framework to handle the server-side functionality, while Bootstrap is used for designing the frontend user interface.

The project integrates the OpenAI API, specifically the GPT-3.5 language model, to generate responses to user queries and simulate a conversation. The OpenAI API allows the chatbot to learn and improve its responses over time.

## Prerequisites

Before running the project, make sure you have the following prerequisites installed:

- Python (version 3.7 or higher)
- Django (version 3.2 or higher)
- Bootstrap (version 4 or higher)
- OpenAI Python SDK

### Home page
![website interface0](Screenshots/screencapture-127-0-0-1-8000-2023-07-04-19_47_24.png)
### Login page
![website interface1](Screenshots/screencapture-127-0-0-1-8000-login-2023-07-01-19_26_40.png)
### Home page
![website interface2](Screenshots/screencapture-127-0-0-1-8000-2023-07-04-19_47_49.png)
### Register page
![website interface3](Screenshots/screencapture-127-0-0-1-8000-register-2023-07-01-19_26_55.png)

## Project Setup

Follow the steps below to set up the project:

1. Clone the project repository from the GitHub repository:

   ```
   git clone https://github.com/KamelTouati/chatbot
   ```

2. Navigate to the project directory:

   ```
   cd django-chatbot
   ```

3. Create a virtual environment to isolate the project dependencies:

   ```
   python3 -m venv env
   ```

4. Activate the virtual environment:

   - For Windows:

     ```
     env\Scripts\activate
     ```

   - For macOS/Linux:

     ```
     source env/bin/activate
     ```

5. Install the project dependencies:

   ```
   pip install -r requirements.txt
   ```

6. Obtain an API key from OpenAI by following their documentation on how to create an account and obtain the API key.

7. Replace the placeholder API key in the `settings.py` file with your OpenAI API key:

   ```python
   OPENAI_API_KEY = 'your-api-key'
   ```

## Running the Project

To run the project, follow these steps:

1. Activate the virtual environment (if not already activated):

   - For Windows:

     ```
     env\Scripts\activate
     ```

   - For macOS/Linux:

     ```
     source env/bin/activate
     ```

2. Start the Django development server:

   ```
   python manage.py runserver
   ```

3. Open a web browser and navigate to `http://localhost:8000` to access the chatbot interface.

## Project Structure

The project structure is organized as follows:

```
chatbot-project/
├── chatbot/
│   ├── migrations/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
├── django_chatbot/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── templates/
├── env/
├── manage.py
└── requirements.txt
```

- The `chatbot/` directory contains the Django app responsible for handling the chatbot functionality.
- The `templates/` directory contains HTML templates for rendering the chatbot interface.
- The `settings.py` file contains project settings, including the OpenAI API key configuration.
- The `urls.py` files define the project's URL routing.
- The `views.py` file contains the Django views that handle user requests and generate responses using the

