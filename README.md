# Final Exam - FA24 - Library Book Management System

## Objective

To create a C++ program that manages a collection of books in a library. The program should allow the user to add, display, update, and delete book records using classes, arrays, enumeration types, and functions. Remember that each program is done separately with a CPP file uploaded for each. You must include the standard formatting for my name and yours and include comments.

## Problem Statement

Write a C++ program to manage a list of books in a library. Each book has a unique ID, title, author, and genre. The genre should be represented as an enumeration (e.g., Fiction, NonFiction, Mystery, SciFi, etc.). The program should store books in an array and provide functions to add, display, update, and delete books.

## Requirements

1.	Define an enum type Genre:
o	Genre should represent book genres: Fiction, NonFiction, Mystery, SciFi, Romance, History, True Crime, and Biography.
2.	Define a Book class:
o	Private member variables:
	int id – A unique identifier for each book.
	string title – The title of the book.
	string author – The author of the book.
	Genre genre – The genre of the book.
o	Public member functions:
	BookCreator: Initializes the book's ID, title, author, and genre.
	void display() const: Displays the book's details, including ID, title, author, and genre.
	void setDetails(int id, const std::string& title, const std::string& author, Genre genre): A function to set book details.
3.	Define a Library class:
o	Private member variables:
	Book books[20] – An array to store up to 20 Book objects.
	int bookCount – Keeps track of the number of books currently in the array.
o	Public member functions:
	void addBook(const Book& book): Adds a Book to the array, if there is space.
	void displayAllBooks() const: Displays details of all books in the array.
	void updateBook(int id, const std::string& title, const std::string& author, Genre genre): Updates a book's details by ID.
	void deleteBook(int id): Deletes a book from the array by ID.
4.	Main Program:
Display a menu with options to:
1.	Add a new book.
2.	Display all books.
3.	Update a book's details by ID.
4.	Delete a book by ID.
5.	Exit.
Use a loop to keep the program running until the user chooses to exit.


## Sample Output

Counterman’s Library Book Management System
1. Add a New Book
2. Display All Books
3. Update Book Details
4. Delete Book
5. Exit
Enter your choice: 1

Enter Book ID: 101
Enter Book Title: The Great Gatsby
Enter Author: F. Scott Fitzgerald
Enter Genre (0=Fiction, 1=NonFiction, 2=Mystery, 3=SciFi, 4=Biography, 5 = Romance, 6 = History, 7 = True Crime): 0

Book added successfully!


## Constraints
* Limit the library to a maximum of 20 books.
* Validate user input to ensure that genre values are within the defined Genre enum.
* Handle errors gracefully, like when trying to update or delete a non-existent book.

## Extra Credit
* Implement a search function to find books by title or author.
* Add functionality to calculate and display the count of books in each genre.

## Hints
* Use static_cast to convert integer input to the Genre enum.
* Use functions to keep the main program organized and modular.
* Put ALL functions after the main program for full credit.
* Don’t forget to comment.


