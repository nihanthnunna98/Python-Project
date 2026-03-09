# Python-Project
Library Management System

This is a console-based Library Management System developed using Python and Object-Oriented Programming (OOP) principles. The program allows users to manage books in a library through a simple menu-driven interface.
The system is built using two main classes:
### Book Class
The Book class represents a single book in the library. Each book object contains:

title – The name of the book

author – The author of the book

is_issued – A boolean value that tracks whether the book is issued or available

By default, a newly added book is marked as available.

### Library Class

The Library class manages the collection of books. It maintains a list of Book objects and provides methods to perform operations such as:

Add Book – Adds a new book to the library.

Display Available Books – Shows all books that are currently not issued.

Issue Book – Marks a book as issued if it is available.

Return Book – Marks a previously issued book as returned.

### Key Features
Object-Oriented Design

Simple and user-friendly console interface

Book availability tracking

Basic error handling (book not found, already issued, etc.)

Case-insensitive search functionality

functionality
### 
Technologies Used

Python

OOP Concepts (Classes and Objects)

Loops and Conditional Statements

The Book class
Purpose
The Book class represents a single book object in the library.
Each time a book is added, a new Book object is created.
Constructor: init()

This is a constructor method. It runs automatically whenever a new Book object is created.

Parameters:

title → Name of the book
author → Name of the author
Instance Variables:
self.title → Stores the book title
self.author → Stores the author name
self.is_issued → Stores availability status
False → Book is available
True → Book is issued
The Library class
Purpose
The Library class manages all books.
It stores all Book objects inside a list called:
How It Works:
A new Book object is created:
That object is added to the list:
A success message is printed.
Function 2: display_available_books()
Purpose:
Displays only books that are not issued. Step-by-Step:

Prints heading

Sets

Loops through each book

Checks: If book is not issued → print it.

If no books were available: Prints- No books available.

Function 3: issue_book()
Purpose:
Marks a book as issued.

Step-by-Step:
Loop through all books
Compare titles (case-insensitive)
If found: Print message. If not issued: This changes availability status.
If already issued: Print message.

If book not found in entire list: Print - Book not found
Function 4: return_book()
Purpose:
Marks a book as returned (available again).

Step-by-Step:
Search book by title. If found: If issued: book.is_issued = False If not issued: Print message.
If not found: Print "Book not found."
