# MRShare

> Privacy-first temporary file sharing platform built with Node.js, Express, SQLite, and Multer.

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge\&logo=node.js\&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge\&logo=express\&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge\&logo=sqlite\&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)

## Overview

[website link](https://mr-share.onrender.com/)

MRShare is an open-source temporary file-sharing platform designed for quick and secure file transfers without requiring user registration, email addresses, or personal information.

Users can upload a file, receive a unique access code, and share that code with others. Files are stored temporarily and automatically deleted after expiration, ensuring privacy and reducing storage overhead.

---

## Problem Statement

Most file-sharing platforms require:

* User accounts
* Personal information
* Third-party services
* Permanent file storage

MRShare solves this by providing a lightweight, privacy-focused solution for temporary file transfers.

---

## Key Features

### Current Features

* Secure file upload system
* Unique access code generation
* Temporary file storage
* Automatic file expiration
* Automatic cleanup service
* File type validation
* File size restrictions
* HTTPS-ready deployment
* Responsive web interface

### Planned Features

* Drag & drop uploads
* QR code sharing
* One-time download links
* File encryption
* Upload progress tracking
* Download analytics
* Cloud storage integration
* Rate limiting
* Admin dashboard

---

## Architecture

```text
Client Browser
      │
      ▼
 Express Server
      │
 ┌────┼───────────┐
 │    │           │
 ▼    ▼           ▼
Multer SQLite  Cleanup Job
 │      │
 ▼      ▼
Uploads Metadata
```

---

## Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript

### Backend

* Node.js
* Express.js

### Database

* SQLite

### File Handling

* Multer

### Deployment

* Nginx
* Render
* DigitalOcean VPS

### Security

* HTTPS (Let's Encrypt)

---

## Project Structure

```bash
MRShare/
│
├── app.js
├── package.json
├── database.db
│
├── uploads/
│
├── public/
│   ├── style.css
│   └── pages/
│       ├── home.html
│       ├── access.html
│       ├── test-upload.html
│       └── errors/
│           ├── invalid.html
│           ├── expired.html
│           └── 404.html
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/your-username/mrshare.git
cd mrshare
```

### Install Dependencies

```bash
npm install
```

### Start Development Server

```bash
node app.js
```

Open:

```text
http://localhost:3000
```

---

## Deployment

MRShare can be deployed on:

* Render
* DigitalOcean
* AWS EC2
* Railway
* VPS Servers

---

## Roadmap

* [ ] Modern UI redesign
* [ ] File encryption
* [ ] QR code file sharing
* [ ] User-selectable expiry
* [ ] Download limits
* [ ] Cloud storage support
* [ ] PostgreSQL migration
* [ ] Analytics dashboard

---

## Contributing

Contributions are welcome.

Please read the [CONTRIBUTING.md](CONTRIBUTING.md) guidelines before submitting a pull request.

---

## License

Distributed under the MIT License.

---

## Maintainer

**Sarjan Sonkar**

Open-source contributions and suggestions are welcome.

If you find this project useful, consider giving it a ⭐ on GitHub.
