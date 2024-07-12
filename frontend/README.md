# Notes App

This project is a full-stack web application that allows users to manage notes. It uses Django for the backend and React for the frontend. The application includes user authentication using JWT tokens, allowing users to register, log in, and manage their notes. The frontend is developed using React and Vite, and the backend is built with Django and Django REST framework.

## Features

- User authentication (register, login, logout) using JWT tokens
- Create, read, update, and delete notes
- Responsive and modern user interface
- RESTful API for notes management

## Technologies Used

- Frontend: React, Vite, Axios
- Backend: Django, Django REST framework, SimpleJWT
- Authentication: JWT tokens
- Styling: CSS

## Installation and Setup

### Prerequisites

- Node.js and npm
- Python 3.x
- Virtual environment (venv)

### Backend Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/notes-app.git
    cd notes-app/backend
    ```

2. **Create a virtual environment and activate it:**

    ```bash
    python -m venv env
    source env/bin/activate  # On Windows, use `env\Scripts\activate`
    ```

3. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Run the migrations:**

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5. **Start the backend server:**

    ```bash
    python manage.py runserver
    ```

### Frontend Setup

1. **Navigate to the frontend directory:**

    ```bash
    cd ../frontend
    ```

2. **Install the required packages:**

    ```bash
    npm install
    ```

3. **Start the frontend development server:**

    ```bash
    npm run dev
    ```

## Project Structure

```plaintext
notes-app/
│
├── backend/
│   ├── api/
│   │   ├── __init__.py
│   │   ├── admin.py
│   │   ├── apps.py
│   │   ├── models.py
│   │   ├── serializers.py
│   │   ├── urls.py
│   │   └── views.py
│   ├── backend/
│   │   ├── __init__.py
│   │   ├── asgi.py
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── wsgi.py
│   ├── db.sqlite3
│   ├── manage.py
│   └── requirements.txt
│
├── frontend/
│   ├── public/
│   │   ├── index.html
│   ├── src/
│   │   ├── api/
│   │   │   └── index.js
│   │   ├── components/
│   │   │   ├── Note.jsx
│   │   ├── pages/
│   │   │   ├── Home.jsx
│   │   │   ├── Login.jsx
│   │   │   ├── NotFound.jsx
│   │   │   ├── Register.jsx
│   │   ├── styles/
│   │   │   ├── Home.css
│   │   │   ├── Note.css
│   │   ├── App.jsx
│   │   ├── constants.js
│   │   ├── main.jsx
│   ├── .env
│   ├── package.json
│   └── vite.config.js
```

## Usage

1. **Register a new user:**
   Navigate to the registration page and create a new account.

2. **Login:**
   Use your credentials to log in. The application will authenticate you using JWT tokens.

3. **Create, Read, Update, and Delete Notes:**
   Once logged in, you can manage your notes. Create new notes, read existing ones, update them, or delete them.

## Issues and Troubleshooting

1. **Import Errors:**
   Ensure all file paths and import statements are correct. Check the project structure and make sure all necessary files exist.

2. **Token Handling:**
   If you encounter issues with token handling, ensure that the tokens are correctly set in local storage and that they are properly sent with each request.

3. **Clearing Cache:**
   If you face persistent issues, try clearing the npm cache, deleting the `node_modules` directory, and reinstalling dependencies.

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature/your-feature`)
6. Open a pull request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

Special thanks to all contributors and the open-source community for their valuable work and support.
