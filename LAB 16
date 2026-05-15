<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form action="" method="post">
        Enter a color:
        <input type="text" name="color" required
        value="<?php echo isset($_POST['color']) ? htmlspecialchars($_POST['color']) : ''?>">
        <input type="submit" value="Submit">
    </form>

    <?php
    switch(isset($_POST['color']) ? $_POST['color'] : '') {
        case 'red':
            echo "Stop.";
            break;
        case 'yellow':
            echo "Caution.";
            break;
        case 'green':
            echo "Go.";
            break;
        default:
            echo "Invalid color.";
    }
    ?>
</body>
</html>
