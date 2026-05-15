<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="post" action="">
        Enter a password:
        <input type="password" name="password" required
        value="<?php echo isset($_POST['password']) ? htmlspecialchars($_POST['password']) : ''?>">

        <input type="submit" value="Login">
    </form>


    <?php
    $fixedpassword = "admin123";
    
    if(isset($_POST['password'])) {
        $userpassword = $_POST['password'];
        
        if($userpassword == $fixedpassword) {
            echo "Access Granted";
        } else {
            echo "Access Denied";
        }
    }
    ?>
</body>
</html>
