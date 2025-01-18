# Dynamic Portal  
This web portal was developed as part of my Summer 2019 internship.  

---

## Website on Localhost Using XAMPP, CSS, and PHP  

This website is built on a localhost using XAMPP and includes key features such as:  
- CAPTCHA integration.  
- Sending OTP and password reset links via Gmail.  

---

### Prerequisites  
To set up this website, you will need the following:  
1. **XAMPP**: Includes Apache and MySQL, which are essential for running the website.  
2. **Text Editor**: Any code editor like Notepad++, Sublime Text, or Atom.  

---

### About the Website  
This website is hosted on a localhost using **XAMPP**:  
- **XAMPP**: Stands for Cross-Platform (X), Apache (A), MariaDB (M), PHP (P), and Perl (P).  
  - **Apache**: A widely-used web server that processes HTTP requests and serves the requested web pages.  
  - **PHP**: A programming language for creating dynamic web content that interacts with databases.

---

### Features  
1. **Registration Page**:  
   - Users must register with details.  
   - Passwords require special characters and numbers.  
   - Phone numbers must have 10 digits.  

2. **Login Page**:  
   - Enter credentials and complete CAPTCHA verification.  
   - Errors are shown for incorrect credentials.  

3. **Forgot Password Option**:  
   - Sends a password reset link to the registered email.  
   - The link expires within **24 hours**.  

4. **Security Features**:  
   - After **3 failed login attempts**, a confirmation email is sent.  
   - An OTP is required for login confirmation.  

5. **Password Reset**:  
   - Users can reset their password through the emailed link.  

---

### Steps to Set Up  
1. **Download Required Software**:  
   - Install XAMPP.  
   - Use any text editor like Notepad++, Sublime Text, or Atom.  

2. **Run the Website**:  
   - Start by running the `register.php` file using the URL: `localhost/websiteproject/register.php`.  

---

### File Descriptions  
Below is a summary of the main files and their functions:  

1. **register.php**: Generates a registration page with a link to the login page if already registered.  
2. **login.php**: Generates the login page for entering credentials.  
3. **index.php**: Displays a welcome page after successful login. Includes a logout option to end the session.  
4. **errors.php**: Handles errors such as:  
   - Empty username or email fields.  
   - Password mismatch during registration.  
   - Duplicate username or email.  
5. **captcha.php**: Generates a new CAPTCHA each time the page reloads.  
6. **mailfornewpassword.php**: Handles the "Forgot Password" feature by accepting an email address to send a password reset link.  
7. **newpassword.php**: Allows users to reset their password using the emailed link.  
8. **sendmail.php**: Sends the password reset email containing the reset link.  
9. **server.php**: Manages server-side operations, including:  
   - Data retrieval and user registration.  
   - Error handling.  
10. **style_new3.css**: Contains all CSS styling for the website.  
11. **congrats_new_register.php**: Displays a congratulatory page for successful registration.  
12. **linkexpire.php**: Informs users that the password reset link has expired after 24 hours.  
13. **mail_suspectsent.php**: Triggered after 3 failed login attempts, prompting users to enter their registered email for confirmation.  
14. **sendmail_suspectentry.php**: Sends a confirmation email to users after they provide their registered email.  

---

### How to Use the Website  
1. Run the `register.php` file to start the registration process.  
2. Login using your credentials via `login.php`.  
3. If you forget your password, use the "Forgot Password" feature to receive a reset link.  
4. For errors or failed login attempts, follow the instructions in the confirmation emails.  

---

### Notes  
- All the necessary code files are included. Simply run them in the specified order for the website to function properly.  
- XAMPP's built-in Apache and MySQL services handle server-side operations.  
- Ensure that email services (like Gmail) are configured correctly to enable OTP and password reset features.  

Happy coding! 🚀
