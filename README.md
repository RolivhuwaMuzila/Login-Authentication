# Login Authentication System

## Project Overview

This project is a basic Login Authentication System built using HTML, CSS, and JavaScript. It allows users to register with a username and password, log in with their credentials, and access a secure page that only logged-in users can view. The system does not persist data and is intended for demonstration purposes.

## Features

- **User Registration**: Users can register with a unique username and password.
- **User Login**: Registered users can log in using their credentials.
- **Secure Page**: Logged-in users can access a secure page.
- **Logout Functionality**: Users can log out, which will hide the secure page and return them to the login form.
- **Switch Between Forms**: The interface allows users to switch between the login and registration forms seamlessly.

## Technologies Used

- **HTML**: Structure of the application.
- **CSS**: Basic styling of the forms and layout.
- **JavaScript**: Core functionality for registration, login, and navigation between different forms.

## How It Works

### Registration Process
1. Users can click on the "Register" link to switch to the registration form.
2. The registration form allows users to enter a username and password.
3. Upon clicking the "Register" button, the credentials are stored in a local array (`users`).
4. If both fields are filled in, a success message is displayed; otherwise, the user is prompted to fill in all fields.

### Login Process
1. Users can switch back to the login form using the "Login" link.
2. After entering their credentials, the system checks if the username and password match an existing entry in the `users` array.
3. If the credentials are valid, the user is logged in, and the secure page is displayed.
4. If the credentials are invalid, an error message is shown.

### Secure Page
- Once logged in, users can view the secure page that includes a welcome message and a logout button.
- The secure page remains hidden until a successful login occurs.

### Logout
- Clicking the "Logout" button will log the user out by hiding the secure page and returning them to the login form.
- The input fields are reset, and any login messages are cleared.

## How to Use

1. **Open the HTML file** in any modern web browser.
2. **Register** a new account by clicking on the "Register" link.
3. **Login** using the registered credentials.
4. Upon successful login, you'll see the secure page.
5. You can **logout** to return to the login page.

## Limitations

- This project does not use persistent storage. User information is stored temporarily in memory (i.e., the `users` array). If the page is refreshed, all data is lost.
- There is no encryption for passwords, making it unsuitable for production environments.
- The system does not handle duplicate usernames, meaning that users could register multiple accounts with the same username.

## Future Improvements

- **Add Persistent Storage**: Use localStorage or integrate a backend to store user data.
- **Password Encryption**: Encrypt passwords to enhance security.
- **Handle Duplicate Usernames**: Add functionality to prevent the registration of duplicate usernames.
- **Validation**: Improve form validation to handle empty inputs, invalid characters, or password strength checks.

## License
This project is free to use and modify. Feel free to extend it with additional features and improvements.
