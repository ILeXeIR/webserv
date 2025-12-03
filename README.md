# Webserv

A lightweight HTTP server written in C++ with CGI support (Python, PHP), built from scratch as a Codam (42 Network) project, implementing core HTTP features without using external web server libraries.

---

## 📚 About the Project

The objective is to understand how an HTTP server works at a low level:

- socket programming
- non-blocking I/O
- process management
- request/response formatting
- CGI execution
- server configuration

---

## 🚀 Features

- HTTP/1.1 server written in **C++**
- Request parsing (methods, headers, body)
- Routing and configuration file support
- Handling **GET**, **POST**, **DELETE** methods
- **CGI execution** (CGI scripts written in Python and PHP)
- Static file serving
- Chunked transfer support
- Basic error handling (4xx/5xx)
- Multiple client connections (non-blocking I/O)
- Cookies and session management support

---

## 🧩 Technologies

- **C++**
- **Python** for CGI scripts
- **epoll()** / non-blocking sockets
- POSIX system calls, Unix-style process and file handling

---

## 👥 Team

Project built by a team of two students at Codam (42 Network): me and [@ilovecjj1127](https://github.com/ilovecjj1127)

### **My contribution**
- HTTP request parsing
- Server response formatting and status handling
- Static file serving and error pages
- Socket setup, connection handling, and non-blocking I/O
- Python CGI script development
- Cookies and session management implementation
- Debugging, testing, and overall backend/server logic

---

## ⚠️ System Requirements

This project uses POSIX system calls (fork, execve, epoll, socket, etc.) and must be run on a **Unix-like operating system**:

- **Linux** (recommended)
- **macOS** (fully supported)

**Windows is not supported**, unless using WSL2 (Windows Subsystem for Linux).

---

## 🔧 How to Run

**1.** Compile:

```make```

**2.** Run server with your config file:

```./webserv default.conf```

**3.** Open (servername and port from your config file):

http://localhost:8081

