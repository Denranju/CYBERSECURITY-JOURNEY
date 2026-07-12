# 🌐 06-Web-Security

## Overview

This folder documents the web security concepts, practical exercises and laboratory challenges I have completed since beginning my cybersecurity journey in **May 2026**.

The knowledge documented here was primarily gained through **Hack The Box Academy**, where I completed the **Web Requests** and **Introduction to Web Applications** modules, together with practical web exploitation exercises in **OverTheWire Natas**.

Web security focuses on protecting websites, web applications and APIs from attacks that could compromise confidentiality, integrity and availability.

---

# 📅 Learning Journey

After building a strong foundation in networking, Linux and penetration testing, I began studying web security.

Through Hack The Box Academy and OverTheWire Natas, I learned how websites communicate, how HTTP requests work, how browsers interact with servers and how attackers identify common web vulnerabilities.

These practical laboratories allowed me to inspect web applications, analyse source code, manipulate HTTP requests and understand why client-side controls should never be trusted.

---

# 🎓 Learning Platforms

- Hack The Box Academy
- OverTheWire Natas

---

# ✅ Modules Completed

- Web Requests
- Introduction to Web Applications

---

# 🎯 Learning Objectives

The objectives of these modules were to:

- Understand how web applications work.
- Learn the HTTP protocol.
- Understand HTTP requests and responses.
- Learn client-server communication.
- Analyse web application components.
- Understand authentication mechanisms.
- Identify common web vulnerabilities.
- Develop practical web security skills.

---

# 📚 Topics Covered

## Web Applications

A web application is software that runs on a web server and is accessed using a web browser.

The three main components include:

- Client (Browser)
- Web Server
- Database

These components communicate using HTTP or HTTPS.

---

## HTTP

HTTP (Hypertext Transfer Protocol) is the protocol used to exchange information between web browsers and web servers.

Common HTTP methods include:

- GET
- POST
- PUT
- DELETE
- HEAD
- OPTIONS

---

## HTTP Response Codes

During my studies I learned the meaning of common HTTP response codes.

Examples include:

- 200 OK
- 301 Moved Permanently
- 302 Found
- 400 Bad Request
- 401 Unauthorized
- 403 Forbidden
- 404 Not Found
- 500 Internal Server Error

---

## HTTP Headers

HTTP headers exchange additional information between clients and servers.

Examples include:

- User-Agent
- Host
- Referer
- Cookie
- Authorization

I learned that HTTP headers are client-controlled and should never be trusted by web applications.

---

## Cookies

Cookies store session information inside a user's browser.

During practical labs I learned that insecure cookie validation can allow authentication bypass when applications trust client-side data.

---

## URL Manipulation

Changing parameters within URLs can reveal hidden functionality or expose sensitive information if applications do not validate user input correctly.

---

## Browser Developer Tools

Developer Tools allow security researchers to inspect:

- HTML
- CSS
- JavaScript
- Network requests
- Cookies
- Storage
- HTTP responses

These tools are essential during web application testing.

---

## Source Code Review

Viewing HTML, JavaScript and PHP source code can reveal hidden information including:

- Credentials
- Comments
- Hidden files
- Configuration information
- Application logic

---

## Directory Enumeration

Directory enumeration is the process of discovering hidden directories and files exposed by a web server.

This technique helps identify sensitive resources that should not be publicly accessible.

---

## robots.txt

The robots.txt file tells search engines which directories should not be indexed.

During my studies I learned that attackers often inspect robots.txt because it may unintentionally reveal sensitive directories.

---

# 🧪 OverTheWire Natas

## Completed Levels

- ✅ Natas 0
- ✅ Natas 1
- ✅ Natas 2
- ✅ Natas 3
- ✅ Natas 4
- ✅ Natas 5
- ✅ Natas 6

---

## Natas Level 0

### Objective

Learn how to inspect a webpage.

### What I Learned

