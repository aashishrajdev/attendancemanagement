# Attendance Management System

A simple **Attendance Management System** for students using C++. It allows an administrator to register students, view or delete student records, and allows students to mark and view their attendance or submit leave applications.

---

## Features

### Admin
- Login with credentials
- Register a new student
- View list of registered students with roll numbers
- Delete all student records
- View list of usernames of registered students
- Delete data of a specific student

### Student
- Login with username and password
- Mark attendance for the day
- View attendance count and percentage
- Send leave application

---

## Project Structure

```
.
├── db.dat                  # Stores registered usernames
├── *.dat                  # Individual student data files (username.dat)
├── application.dat        # Stores leave applications
└── main.cpp               # Source code file
```

Each student's `.dat` file contains the following:
```
Name
Username
Password
Roll Number
Address
Father's Name
Mother's Name
Attendance Count
```

---

## Getting Started

### Prerequisites
- Windows OS (uses `<windows.h>` and `<conio.h>`)
- C++ compiler (e.g., GCC via MinGW or MSVC)

### Compile and Run
```bash
g++ main.cpp -o attendance.exe
./attendance.exe
```

## Admin Credentials

```
Username: admin
Password: admin@2
```

---

## Notes

- Data persistence is achieved using plain text files (`.dat`).
- Attendance count is a number stored at the end of each student's file.
- Students must use the exact username/password they registered with.

---

## Limitations

- Console-based UI only
- No encryption on stored passwords
- Platform dependent (Windows)

---

## To-Do

- [ ] Use hashed passwords for security
- [ ] Add export to CSV functionality
- [ ] Build a GUI using a library like Qt or a web front-end

---

## License

This project is open-source and free to use for educational purposes.
