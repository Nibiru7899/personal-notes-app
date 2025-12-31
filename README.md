# Personal Notes App [![Python](https://img.shields.io/badge/Python-3.9+-blue)](https://www.python.org/) [![HTML/CSS](https://img.shields.io/badge/HTML/CSS-5+-orange)](https://www.w3schools.com/) [![SQLite](https://img.shields.io/badge/SQLite-3.3+-green)](https://www.sqlite.org/)

## Description
The Personal Notes App is a simple web application designed to allow users to create, read, update, and delete personal notes in a secure and organized manner. This project serves as a learning tool for beginners, focusing on basic CRUD operations and simple I/O operations in Python.

## Features
* User-friendly interface for creating and managing notes
* Ability to add, edit, and delete notes
* Secure storage of notes using SQLite database
* Basic search functionality for notes

## Tech Stack
The project utilizes the following technologies:
* **Primary**:
	+ Python: For backend logic and database interactions
	+ HTML/CSS: For frontend development and styling
* **Secondary**:
	+ SQLite: For database management and storage
* **Optional**:
	+ None

## Getting Started
### Prerequisites
* Python 3.9+
* SQLite 3.3+
* Basic understanding of Python and HTML/CSS

### Installation
1. Clone the repository: `git clone https://github.com/your-username/Personal-Notes-App.git`
2. Navigate to the project directory: `cd Personal-Notes-App`
3. Install required packages: `pip install -r requirements.txt`
4. Initialize the database: `python db_init.py`

### Usage
1. Run the application: `python app.py`
2. Open a web browser and navigate to `http://localhost:5000`
3. Create an account and start managing your notes

## Project Structure
The project is organized into the following directories:
* `app`: Contains the main application logic and routes
* `db`: Contains the database schema and initialization scripts
* `templates`: Contains HTML templates for the frontend
* `static`: Contains CSS and JavaScript files for the frontend
* `requirements.txt`: Lists the required packages for installation

## Learning Objectives
This project aims to help beginners achieve the following learning objectives:
* Understand basic syntax and data structures in Python
* Learn to perform CRUD operations using a simple database
* Implement basic I/O operations for user input and output

## Contributing
Contributions are welcome! If you'd like to contribute to the project, please:
1. Fork the repository
2. Create a new branch for your feature or bug fix
3. Submit a pull request with a clear description of your changes

## License
The Personal Notes App is licensed under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute the code as per the terms of the license.

Example use case:
```python
# Create a new note
note = Note(title="My First Note", content="This is my first note.")
db.session.add(note)
db.session.commit()

# Retrieve all notes
notes = Note.query.all()
for note in notes:
    print(note.title, note.content)
```