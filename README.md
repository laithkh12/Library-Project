# 📚 **Book Collection Application** 

This is a simple **Flask** web application to manage a collection of books. You can **add**, **edit**, **delete**, and **view** books with their title, author, and rating.

---

## 📝 **Table of Contents**

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [How to Use](#how-to-use)
- [License](#license)

---

## 📦 **Project Overview**

This project is a simple Flask app that allows users to interact with a database of books. It includes functionality for CRUD (Create, Read, Update, Delete) operations on the book collection. The app uses **SQLAlchemy** to manage the SQLite database.

---

## 🛠️ **Technologies Used**

- **Flask**: A micro web framework for Python.
- **SQLAlchemy**: An ORM (Object Relational Mapper) for interacting with databases.
- **SQLite**: A lightweight database system used for storing book data.

---

## ⚙️ **Setup Instructions**

To set up the project on your local machine, follow the steps below:

1. Clone this repository.
2. Install the necessary dependencies:
   - **For Windows**: 
     ```bash
     python -m pip install -r requirements.txt
     ```
   - **For MacOS**: 
     ```bash
     pip3 install -r requirements.txt
     ```
3. Run the application:
   ```bash
   python app.py
    ```
4. Access the app by visiting http://127.0.0.1:5000 in your browser.
---
## 💻 How to Use
### 📖 Home Page
The homepage displays all books in the collection sorted by title. You can:
- View book details (title, author, and rating).
- Add new books to the collection.
- Edit the rating of existing books.
- Delete books from the collection.
### ➕ Add a Book
To add a book:
1. Click on the "Add Book" button.
2. Enter the book's title, author, and rating.
3. Submit the form to add the book to the collection.
## ✏️ Edit a Book
To edit a book's rating:
1. Click the "Edit" button next to a book.
2. Update the rating field.
3. Submit the form to save the changes.
## 🗑️ Delete a Book
To delete a book:
1. Click the "Delete" button next to the book you want to remove.
2. Confirm the deletion, and the book will be removed from the database.
---
## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
---
## 🎨 Logo and Decorations
Feel free to customize and decorate this app with your favorite logos and colors! Here’s an example to help you get started:
- Logo: Add your app's logo to the top of the pages.
- CSS: Customize the styles in your styles.css for a better UI.
---
## 🔧 Database Models
Here is an overview of the main database model:
```python
class Book(db.Model):
    id: Mapped[int] = mapped_column(Integer, primary_key=True)
    title: Mapped[str] = mapped_column(String(250), unique=True, nullable=False)
    author: Mapped[str] = mapped_column(String(250), nullable=False)
    rating: Mapped[float] = mapped_column(Float, nullable=False)
```
This model stores information about books, including the title, author, and rating.
---
Happy coding! 👨‍💻👩‍💻
