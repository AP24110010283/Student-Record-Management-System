# Student Record Management System (SRMS) – C Language

A console-based Student Record Management System built using **C programming** with **file handling** and **role-based authentication**.  
The project demonstrates CRUD operations, secure login, and persistent data storage using text files.

## Features

### Role-Based Access Control
- **ADMIN** – Add, View, Search, Update, Delete  
- **STAFF** – View, Search, Update  
- **GUEST** – View, Search  

### File Handling
- Student records → `students.txt`  
- Login credentials → `credentials.txt`  
- Safe update/delete using temporary file swapping  

### Core Functionalities
- Add Student  
- View All Records  
- Search (Name / Roll No., case-insensitive)  
- Update Record  
- Delete Record  
- Duplicate roll number prevention  
- Strong input validation  

## Project Structure

```text
SRMS-Project/
│-- main.c
│-- credentials.txt
│-- students.txt (empty)
│-- README.md
```

## Credentials Format (`credentials.txt`)

```text
username password ROLE
```

Example:
```text
admin admin123 ADMIN
staff staff123 STAFF
guest guest123 GUEST
```

## How to Compile & Run

### Using GCC

```bash
gcc main.c -o srms
./srms
```

### Using GitHub Codespaces

```bash
gcc main.c -o srms
./srms
```

## Student File Format (`students.txt`)

```text
Roll|Name|Marks
```

Example:
```text
101|Alice Smith|92.50
```

## Technologies Used

- C Programming  
- Structures  
- File I/O (`fopen`, `fscanf`, `fprintf`)  
- Modular programming  
- Input validation utilities  

## Future Improvements

- Password hashing  
- Add more fields (Dept, Semester, Attendance)  
- SQLite integration  
- GUI Version  

## Author

**Mukesh Krishna**  
B.Tech CSE (AI & ML)
