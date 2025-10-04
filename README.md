To-Do: A Full-Stack Productivity Manager

## Overview
To-Do is a secure, personal productivity web application built using the Flask framework. It allows users to register, log in, and manage their daily tasks with advanced filtering capabilities. This project serves as a comprehensive demonstration of full-stack Python development, secure authentication, and relational database management.

---

## 🚀 Key Features
- **Secure User Authentication**: Implemented user signup and login using Flask-Login and securely hashing passwords with Flask-Bcrypt.  
- **Database Management**: Uses SQLAlchemy (ORM) with an SQLite database (`todo.db`) to manage users and tasks, enforcing a one-to-many relationship.  
- **Dynamic Task Filtering**: Tasks are automatically categorized and filterable by status based on the due_date:
  - **Overdue**: Tasks past the due date.  
  - **Due Today**: Tasks due on the current day.  
  - **Pending**: Tasks with a future due date.  
- **CRUD Operations**: Full functionality to Create, Read, Update (edit content and due date), and Delete tasks.  
- **Responsive Design**: Uses custom CSS for a clean, professional, dark-themed user interface.  

---

## 💻 Technology Stack

| Component      | Technology          | Description |
|----------------|---------------------|-------------|
| **Backend**    | Python 3.x, Flask   | Core web framework for routing and business logic. |
| **Database**   | SQLite, SQLAlchemy  | ORM for managing models (`User`, `Task`) and data persistence. |
| **Authentication** | Flask-Login, Flask-Bcrypt | Handling session management and secure password hashing. |
| **Frontend**   | Jinja2, HTML5, CSS  | Templating engine for dynamic content generation and styling. |

---

## 📁 Project Structure
The project follows a standard Flask structure:

To-Do/

├── app.py                                                # Main Flask application, routes, and database models

├── instance/

        └── todo.db                                            # SQLite database file (automatically generated)

├── static/

       ├── favicon.png                                        # Website favicon

       ├── reset.min.css                      # CSS reset file
       
       └── style.css # Custom application styles
       
├── templates/

       ├── about.html # Information about the application and stack
       
       ├── base.html # Main layout and navigation (header/footer)
       
       ├── login.html # Login form
       
       ├── signup.html # User registration form
       
       ├── tasks.html # Main dashboard for managing tasks
       
       ├── edit_task.html # Form for editing task details

       ├── privacy.html

       ├──terms.html
       
├── README.md # Project documentation (this file)

└── requirements.txt # List of required Python packages

├── .gitignore

├── procfile


## 🛠️ Setup and Installation

Follow these steps to get a copy of the project running on your local machine.

### 1. Prerequisites
You must have Python 3.x installed.

### 2. Create a Virtual Environment
It is recommended to use a virtual environment to manage dependencies:

bash
python3 -m venv venv

source venv/bin/activate  # On macOS/Linux

venv\Scripts\activate     # On Windows 

---
Install Dependencies

Install all required packages using pip. You will need to create a requirements.txt file (see the next step):

pip install -r requirements.txt

---

Run the Application

Start the Flask development server:

python3 app.py

---

🤝 Contribution

Feel free to fork the repository, submit pull requests, or open issues to suggest improvements or fix bugs!



