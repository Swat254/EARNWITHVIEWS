<!DOCTYPE html>
<html>
<head>
    <title>User Dashboard</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f7f6;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            color: #333;
        }

        #auth, #dashboard {
            background-color: #fff;
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: 400px;
            text-align: center;
        }

        h1 {
            color: #007bff;
            margin-bottom: 20px;
        }

        input[type="text"], input[type="password"], input[type="file"], textarea {
            width: calc(100% - 22px);
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }

        button {
            background-color: #007bff;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin: 10px 0;
            width: 100%;
        }

        button:hover {
            background-color: #0056b3;
        }

        img#profilePic {
            max-width: 150px;
            border-radius: 50%;
            margin-bottom: 20px;
        }

        textarea {
            height: 150px;
        }

        #referralLink {
            background-color: #e9ecef;
            padding: 8px;
            border-radius: 4px;
            display: inline-block;
            margin-bottom: 20px;
        }

    </style>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            document.getElementById('loginButton').addEventListener('click', function() {
                alert("Login functionality needs backend implementation.");
            });

            document.getElementById('registerButton').addEventListener('click', function() {
                alert("Register functionality needs backend implementation.");
                showDashboard();
            });

            document.getElementById('logoutButton').addEventListener('click', function() {
                document.getElementById('auth').style.display = 'block';
                document.getElementById('dashboard').style.display = 'none';
            });

            document.getElementById('shareButton').addEventListener('click', function() {
                alert("Share functionality needs backend implementation or sharing API.");
            });

            document.getElementById('profilePicUpload').addEventListener('change', function() {
                alert("Profile picture upload needs backend implementation.");
            });
        });

        function showDashboard() {
            document.getElementById('auth').style.display = 'none';
            document.getElementById('dashboard').style.display = 'block';
            document.getElementById('profilePic').src = "placeholder.jpg";
            document.getElementById('referralLink').textContent = "yourreferral.com/user123";
        }
    </script>
</head>
<body>
    <div id="auth">
        <h1>Login / Register</h1>
        <input type="text" id="username" placeholder="Username">
        <input type="password" id="password" placeholder="Password">
        <button id="loginButton">Login</button>
        <button id="registerButton">Register</button>
    </div>
    <div id="dashboard" style="display: none;">
        <h1>User Dashboard</h1>
        <img id="profilePic" src="" alt="Profile Picture">
        <input type="file" id="profilePicUpload">
        <p>Referral Link: <span id="referralLink"></span></p>
        <textarea id="shareText"></textarea>
        <button id="shareButton">Share</button>
        <button id="logoutButton">Logout</button>
    </div>
</body>
</html>
