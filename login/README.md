# Login Page

A modern, responsive login page with Firebase Authentication integration.

## Features

- Email/Password authentication
- Remember me functionality
- Forgot password flow
- Social login (Google, GitHub) - requires additional setup
- Responsive design that works on all devices
- Clean and modern UI with smooth animations

## Setup Instructions

1. **Firebase Setup**
   - Go to the [Firebase Console](https://console.firebase.google.com/)
   - Create a new project or select an existing one
   - In the project settings, find your Firebase configuration object
   - Replace the placeholder values in `js/login-app.js` with your actual Firebase config

2. **Enable Authentication Methods**
   - In the Firebase Console, go to Authentication > Sign-in method
   - Enable Email/Password authentication
   - (Optional) Enable Google, GitHub, or other social providers

3. **Update Authorized Domains**
   - In Firebase Console, go to Authentication > Settings > Authorized domains
   - Add your domain (e.g., `localhost` for development)

4. **Customize**
   - Update the colors in `css/login-styles.css` to match your brand
   - Modify the redirect URLs in `js/login-app.js` to point to your app's pages

## File Structure

```
resumetrial/
├── login/
│   ├── index.html         # Login page HTML
├── css/
│   └── login-styles.css   # Login page styles
└── js/
    └── login-app.js       # Firebase authentication logic
```

## Usage

1. Open `login/index.html` in a web server (don't open directly as a file)
2. Test the login functionality with a user account created in Firebase

## Security Notes

- Never commit your Firebase config with real API keys to version control
- Make sure to set up proper security rules in Firebase
- Always use HTTPS in production

## License

This project is open source and available under the [MIT License](LICENSE).
