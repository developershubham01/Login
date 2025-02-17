# Login
# Animated Login Page

This is a simple animated login page using HTML, CSS, and JavaScript.

## How to Use
1. Clone or download this repository.
2. Open `index.html` in your browser.
3. Enter your username and password, then click the login button.

## Code
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Login Page</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(to right, #ad7f73, #161615);
            font-family: Arial, sans-serif;
        }
        .container {
            background: rgba(61, 61, 85, 0.11);
            padding: 50px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(104, 71, 71, 0.1);
            width: 300px;
            text-align: center;
            transform: scale(0.8);
            transition: transform 0.5s ease-in-out;
        }
        .container.active {
            transform: scale(1);
        }
        h2 {
            margin-bottom: 20px;
        }
        input {
            width: 60%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #0e0b0b;
            border-radius: 5px;
        }
        button {
            width: 50%;
            padding: 10px;
            background: #110d0c;
            border: none;
            color: rgb(243, 238, 238);
            font-size: 10px;
            cursor: pointer;
            border-radius: 5px;
            transition: background 0.3s;
        }
        button:hover {
            background: #feb47b;
        }
    </style>
</head>
<body>
    <div class="container" id="loginBox">
        <h2>Hi! Login</h2>
        <h6>Welcome to GitHub</h6>
        <input type="text" placeholder="Username" id="username">
        <input type="password" placeholder="Password" id="password">
        <button onclick="login()">Login</button>
    </div>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            document.getElementById("loginBox").classList.add("active");
        });
        function login() {
            alert("Login button clicked!");
        }
    </script>
</body>
</html>
```

## Developer
Shubham Sharma

