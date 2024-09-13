<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EarnWithViews - Investment Platform</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        /* Add your styles here */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 1rem;
            text-align: center;
        }
        nav ul {
            list-style-type: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin: 0 10px;
        }
        nav ul li a {
            color: #fff;
            text-decoration: none;
        }
        main {
            padding: 2rem;
        }
        section {
            margin-bottom: 2rem;
        }
        button {
            background-color: #333;
            color: #fff;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
        }
        button:hover {
            background-color: #555;
        }
        .whatsapp-btn {
            display: inline-block;
            padding: 10px 20px;
            margin-top: 20px;
            background-color: #25D366; /* WhatsApp Green */
            color: #fff;
            border: none;
            border-radius: 5px;
            text-align: center;
            text-decoration: none;
            font-size: 16px;
        }
        .whatsapp-btn:hover {
            background-color: #128C7E;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #333;
            color: #fff;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to EarnWithViews</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#signup">Sign Up</a></li>
                <li><a href="#login">Login</a></li>
                <li><a href="#payment">Make a Payment</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Invest with EarnWithViews</h2>
            <p>Start investing your money and earn daily rewards with EarnWithViews!</p>
        </section>

        <section id="about">
            <h2>About EarnWithViews</h2>
            <p>EarnWithViews provides a platform where users can securely invest their money and earn daily profits.</p>
        </section>

        <section id="signup">
            <h2>Create an Account</h2>
            <form action="register.php" method="post">
                <label for="username">Username:</label>
                <input type="text" id="username" name="username" required><br>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required><br>
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" required><br>
                <button type="submit">Sign Up</button>
            </form>
        </section>

        <section id="login">
            <h2>Login</h2>
            <form action="login.php" method="post">
                <label for="login-username">Username:</label>
                <input type="text" id="login-username" name="username" required><br>
                <label for="login-password">Password:</label>
                <input type="password" id="login-password" name="password" required><br>
                <button type="submit">Login</button>
            </form>
        </section>

        <section id="payment">
            <h2>Make a Payment with M-Pesa</h2>
            <form action="mpesa_payment.php" method="post">
                <label for="phone">M-Pesa Phone Number:</label>
                <input type="tel" id="phone" name="phone" required pattern="[0-9]{10}" placeholder="Enter your phone number"><br>
                <label for="amount">Amount to Invest (in KES):</label>
                <input type="number" id="amount" name="amount" required><br>
                <button type="submit">Pay with M-Pesa</button>
            </form>
        </section>
        
        <!-- WhatsApp Contact Button -->
        <section>
            <h2>Contact Us</h2>
            <a href="https://wa.me/0700698204" class="whatsapp-btn" target="_blank">Contact Us on WhatsApp</a>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 EarnWithViews. All rights reserved.</p>
        <p>Follow us on social media:</p>
        <a href="https://x.com/marcustaxlord?t=YNTi98tG3YAYiTYNHLpbEA&s=09" target="_blank">Twitter</a>
    </footer>
</body>
</html>
