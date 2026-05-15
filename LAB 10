<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="post">
    Username:
    <input type="text" name="username" required
    value="<?php echo isset($_POST['username']) ? htmlspecialchars($_POST['username']) : ''; ?>"><br><br>

    Password:
    <input type="password" name="password" required><br><br>

    <input type="submit" value="Login">

    <?php
    $username = "admin";
    $password = "1234";

    if ($_SERVER["REQUEST_METHOD"] == "POST") {

        $user = $_POST["username"];
        $pass = $_POST["password"];

        if ($user == $username && $pass == $password) {
        echo "Login Successful";
        } else {
        echo "Invalid Username or Password";
        }
    }
    ?>
</form>
</body>
</html>
