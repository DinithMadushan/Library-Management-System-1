# Library Management Frontend (React CDN - Zero Setup) - TODO

## Completed
- [x] Understand C++ backend from main.cpp and data files
- [x] Initial plan & user confirmation (React)
- [x] Adapt to CDN for no Node/npm issues

## Progress
1. **Project Setup** [x] Done (manual React+Tailwind CDN in single HTML)

2. **Core Implementation** [x] Done
   - App & all components/tabs/logic in index.html
   - Full CRUD, CSV parse/download, userID gen base

3. **Data Logic**
   - parseCSV(text): Split lines, ',' → objects
   - genUserID(firstName, readers): Mimic C++ (firstName0001++)
   - CRUD: addBook → books.push({title, isbn}), update display/download
   - Borrow: Move from tempBooks/books to userBorrowed, download userID.txt
   - Return: Reverse

4. **Create files**
   - frontend/index.html (React SPA)
   - frontend/style.css? No, Tailwind CDN

5. **Integrate Files**
   - Upload buttons (FileReader → parse → setState)
   - Download all (books.txt, readers.txt, temp_books.txt, selectedUser.txt)

6. **UI Polish**
   - Tailwind tables/forms/tabs responsive
   - Sidebar nav post-login

7. **Update README** & Test

8. **attempt_completion**