I learned how to inspect HTML source code to discover hidden information that was not visible on the webpage.

### Skills Developed

- Viewing page source
- HTML inspection

---

## Natas Level 1

### Objective

Access page source even when right-click is disabled.

### What I Learned

I learned that disabling right-click provides no real security because browser developer tools and keyboard shortcuts still allow users to inspect webpages.

### Skills Developed

- Browser Developer Tools
- HTML inspection

---

## Natas Level 2

### Objective

Discover hidden files.

### What I Learned

I learned how directory enumeration can reveal sensitive files exposed on a web server.

### Skills Developed

- Directory enumeration
- File discovery

---

## Natas Level 3

### Objective

Locate hidden information using robots.txt.

### What I Learned

I learned that robots.txt may unintentionally disclose hidden directories that attackers can access.

### Skills Developed

- Information gathering
- robots.txt analysis

---

## Natas Level 4

### Objective

Manipulate the HTTP Referer header.

### What I Learned

I learned that HTTP headers are controlled by the client and can be modified, making them unsuitable for authentication or authorization decisions.

### Skills Developed

- HTTP headers
- Request manipulation

---

## Natas Level 5

### Objective

Modify browser cookies.

### What I Learned

I learned that client-side cookies can be modified by users and should never be trusted without proper server-side validation.

### Skills Developed

- Cookie manipulation
- Session management

---

## Natas Level 6

### Objective

Review application source code.

### What I Learned

I learned how exposed PHP source code and included configuration files can reveal sensitive secrets used for authentication.

### Skills Developed

- PHP source code analysis
- Configuration review
- Information disclosure

---

# 💻 Commands Used

Retrieve a webpage:

```bash
curl http://example.com
```

Send a custom HTTP header:

```bash
curl -H "Referer: http://example.com" URL
```

Retrieve only HTTP headers:

```bash
curl -I http://example.com
```

Retrieve a webpage with verbose output:

```bash
curl -v http://example.com
```

---

# 🛠️ Practical Skills Developed

During these modules and laboratories I developed practical skills in:

- Understanding web application architecture.
- Understanding HTTP communication.
- Analysing HTTP requests and responses.
- Inspecting web applications using browser developer tools.
- Viewing HTML source code.
- Discovering hidden directories.
- Performing directory enumeration.
- Analysing robots.txt.
- Manipulating HTTP headers.
- Modifying cookies.
- Understanding session management.
- Reading PHP source code.
- Identifying exposed files.
- Understanding information disclosure vulnerabilities.

---

# 💻 Tools and Technologies

During this stage of my learning journey I used:

- Hack The Box Academy
- OverTheWire Natas
- Firefox
- Google Chrome
- Browser Developer Tools
- curl
- Linux Terminal
- Windows PowerShell
- Git
- GitHub
- Visual Studio Code

---

# 🌍 Real-World Applications

The knowledge gained during these modules is directly applicable to:

- Web Application Penetration Testing
- Vulnerability Assessments
- Security Auditing
- Bug Bounty Hunting
- Secure Web Development
- Web Application Security Testing

---

# ✅ Best Practices

- Never trust client-side input.
- Validate all user input on the server.
- Secure cookies properly.
- Protect sensitive files.
- Remove unnecessary source code exposure.
- Restrict access to administrative resources.
- Implement proper authentication and authorization.
- Regularly test web applications for vulnerabilities.

---

# 📖 Source

- Hack The Box Academy – Web Requests
- Hack The Box Academy – Introduction to Web Applications
- OverTheWire – Natas

---

# 📌 Summary

Completing the **Hack The Box Academy** Web Requests and Introduction to Web Applications modules together with the **OverTheWire Natas** challenges provided me with a strong foundation in web application security.

I learned how web applications communicate using HTTP, how to inspect and manipulate requests, analyse source code, enumerate hidden resources and identify common web security weaknesses. These practical skills form the foundation for advanced web application penetration testing and secure software assessment.