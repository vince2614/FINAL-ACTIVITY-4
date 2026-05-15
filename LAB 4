<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form  method="post" action="">
        Enter a number: 
        <input type="number" name="number" 
        value="<?php echo isset($_POST['number']) ? htmlspecialchars($_POST['number']) : ''; ?>">
        <input type="submit">
    </form>

    <?php
    if(isset($_POST['number'])) {
        $number = $_POST['number'];

        if($number % 2 == 0) {
            echo "Even";
        } else {
            echo "Odd";
        }
    }
    ?>
</body>
</html>
