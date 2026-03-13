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
  - ➕ Add new books to the library inventory
  - 👁️ Display complete book list with details
  - 🔍 Search books by ISBN
  - 📦 Search books in current inventory
  - 🗑️ Remove books from the library
- 👥 **Reader Management**:
  - 📝 Register new library members
  - 📋 Track reader information and borrowed books
- 🔄 **Book Borrowing System**:
  - 📥 Borrow available books
  - 📤 Return borrowed books to the library
  - ✅ Automatic availability tracking

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
| 1 | ➕ Add Book | Add a new book to the library inventory |
| 2 | 👁️ Display Book List | View all books currently in the library |
| 3 | 🔍 Search Book by ISBN | Find a specific book using its ISBN number |
| 4 | 📥 Borrow Book | Borrow an available book from the library |
| 5 | 📤 Return Book | Return a previously borrowed book |
| 6 | 📝 Register Reader | Register a new library member |
| 7 | 📦 Search Current Lot | Search within the current book inventory |
| 8 | 🚪 Exit | Close the application |

## 📝 File Format

### 📚 books.txt
Stores book information with the following format:
```
ISBN | Title | Author | Quantity | Available
978-0-13-110362-7 | The C++ Programming Language | Bjarne Stroustrup | 5 | 3
```

### 👥 readers.txt
Stores reader information and their borrowed books:
```
UserID | Name | Email | Borrowed Books
R001 | John Doe | john@example.com | Book Title (ISBN)
```

## 🔐 Login Credentials

🔓 **Default Librarian Account:**
- 👤 **Username**: `admin`
- 🔑 **Password**: `password`

⚠️ **Security Note**: Change credentials after initial setup in production environments.

## 🎯 Features in Detail

### 📚 Book Management
- ➕ **Add Books**: Input ISBN, title, author, and quantity
- 🔍 **Search Functionality**: Multiple search options (ISBN, title, or full inventory)
- ✅ **Availability Tracking**: System automatically tracks book availability
- 🗑️ **Remove Books**: Manage inventory by removing out-of-stock items

### 👥 Reader System
- 📝 **Registration**: New readers can register with their details
- 📋 **Borrow Tracking**: System maintains records of borrowed books per reader
- 🔄 **Return Management**: Streamlined return process that updates availability

### 💾 Data Persistence
- 📄 All book and reader data is stored in text files
- ⚡ Changes persist between application sessions
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