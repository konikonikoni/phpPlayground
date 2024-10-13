# TODO for phpPlayground

## 1. User Registration Form
- [ ] Create a PHP form that allows users to register by entering:
    - Email
    - Nickname
    - Password (hashed securely)
    - Role (optional, e.g., user/admin)

### Steps:
- [ ] Set up a basic HTML form.
- [ ] Add form validation (server-side and client-side).
- [ ] Implement password hashing using `password_hash()` for security.

## 2. MySQL Database Setup
- [ ] Set up a MySQL database to store user information.
- [ ] Create a table `users` with the following columns:
    - `id` (INT, primary key, auto-increment)
    - `email` (VARCHAR, unique)
    - `nickname` (VARCHAR, unique)
    - `role` (VARCHAR, e.g., 'user', 'admin')
    - `password` (VARCHAR, hashed password)
    - `session_token` (VARCHAR, optional for session handling)

### Steps:
- [ ] Write the SQL to create the table and fields.
- [ ] Use PHP's PDO to connect to MySQL and interact with the database.

## 3. User Session Management (Optional)
- [ ] Consider using a `session_token` for secure user sessions.
- [ ] Implement secure session handling with PHP sessions.

## 4. Additional Security Considerations
- [ ] Implement CSRF protection for the registration form.
- [ ] Add email validation and sanitization.
- [ ] Ensure SQL queries are protected against SQL injection (use prepared statements).

## 5. Testing
- [ ] Write basic test cases to ensure user registration works.
- [ ] Verify secure password hashing and session handling.