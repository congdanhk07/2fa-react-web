# Two-Factor Authentication (2FA) Project

## Overview

This project implements a Two-Factor Authentication (2FA) system using React, Node.js, and Express. The system allows users to log in with their credentials and then requires a second form of verification using a QR code.

## Features

* User authentication using username and password
* Two-Factor Authentication (2FA) using QR code
* User profile management
* Protected routes for authenticated users

## Technologies Used

* Frontend: React, React Router, Material-UI
* Backend: Node.js, Express, MongoDB (using NeDB)
* Authentication: JSON Web Tokens (JWT)

## Getting Started

### Prerequisites

* Node.js (version 20.x)
* npm (version 8.x)
* MongoDB (using NeDB)

### Installation

1. Clone the repository: `git clone https://github.com/your-username/2fa-project.git`
2. Install dependencies: `npm install`
3. Start the backend server: `node src/server.js`
4. Start the frontend server: `npm start`

## API Documentation

### User API

* `POST /v1/users/login`: Log in with username and password
* `GET /v1/users/:id`: Get user profile
* `GET /v1/users/:id/get_2fa_qr_code`: Get 2FA QR code

### 2FA API

* `POST /v1/users/:id/confirm_2fa`: Confirm 2FA setup

## Frontend Routes

* `/login`: Login page
* `/dashboard`: Dashboard page (protected route)
* `/setup-2fa`: 2FA setup page (protected route)

## Contributing

Contributions are welcome! Please submit a pull request with a clear description of the changes.

## License

This project is licensed under the MIT License.

## Acknowledgments

This project was inspired by the MERN Stack Pro tutorial series by Tran Cong Danh.
