<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="post" action="">
        Enter the first number:
        <input type="number" name="num1" value="<?php echo isset($_POST['num1']) ? htmlspecialchars($_POST['num1']) : ''; ?>"><br><br>

        Enter the second number:
        <input type="number" name="num2" value="<?php echo isset($_POST['num2']) ? htmlspecialchars($_POST['num2']) : ''; ?>"><br><br>

        Enter the third number:
        <input type="number" name="num3" value="<?php echo isset($_POST['num3']) ? htmlspecialchars($_POST['num3']) : ''; ?>"><br><br>

        <input type="submit">
    </form>

    <?php
    if($_SERVER["REQUEST_METHOD"] == "POST") {
        $num1 = $_POST['num1'];
        $num2 = $_POST['num2'];
        $num3 = $_POST['num3'];

        if($num1 >= $num2 && $num1 >= $num3) {
            $largest = $num1;
        } elseif ($num2 >= $num1 && $num2 >= $num3) {
            $largest = $num2;
        } else {
            $largest = $num3;
        }

        echo "The largest number is: " . $largest;
    }
    ?>


</body>
</html>
