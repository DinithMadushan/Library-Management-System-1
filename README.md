# 📚 Library Management System

A comprehensive C++ command-line application for managing library operations including book inventory, reader registration, and book borrowing/returning functionality.

## 📖 Table of Contents
- ✨ [Features](#features)
- 🖥️ [System Requirements](#system-requirements)
- 📁 [Project Structure](#project-structure)
- 🔨 [Compilation & Setup](#compilation--setup)
- 🚀 [Usage Guide](#usage-guide)
- 📝 [File Format](#file-format)
- 🔐 [Login Credentials](#login-credentials)
- 🎯 [Features in Detail](#features-in-detail)

## ✨ Features

- 🔐 **Librarian Authentication**: Secure login system with username and password verification
- 📚 **Book Management**:
  - ➕ Add new books to the library with ISBN
  - 👁️ Display complete book inventory
  - 🔍 Search books by ISBN
  - 📦 Search within current library lot
- 👥 **Reader Management**:
  - 📝 Register new library members with auto-generated User IDs
  - 📋 Track reader information
- 🔄 **Book Borrowing System**:
  - 📥 Borrow available books from inventory
  - 📤 Return borrowed books to library
  - ✅ Automatic availability tracking via file management

## 🖥️ System Requirements

- 💻 **Compiler**: GCC, Clang, or any C++11 compatible compiler
- 🐧 **OS**: Windows, Linux, or macOS
- 🛠️ **IDE** (Optional): Code::Blocks, Visual Studio, Eclipse, or any text editor

## 📁 Project Structure

```
Library-Management-System-1/
├── main.cpp                           # Main program file
├── books.txt                          # Book inventory database
├── readers.txt                        # Reader information database
├── README.md                          # Project documentation
├── Library Management System 01.cbp  # Code::Blocks project file
├── Library Management System 01.depend
├── Library Management System 01.layout
└── obj/                               # Object files (build artifacts)
    └── Debug/
└── bin/                               # Compiled executable
    └── Debug/
```

## 🔨 Compilation & Setup

### 🟦 Using Code::Blocks (Recommended)
1. Open `Library Management System 01.cbp` in Code::Blocks
2. Click **Build** > **Build** (or press Ctrl+F9)
3. Click **Build** > **Run** (or press Ctrl+F10)

### 🖥️ Using Command Line (GCC/Clang)
```bash
# Navigate to project directory
cd Library-Management-System-1

# Compile the program
g++ -o library_system main.cpp

# Run the program
./library_system
```

### 🪟 On Windows (PowerShell)
```powershell
g++ -o library_system.exe main.cpp
.\library_system.exe
```

## 🚀 Usage Guide

### ▶️ Starting the Application
1. Run the compiled executable
2. Choose to login as a librarian or register/access as a reader

### 📋 Main Menu Options

| #️⃣ Option | 🎯 Feature | 📝 Description |
|--------|---------|-------------|
| 1 | ➕ Add Book | Add a new book with title and ISBN |
| 2 | 👁️ Display Book List | View all available books in inventory |
| 3 | 🔍 Search Book by ISBN | Find a specific book using ISBN |
| 4 | 📥 Borrow Book | Borrow an available book after registration |
| 5 | 📤 Return Book | Return a previously borrowed book |
| 6 | 📝 Register Reader | Register as a library member |
| 7 | 📦 Search Current Lot | Search within current book inventory |
| 8 | 🚪 Exit | Close the application |

## 📝 File Format

### 📚 books.txt
Stores available books in the inventory with comma-separated values:
```
Title,ISBN
The C++ Programming Language,978-0-13-110362-7
Modern C++ Design,978-0-201-70431-8
```

### 👥 readers.txt
Stores registered reader information:
```
UserID,FullName,ContactInfo
John0001,John Doe,john.doe@email.com
Jane0001,Jane Smith,jane.smith@email.com
```

### 📖 Individual Reader Files (UserID.txt)
Each registered reader has their own file storing borrowed books:
```
BookTitle,ISBN
The C++ Programming Language,978-0-13-110362-7
```

## 🔐 Login Credentials

🔓 **Default Librarian Account:**
- 👤 **Username**: `admin`
- 🔑 **Password**: `password`

⚠️ **Security Note**: Change credentials after initial setup in production environments.

## 🎯 Features in Detail

### 📚 Book Management
- ➕ **Add Books**: Add books by entering title and ISBN
- 🔍 **Search Functionality**: Search by ISBN or browse entire inventory
- ✅ **Availability Tracking**: Available books tracked in books.txt; borrowed books stored in reader files
- 📋 **Display Books**: View all current library inventory

### 👥 Reader System
- 📝 **Registration**: New readers register with name and contact info; auto-generated User IDs
- 📋 **Borrow Tracking**: Each reader has a personal file tracking their borrowed books
- 🔄 **Return Management**: Returns move books from reader files back to inventory

### 💾 Data Persistence
- 📄 Books stored in books.txt; readers in readers.txt
- 👤 Individual reader files (UserID.txt) track borrowed books
- ⚡ Changes persist between sessions
- 🚀 No database server required

## 💡 Development Notes

- 🛠️ Built in C++ using standard libraries (iostream, fstream, string, iomanip, sstream)
- 📄 File-based data storage for simplicity and portability
- ⌨️ Console-based user interface for straightforward interaction
- 🧩 Modular function design for easy maintenance and extension

## 🚀 Future Enhancements

- 🗄️ Database integration (SQLite/MySQL)
- 🖼️ GUI using Qt or wxWidgets
- 📧 Email notifications for overdue books
- 💰 Fine calculation system
- 🔎 User-friendly search filters
- 📤 Export/Import functionality

## License

This project is open-source and available for educational and personal use.

## 👨‍💻 Author

 Created as a library management system project demonstrating fundamental C++ concepts and file I/O operations.