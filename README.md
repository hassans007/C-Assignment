# Book Management System

This is a Book Management System that allows users to search, update, and view details of books in a bookstore or library. The system is capable of managing the inventory, including adding new books and displaying their details, availability, and cost.

## Features

- **Search Book or Author**: Search for books by title or author, and view their details such as availability, cost, and copies available.
- **Update Inventory**: Admin users (e.g., shopkeeper, librarian) can add new books to the inventory and update the list.
- **Display All Books**: View details of all books currently in the inventory.
- **Login for Admin**: Admin users must log in to update the inventory.
- **Purchase Books**: Users can purchase available books, reducing the number of copies in the inventory.

## File Description

- **bookslist.txt**: This file is used to record updates such as the purchase of books and inventory changes. It is also used for storing details of books that are added to the system.
  
## Program Flow

1. **Main Menu**: The user is presented with the following options:
   - **1**: Search Book / Author
   - **2**: Update Inventory (Admin Only)
   - **3**: Display All Books Available
   - **4**: Exit

2. **Search Functionality**: Users can enter the book title or author's name to find a book. The system will display the book's details if found.

3. **Update Inventory (Admin Only)**: Admin users can log in with a specific ID and password to add new books to the inventory.

4. **Display All Books**: Displays the details of all books available in the store/library.

## Usage

1. **Search for a Book**: 
   - Enter the book title or author's name when prompted.
   - If the book is available, you can view its details and purchase it.

2. **Add New Books** (Admin only):
   - Admin users can add new books to the system by logging in with the correct ID and password.

3. **View Inventory**:
   - Displays all the books currently in the inventory, including their availability and price.

## Login Details (Admin Only)

- **Admin ID**: 2335
- **Admin Password**: 1122

Use these credentials to gain access to the admin functionalities like updating the inventory.

## How to Compile and Run

1. **Compile**: 
   - Use a C++ compiler to compile the program.
   - Example: `g++ book_management.cpp -o book_management`
   
2. **Run**:
   - After compiling, run the program.
   - Example: `./book_management`

## Author

Made by: **Hassan Shahid**
