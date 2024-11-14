# Kanban-Board-Security-Authentication


## Description
A secure Kanban board application for agile teams, leveraging JSON Web Tokens (JWT) for user authentication. This project provides a seamless login experience, robust session management, and task organization within a simple Kanban interface.

## Table of Contents
- [About the Project](#about-the-project)
- [Features](#features)
- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [GitHub Link](#github-link)
- [Render Link](#render-link)

## About the Project

This project is built to securely authenticate users and manage work tasks via a Kanban board. It uses JWTs to encode user credentials, offering a scalable, secure way to verify identity across various parts of the application. Users can log in to access their Kanban board, where they can add, move, and manage tasks according to agile methodologies.

## Features

- **Secure Login Page**: Includes form inputs for username and password.
- **JWT Authentication**: Tokens are securely stored in client local storage, allowing authenticated API requests.
- **Session Management**: Tokens expire after a period of inactivity, redirecting users to log in again.
- **Error Handling**: Displays errors for invalid login credentials.
- **Logout**: JWT is removed from local storage, and users are redirected to the login page.

## User Story

**As a** member of an agile team  
**I want** a Kanban board with a secure login page  
**So that** I can securely access and manage my work tasks  

## Acceptance Criteria

1. **Login Page**: Users see input fields for username and password.
2. **Valid Login**: Authenticates users with JWT and redirects them to the Kanban board.
3. **Invalid Login**: Displays an error message for incorrect credentials.
4. **Session Persistence**: JWT is stored securely for authenticated requests.
5. **Logout**: JWT is removed from local storage, and users are redirected to log in.
6. **Unauthenticated Access**: Redirects unauthenticated users to the login page.
7. **Session Expiration**: JWT invalidates after a defined period of inactivity.

## Getting Started

To get a local copy of the project up and running, follow these steps.

### Prerequisites
- Node.js (v14 or later)
- MongoDB or similar NoSQL database
- Basic knowledge of JWTs and secure storage practices

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/kanban-jwt-auth

2. Navigate to the project directory:
   ```
   cd Kanban-Board-Security-Authentication

3. Install dependencies:
   ```
   npm install

4. Create a .env file to store your JWT secret and database configuration:
   ```
   JWT_SECRET=your_secret_key
   DB_URI=your_database_uri

5. Start the development server:
   ```
   npm run start:dev

## Usage

1. Visit http://localhost:3000/login in your browser.
2. Register or log in using valid credentials.
3. After successful login, manage tasks on your Kanban board.
4. Log out to invalidate your session.

## License
This project is licensed under the MIT License.

![License](https://img.shields.io/badge/license-MIT-yellow)

## GitHub Link
https://github.com/bobdajacob/Kanban-Board-Security-Authentication

## Render Link
https://kanban-board-security-authentication.onrender.com
