# To-Do List Web Application

A comprehensive, full-stack To-Do list web application designed for personal productivity and built to showcase modern development skills.

## Features

- **User Authentication:** Secure signup/login via Flask-Login, passwords hashed using Bcrypt.
- **Task Management:** Add, edit, delete, and toggle tasks (complete/incomplete).
- **Due Dates:** Set due dates for tasks, with automatic status categorization.
- **Dynamic Filtering:** Filter tasks by Overdue, Due Today, and Pending status.
- **User Isolation:** Each user has private access to their own tasks.
- **Responsive UI:** Modern design with Jinja2 templates and FontAwesome icons.
- **Built-in Flash Messages:** User feedback for every key action.
- **Cloud Database:** All data stored in a managed PostgreSQL instance (e.g., on Render).

## Tech Stack

- **Backend:** Flask (Python)
- **ORM:** SQLAlchemy
- **Frontend:** Jinja2 templating, HTML5, CSS3
- **Authentication:** Flask-Login, Bcrypt
- **Database:** PostgreSQL (cloud-hosted)
- **Deployment:** Compatible with Render, Heroku, etc.

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

## Usage

- Sign up and log in.
- Add tasks with optional due dates.
- Edit, delete, or mark tasks complete/incomplete.
- Filter tasks by status using the UI.

## Screenshots

*(Add screenshots of the main UI, task list, filters, etc.)*

## Contributing

Pull requests are welcome! Please open an issue to discuss changes or features.

## License

MIT License

## Contact

- **GitHub:** [Nanamshruthi](https://github.com/Nanamshruthi)
- **LinkedIn:** [Shruthi Nanam](https://www.linkedin.com/in/nanam-shruthi-8b747b284/)
- **Instagram:** [shruthinanam](https://www.instagram.com/shruthinanam?igsh=MXYxNDkwcG9oYWUzOA==)

---

*This app was created for educational and productivity purposes. Thank you for checking out ToDo!*