# Chatbot Application

This project is a simple chatbot application built with a Vue.js frontend and a Flask backend.

## Requirements Specifications

-   **Frontend:** Vue.js
-   **Backend:** Flask (Python)
-   **Database:** MongoDB (To be implemented)
-   **DevOps:** Docker and Jenkins (Future Enhancement)
-   **NLP/LLM:** Llama or Hugging Face (Future Enhancement)
-   **Proxy Server:** NGINX (Future Enhancement)

## Project Structure
chatbot-app/
├── backend/ # Flask backend
│ ├── app/
│ │ ├── init.py # Flask app initialization
│ │ ├── routes.py # Flask routes
│ │ └── chatbot.py # Chatbot logic (placeholder)
│ ├── venv/ # Python virtual environment
│ ├── config.py # Configuration file (placeholder)
│ ├── requirements.txt # Python dependencies
│ └── run.py # Entry point for Flask app
├── frontend/ # Vue.js frontend
│ ├── src/
│ │ ├── components/
│ │ │ └── HelloWorld.vue # Vue Hello World component
│ │ ├── App.vue # Main Vue app file
│ │ └── main.js # Vue entry point
│ ├── public/ # Static files (placeholder)
│ ├── package.json # Node.js dependencies
│ └── vite.config.js # Vite configuration
└── README.md # Documentation


## Getting Started

### Prerequisites

Make sure you have the following installed:

-   Node.js (v18+) and npm
-   Python 3.12+
-   pip (Python package installer)

### Cloning the Repository
git clone [<repository-url>](https://github.com/Srivastava-Team1/canes-app.git)
cd chatbot-app


### Backend Setup (Flask)

1.  Navigate to the backend directory:

    ```
    cd backend
    ```

2.  Create a virtual environment:

    ```
    python3.12 -m venv venv
    ```

3.  Activate the virtual environment:

    -   **Linux/Mac:**

    ```
    source venv/bin/activate
    ```

    -   **Windows:**

    ```
    .\venv\Scripts\activate
    ```

4.  Install the dependencies:

    ```
    pip install -r requirements.txt
    ```

5.  Run the Flask application:

    ```
    python app/routes.py
    ```

    The backend server will start at `http://127.0.0.1:5000`.

### Frontend Setup (Vue.js)

1.  Navigate to the frontend directory:

    ```
    cd ../frontend
    ```

2.  Install the dependencies:

    ```
    npm install
    ```

3.  Run the Vue.js application:

    ```
    npm run dev
    ```

    The frontend development server will start at `http://127.0.0.1:3000`.

### Accessing the Application

-   **Frontend:** Open your browser and go to `http://127.0.0.1:3000` to see the Vue.js application.
-   **Backend:** Open your browser and go to `http://127.0.0.1:5000` to see the Flask backend response.

## Configuration

-   Backend configurations can be set in the `backend/config.py` file.  (To be implemented)
-   Frontend configurations are in `frontend/vite.config.js`.

## Future Enhancements

-   Implement MongoDB integration.
-   Set up Docker and Jenkins for DevOps.
-   Integrate NLP/LLM models (Llama or Hugging Face).
-   Configure NGINX as a proxy server.

---
