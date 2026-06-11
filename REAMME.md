# Patogrills Admin Panel 🔐

## Secure Admin Access System

This is a password-protected admin panel for managing Patogrills food ordering system.

## 🔧 Setup Instructions for Local Use:

### First Time Setup (One Time Only):

1. Clone this repository
2. Create a file called `admin-login.html` (DO NOT use the one from GitHub - create your own)
3. Add this code to your local `admin-login.html`:
   ```html
   <!DOCTYPE html>
   <html>
   <head><title>Admin Setup</title></head>
   <body>
   <script>
       const password = prompt("Create admin password:");
       if(password) {
           localStorage.setItem('adminAuth', btoa(password));
           alert("Setup complete! Go to admin.html and login with: " + password);
           window.location.href = 'admin.html';
       }
   </script>
   </body>
   </html>