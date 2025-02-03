# Chat Application Documentation

## Introduction
This project is a simple and interactive web-based chat application developed using PHP, MySQL, HTML, CSS, and JavaScript. It allows users to communicate in real-time by exchanging text messages.

## Features
- User Authentication (Login and Registration)
- Real-time Messaging
- Profile Management

## File Structure
```
├── .vscode
├── javascript
├── php
│   ├── config.php         # Database configuration
│   └── additional PHP files for backend logic
├── chat.php               # Main chat interface
├── chat.sql               # Database structure and seed data
├── header.php             # Header component
├── index.php              # User Registration page
├── login.php              # User login page
├── user.php               # User profile management
├── style.css              # Styling for the application                
```

## Setup Instructions

### Prerequisites
- WAMP/XAMPP Server
- PHP 7.4 or later
- MySQL Database
- Browser (Chrome, Firefox, etc.)

### Installation Steps
1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   ```

2. **Move to Server Directory:**
   Place the project folder in the `www` or `htdocs` directory of your server.

3. **Database Setup:**
   - Open PHPMyAdmin and create a new database.
   - Import `chat.sql` into the database.

4. **Update Database Configuration:**
   - Edit the file `php/config.php` and update the database credentials:
     ```php
     $conn = mysqli_connect("localhost", "root", "", "chat_db_name");
     ```

5. **Start the Server:**
   - Launch WAMP/XAMPP and start Apache and MySQL services.

6. **Access the Application:**
   - Open your browser and go to `http://localhost/project-folder-name/index.php`

## Usage
1. Register a new user or log in with existing credentials.
2. Select a user to start a chat.
3. Send and receive messages in real-time.

## Troubleshooting
### Common Errors
1. **Undefined array key "user_id":**
   - Ensure that `user_id` is passed correctly in the URL.
2. **Database Connection Errors:**
   - Verify that your database credentials are correct.
3. **Missing Dependencies:**
   - Ensure that the PHP environment is set up correctly.

## Future Enhancements
- Add multimedia file sharing (images, videos, etc.)
- Implement group chat functionality
- Improve security measures (input validation, prepared statements)
- Add typing indicators and message read receipts

