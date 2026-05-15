<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    Enter a day number (1-7):
    <form method="post" action="">
        <input type="number" name="day" required
        value="<?php echo isset($_POST['day']) ? htmlspecialchars($_POST['day']) : ''?>"><br>
        <input type="submit">
    </form>

    <?php
    $day = isset($_POST['day']) ? (int)$_POST['day'] : 0;

    switch($day) {
        case 1:
            echo "Today is Monday";
            break;
        case 2:
            echo "Today is Tuesday";
            break;
        case 3:
            echo "Today is  Wednesday";
            break;
        case 4:
            echo "Today is Thursday";
            break;
        case 5:
            echo "Today is Friday";
            break;
        case 6:
            echo "Today is Saturday";
            break;
        case 7:
            echo "Today is Sunday";
            break;
        default:
            echo "Invalid day";
    }
    ?>
</body>
</html>
