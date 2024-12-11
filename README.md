# Book Store System

## Introduction

This is a program that implements a Book Store System. The program allows users to search for books in the library by name or author and then buy the book if they want. If the book is available, the program displays its details, including the title, author, publisher, cost, and the number of copies available. The program also updates the inventory file after a user buys a book, reducing the number of copies available.

## Implementation

### Book Structure

The program uses a struct called `Book` to store information about each book. The `Book` struct has the following fields:

- **name**: A string that represents the name of the book.
- **author**: A string that represents the name of the author of the book.
- **publisher**: A string that represents the name of the publisher of the book.
- **available**: A string that indicates whether the book is available or not. If the book is available, this field is set to "Yes"; otherwise, it is set to "No".
- **cost**: A string that represents the cost of the book.
- **copies**: An integer that represents the number of copies of the book that are available.

### Books File Format

The program reads the book information from a file called `bookslist.txt` and stores it in an array of `Book` structs called `books`. The `bookslist.txt` file has the following format:

For example, a line in the file might look like this:

To Kill a Mockingbird, Harper Lee, Grand Central Publishing, Yes, $9.89, 10


### Functions

The program includes the following functions:

1. **Logincheck()**  
   This function is responsible for verifying user credentials before allowing access to the system. It prompts the user to choose between admin or user login, sets the correct ID (2335) and password (1122), and allows the user to enter their credentials. If the login is successful, the function sets a flag variable to indicate this.

2. **Search()**  
   The `Search()` function allows users to search for books by title or author. The program reads the book information from the `bookslist.txt` file and stores it in the `books` array. The user can enter either a book name or the author's name to search. If the user enters "exit", the program terminates. If a valid book or author is found, the program displays its details and prompts the user to buy the book. If no match is found, an appropriate message is displayed. If the user buys the book, the program updates the `bookslist.txt` file and reduces the number of available copies.

3. **UpdateInventory()**  
   The `UpdateInventory()` function allows the admin to update the inventory list by adding new books. It is responsible for adding new books to the `bookslist.txt` file. It prompts the admin to enter the name of the book, the author's name, the publisher's name, the cost, and the number of copies available. The new book information is then appended to the inventory file.

4. **Display()**  
   The `Display()` function is responsible for displaying all the books available in the inventory. It outputs all the details about each book, including the book's name, author, publisher, availability, cost, and the number of copies available.

## Features

- **Search Books by Name or Author**: Users can search for books by entering the book title or the author's name.
- **Display Book Details**: If a book is found, the program displays the book's details, including the title, author, publisher, cost, availability, and number of copies available.
- **Buy Books**: Users can buy books. If the user buys a book, the number of available copies is reduced and the `bookslist.txt` file is updated accordingly.
- **Admin Access**: Admin users can log in using predefined credentials (ID: 2335, Password: 1122) and can update the inventory by adding new books to the system.
- **Inventory Update**: Admins can add new books to the inventory and update the `bookslist.txt` file with new book details.

## How to Use

1. **Search for a Book**:  
   - Enter the name of the book or the author's name when prompted.
   - If the book is available, you will see its details and be prompted to purchase it.
   - If no match is found, an error message will appear.
   
2. **Purchase a Book**:  
   - If the book is available, you can choose to purchase it.
   - If you purchase the book, the number of available copies will be reduced and the `bookslist.txt` file will be updated.

3. **Add New Books (Admin Only)**:  
   - Admins can log in using the credentials (ID: 2335, Password: 1122).
   - Admins can add new books to the inventory and the `bookslist.txt` file by entering the details of the new book (name, author, publisher, cost, copies).

4. **View All Available Books**:  
   - Admin or user can display all books in the inventory, with all their details.

## Login Details (Admin Only)

- **Admin ID**: 2335
- **Admin Password**: 1122

## Program Flow

1. **Main Menu**:  
   - The user is presented with the following options:
     - **1**: Search Book / Author
     - **2**: Update Inventory (Admin Only)
     - **3**: Display All Books Available
     - **4**: Exit

2. **Search Functionality**:  
   - The user is prompted to enter a book name or author's name.
   - If a match is found, the book details are displayed.
   - The user can choose to buy the book, which reduces the number of copies.

3. **Admin Login**:  
   - Admin users log in using their ID and password (2335/1122).
   - Once logged in, the admin can add new books to the inventory.

4. **Inventory Update**:  
   - The program updates the `bookslist.txt` file when a user buys a book or when an admin adds new books to the system.

## Author

Made by: **Hassan Shahid**

