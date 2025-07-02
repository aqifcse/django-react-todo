# django-react-todo

A full-stack Todo application using Django (REST API) for the backend and React (Redux, Hooks) for the frontend.

---

## Features

- Add, edit, delete, and filter todos
- Mark todos as complete/incomplete
- Persistent storage with Django and SQLite
- Modern React UI with Redux Toolkit


## Backend Setup (Django)

1. **Install dependencies:**
    ```bash
    cd backend
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

2. **Apply migrations:**
    ```bash
    python manage.py migrate
    ```

3. **Run the backend server:**
    ```bash
    python manage.py runserver
    ```
    The API will be available at `http://localhost:8000/api/todos/`.

---

## Frontend Setup (React)

1. **Install dependencies:**
    ```bash
    cd ../frontend
    npm install
    ```

2. **Start the React development server:**
    ```bash
    npm start
    ```
    The app will be available at `http://localhost:3000`.

---

## Usage

- Add a task using the input field and "Add task" button.
- Edit or delete tasks using the respective buttons.
- Filter tasks by "complete" or "incomplete" status.

---

## API Endpoints

- `GET    /api/todos/` — List all todos
- `POST   /api/todos/` — Create a new todo
- `PATCH  /api/todos/<id>/` — Update a todo (title, description, completed)
- `DELETE /api/todos/<id>/` — Delete a todo

---

## Environment Variables

- You can set up a `.env` file in the backend for Django secrets.
- For the frontend, if you want to use a custom backend URL, create a `.env` file in `/frontend`:
    ```
    REACT_APP_API_BASE_URL=http://localhost:8000
    ```

---

## License

MIT License

---
