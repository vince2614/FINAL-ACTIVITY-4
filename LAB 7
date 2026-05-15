<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="post" action="">
        Enter a year:
        <input type="number" name="year" required
        value="<?php echo isset($_POST['year']) ? htmlspecialchars($_POST['year']) : ''?>">

        <input type="submit">
    </form>
    
    <?php
    if($_SERVER["REQUEST_METHOD"] == "POST") {

        $year = $_POST['year'];

        if($year % 4 == 0 && $year % 100 != 0 || ($year % 400 == 0)) {
            echo $year . " is a leap year.";
        } else {
            echo $year . " is not a leap year.";
        }
    }
    ?>
</body>
</html>
