# Rent-Room-Project

This is a room rental system for MFU (Maejo University) that allows users to request and rent rooms across campus buildings. The system includes a Flutter mobile app for users, a Node.js backend server, and a MySQL database.

## Features

- User registration and login
- Browse available rooms with time slots
- Submit room rental requests with reasons
- View personal request history and borrowing history
- Role-based access (user, approver, staff)
- Room availability tracking

## Technologies

- Frontend: Flutter
- Backend: Node.js with Express
- Database: MySQL
- Authentication: bcrypt for password hashing

## Setup

### Prerequisites

- MySQL server running
- Node.js installed
- Flutter SDK configured

### Database Setup

1. Create a MySQL database named MFUrooms
2. Import the SQL file from SQL/MFUrooms.sql

### Backend Setup

1. Navigate to the Server directory
2. Install dependencies: npm install
3. Start the server: npm run app

### Frontend Setup

1. Navigate to the Fultter directory
2. Install dependencies: flutter pub get
3. Run the app: flutter run

## Usage

1. Register a new account or login with existing credentials
2. Browse available rooms and select a time slot
3. Submit a rental request with a reason
4. View your requests and history in the user dashboard

## API Endpoints

- POST /login - User authentication
- POST /register - User registration
- GET /rooms - Get available rooms
- POST /user/rentRoom - Submit rental request
- GET /user/request - Get user requests
- GET /user/history - Get user borrowing history
- GET /staff/history - Get all rental history (staff only)

## Notes

- The server is configured to run on http://192.168.2.34:3000
- Update the IP address in the Flutter app if deploying to a different server
- This is a development version with hardcoded values
