<img width="1919" height="910" alt="Screenshot 2025-10-05 122009" src="https://github.com/user-attachments/assets/82da4f15-da76-4bde-8e16-a246eab2ee64" /># To-Do List Web Application

A comprehensive, full-stack To-Do list web application designed for personal productivity and built to showcase modern development skills.

---

## 🚀 Live Demo

**Try it here:**    [Live Demo](https://to-do-efso.onrender.com)

---

## Features

- **User Authentication:** Secure signup/login via Flask-Login, passwords hashed using Bcrypt.
- **Task Management:** Add, edit, delete, and toggle tasks (complete/incomplete).
- **Due Dates:** Set due dates for tasks, with automatic status categorization.
- **Dynamic Filtering:** Filter tasks by Overdue, Due Today, and Pending status.
- **User Isolation:** Each user has private access to their own tasks.
- **Responsive UI:** Modern design with Jinja2 templates and FontAwesome icons.
- **Built-in Flash Messages:** User feedback for every key action.
- **Cloud Database:** All data stored in a managed PostgreSQL instance (e.g., on Render).

---

## 🗂️ Project Folder Structure

```text
To-Do/
│
├── app.py                # Main Flask application
├── requirements.txt      # Python dependencies
├── Procfile              # For deployment platforms (like Heroku/Render)
├── .gitignore
├── create_tables.py
│
├── templates/            # Jinja2 HTML templates
│   ├── index.html
│   ├── login.html
│   ├── signup.html
│   ├── tasks.html
│   ├── about.html
│   ├── base.html
│   ├── edit_task.html
│   ├── privacy.html
│
├── static/               # Static files (CSS, JS, images)
│   ├── style.css
│   ├── favicon.png
│   └── ... (other assets)
│
└── README.md             # Project documentation
```

---

## Tech Stack

- **Backend:** Flask (Python)
- **ORM:** SQLAlchemy
- **Frontend:** Jinja2 templating, HTML5, CSS3
- **Authentication:** Flask-Login, Bcrypt
- **Database:** PostgreSQL (cloud-hosted)
- **Deployment:** Compatible with Render, Heroku, etc.

---

## Getting Started

### Prerequisites

- Python 3.8+
- PostgreSQL (local or cloud)
- Node.js/NPM (for Render CLI, optional for database management)

### Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/Nanamshruthi/To-Do.git
    cd To-Do
    ```

2. **Set up a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables:**

    Create a `.env` file (or set in your deployment dashboard) with:
    ```
    SECRET_KEY=your_secret_key
    DATABASE_URL=your_postgres_connection_url
    ```

5. **Initialize the database:**
    - For a fresh database:
        ```python
        from app import db
        db.create_all()
        ```
    - For production apps, use Flask-Migrate.

6. **Run the application:**
    ```bash
    flask run
    ```

### Deployment

- Push to GitHub and connect to Render/Heroku.
- Configure environment variables (`DATABASE_URL`, `SECRET_KEY`).
- Use Render’s dashboard to manage and view your cloud database.

---

## Usage

- Sign up and log in.
- Add tasks with optional due dates.
- Edit, delete, or mark tasks complete/incomplete.
- Filter tasks by status using the UI.

---

## Screenshots

<img width="1919" height="896" alt="Screenshot 2025-10-05 121817" src="https://github.com/user-attachments/assets/ee285d86-961e-49df-aba2-4e359abc084c" />

---

<img width="1919" height="910" alt="Screenshot 2025-10-05 122009" src="https://github.com/user-attachments/assets/7f0542c0-2a61-437e-883d-924e728614a1" />


---

## Contributing

Pull requests are welcome! Please open an issue to discuss changes or features.

---

## License

MIT License

---

## Contact

- **GitHub:** [Nanamshruthi](https://github.com/Nanamshruthi)
- **LinkedIn:** [Shruthi Nanam](https://www.linkedin.com/in/nanam-shruthi-8b747b284/)
- **Instagram:** [shruthinanam](https://www.instagram.com/shruthinanam?igsh=MXYxNDkwcG9oYWUzOA==)

---

*This app was created for educational and productivity purposes. Thank you for checking out ToDo!*
