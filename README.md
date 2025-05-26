# Bus Tracking and User Management System (Flask)

## 1. Project Content

This project is a simple bus tracking system combined with user registration and login functionality built using Flask. Users can register, log in, view their profile details in a table format, and track bus locations on a map on the homepage.

## 2. Project Code

- `bus_system.py` : Flask backend handling routes for registration, login, logout, and homepage.
- `register.html` : User registration form with fields for username, email, phone, and address.
- `login.html` : User login form.
- `homepage.html` : Homepage displaying logged-in user profile in a table and embedded Google Map for bus tracking.
- `welcome1.html` : (Optional) Landing or welcome page.

## 3. Key Technologies

- **Flask**: Lightweight Python web framework used for backend.
- **Python**: Programming language.
- **HTML/CSS**: Frontend structure and styling.
- **JavaScript & Google Maps API**: For displaying bus locations on map.
- **SQLite**: Database for storing user credentials and profile data (can be swapped for others).

## 4. Description

This Flask application provides:

- User registration with extended profile fields (phone, address).
- Secure user login with session management.
- Homepage that displays user profile details in a table.
- Real-time bus tracking on a Google Map embedded in the homepage.
- Logout functionality.

The backend handles form submissions, database interactions, and session control. The frontend presents a user-friendly interface and a dynamic map for tracking buses.

## 5. Output

- **Registration Page**: Form to create a new user.
- **Login Page**: Form for user authentication.
- **Homepage**:
  - Displays user details (username, email, phone, address) in a table.
  - Shows bus locations on a Google Map.
- **Logout**: Button to securely end the session.

### Example Profile Table on Homepage

| Username | Email           | Phone      | Address          |
|----------|-----------------|------------|------------------|
| john123  | john@example.com| 1234567890 | 123 Main Street  |

*(Below the table, a map shows current bus positions.)*

## 6. Further Research

- Integrate real-time GPS data for live bus updates.
- Implement user roles (admin, driver, passenger).
- Add push notifications for bus arrivals or delays.
- Develop mobile-friendly UI or native mobile app.
- Add analytics on bus routes and user activity.
- Enhance security with password hashing, HTTPS, and session timeout.

---

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
