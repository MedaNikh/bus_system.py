# Bus Tracker System

A comprehensive web-based bus management system that allows users to track buses, manage routes, view driver information, and handle digital bus passes.

## Features

### 🚌 Core Functionality
- *Real-time Bus Tracking*: Track buses and their current locations
- *Route Management*: View bus routes with source, destination, and timing information
- *Driver Information*: Access driver details and contact information
- *Digital Bus Pass*: E-bus pass system with pass ID lookup functionality
- *User Authentication*: Secure user registration and login system

### 🎨 User Interface
- Responsive web design with modern gradient backgrounds
- Clean, intuitive navigation across all pages
- Interactive bus tracking cards and information displays
- Mobile-friendly interface

## Tech Stack

### Backend
- *Framework*: Flask (Python)
- *Database*: MySQL with SQLAlchemy ORM
- *Authentication*: JWT tokens with Flask-JWT-Extended
- *Security*: Password hashing with Flask-Bcrypt
- *API*: RESTful API with CORS support

### Frontend
- *Languages*: HTML5, CSS3, JavaScript (ES6+)
- *Styling*: Custom CSS with gradients and modern design
- *API Communication*: Fetch API for backend communication
- *Storage*: In-memory storage for session data

## 📸 Screenshots

### Welcome Page
![Welcome Page](screenshots/welcome.png)

### Login Page
![Login Page](screenshots/login.png)

### Registration Page
![Registration Page](screenshots/register.png)

### Dashboard/Homepage
![Dashboard](screenshots/homepage.png)

### Dashboard/Homepage
![Dashboard](screenshots/homepage-continued.png)

### User Profile
![User Profile](screenshots/profile.png)

### Digital Bus Pass - Login Form
![Bus Pass Login](screenshots/buspass-login.png)

### Digital Bus Pass - Pass Display
![Bus Pass Display](screenshots/buspass-display.png)

## Project Structure


bus_tracker_system/
│   ├── welcome.html          # Landing page
│   ├── login.html           # User login
│   ├── register.html        # User registration
│   ├── homepage.html        # Main dashboard
│   ├── profile.html         # User profile
│   ├── buspass.html         # Digital bus pass
│   └── bus1.jpg             # Bus image asset
│   └── busSystem.py         # Flask application
├── screenshots/              # Screenshots for documentation
│   ├── welcome.png          # Welcome page screenshot
│   ├── login.png            # Login page screenshot
│   ├── register.png         # Registration page screenshot
│   ├── homepage.png         # Homepage/dashboard screenshot
│   ├── profile.png          # User profile screenshot
│   ├── buspass-login.png    # Bus pass login form screenshot
│   └── buspass-display.png  # Bus pass display screenshot
└── README.md


## Database Schema

### Tables
1. *user* - User accounts and authentication
2. *route* - Bus routes with timing and stops
3. *driver* - Driver information and contact details
4. *bus* - Bus details and current locations
5. *bus_pass* - Digital bus passes for users
6. *bus_tracking* - Real-time bus location tracking

## Installation & Setup

### Prerequisites
- Python 3.7+
- MySQL Server
- Web browser (Chrome, Firefox, Safari, Edge)

### Backend Setup

1. *Clone the repository*
   bash
   git clone <repository-url>
   cd bus-tracker
   

2. *Install Python dependencies*
   bash
   pip install flask flask-sqlalchemy flask-cors flask-bcrypt flask-jwt-extended pymysql
   

3. *Configure Database*
   - Create a MySQL database named busTrackingSystem
   - Update database connection string in busSystem.py:
   python
   busSys.config['SQLALCHEMY_DATABASE_URI'] = 'mysql+pymysql://username:password@localhost/busTrackingSystem'
   

4. *Run the Flask application*
   bash
   python busSystem.py
   
   The backend server will start on http://localhost:5000

### Frontend Setup

1. *Serve the HTML files*
   - Use a local web server or open Welcome.html directly in your browser
   - For local server (recommended):
   bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if you have it)
   npx serve .
   

2. *Access the application*
   - Open your browser and navigate to http://localhost:8000/Welcome.html

## Usage Guide

### For Regular Users

1. *Getting Started*
   - Visit the welcome page and click "Login"
   - Create a new account if you don't have one
   - Login with your credentials

2. *Dashboard Features*
   - View real-time bus locations
   - Check route information
   - See driver details
   - Browse all available buses

3. *Digital Bus Pass*
   - Access your bus pass from the navigation menu
   - If logged in, click "View My Bus Pass" for automatic access
   - Alternatively, enter a specific Pass ID to view any pass

4. *Profile Management*
   - View your account information
   - Check your user ID and account status

### For Administrators

1. *Adding Data*
   - Use the API endpoints to add new buses, routes, and drivers
   - Create bus passes for users
   - Update bus tracking information

2. *Managing Users*
   - Monitor user registrations
   - View user details through the API

## Security Features

- *Password Hashing*: All passwords are securely hashed using bcrypt
- *JWT Authentication*: Token-based authentication for secure API access
- *Input Validation*: Frontend and backend validation for all user inputs
- *CORS Protection*: Configured for secure cross-origin requests

  ### 🔧  Further Research / Future Scope
  
- 🔄 Integrate GPS hardware for live automatic bus location updates instead of manual coordinates

- 📱 Develop mobile apps using React Native or Flutter for student & admin access

- 🔔 Push notifications for bus arrival alerts using Firebase or Twilio

- 📊 Admin dashboard for visual analytics of routes, bus utilization, and driver performance

- 🔐 Two-factor authentication (2FA) for enhanced login security

- ☁ Migrate backend to cloud (e.g., AWS, Heroku, or GCP) for better scalability

- 🧾 Online payment gateway for digital bus pass purchase (Stripe, Razorpay etc.)

- 🧮 Auto-assign buses & drivers based on load, timing, and driver availability using algorithms

### ✅ Conclusion
The Online Bus Tracking System provides a reliable and efficient solution to track buses in real time. It reduces the uncertainty of bus arrival times and improves communication between students, drivers, and administrators. By using a user-friendly web interface, the system enables users to view current bus locations, estimated arrival times, and route information.

This project demonstrates how technology can improve daily transportation experiences and ensure better safety and time management for students. With further enhancements like GPS integration and mobile app support, this system can become a fully automated smart transportation solution.
