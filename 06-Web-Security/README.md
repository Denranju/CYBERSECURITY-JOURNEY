# 06-Web-Security
# 🌐 06-Web-Security

## Overview

This folder contains my notes, commands and lessons learned while studying web security through OverTheWire Natas and other web security labs.

## What is Web Security?

Web security focuses on protecting websites, web applications and APIs from attacks that could compromise confidentiality, integrity or availability.

## Tools Used

Browser Developer Tools

View Page Source

curl

Firefox

Google Chrome

HTTP Headers

Cookies

URL Manipulation

## OverTheWire Natas Progress

Completed Levels:

✅ Natas 0

✅ Natas 1

✅ Natas 2

✅ Natas 3

✅ Natas 4

✅ Natas 5

✅ Natas 6

---

## Natas Level 0

### Objective

Learn how to inspect a web page.

### What I Learned

I learned how to view a webpage's source code and identify hidden information.

### Skills Gained

Viewing HTML source code.

---

## Natas Level 1

### Objective

Access the page source even when right-click is disabled.

### What I Learned

Disabling right-click does not provide security because page source can still be viewed using browser shortcuts or developer tools.

### Skills Gained

Using browser developer tools.

---

## Natas Level 2

### Objective

Discover hidden files.

### What I Learned

I learned directory enumeration by exploring hidden directories and files exposed on a web server.

### Skills Gained

Directory enumeration.

Understanding exposed files.

---

## Natas Level 3

### Objective

Find hidden information using robots.txt.

### What I Learned

I learned that robots.txt can reveal directories that website administrators intended to hide from search engines.

### Skills Gained

Using robots.txt for information gathering.

---

## Natas Level 4

### Objective

Manipulate the HTTP Referer header.

### What I Learned

I learned that web applications should never trust client-controlled HTTP headers because they can be modified.

### Skills Gained

Understanding HTTP headers.

Using modified requests.

---

## Natas Level 5

### Objective

Modify cookies.

### What I Learned

I learned that client-side cookies should never be trusted because users can edit them.

### Skills Gained

Cookie manipulation.

Understanding client-side authentication.

---

## Natas Level 6

### Objective

Review the source code and find hidden secrets.

### What I Learned

I learned how exposed source code and included files can reveal sensitive information that allows authentication bypass.

### Skills Gained

Reading PHP source code.

Finding exposed include files.

Using discovered secrets.

---

## Commands Used

```bash
curl http://example.com
```

Retrieves a web page from the command line.

```bash
curl -H "Referer: http://natas5.natas.labs.overthewire.org/" URL
```

Sends a custom HTTP Referer header.

## Skills Gained

I learned how to inspect web pages, enumerate directories, use robots.txt for reconnaissance, manipulate HTTP headers, modify cookies, review source code, identify exposed files and understand why client-side controls should never be trusted.
Notes for 06-Web-Security go here.