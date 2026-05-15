<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="post" action="">
        Enter a grade (A-F):
        <input type="text" name="grade" required
        value="<?php echo isset($_POST['grade']) ? htmlspecialchars($_POST['grade']) : ''?>">
        <input type="submit">
    </form>
    
    <?php
    switch(isset($_POST['grade']) ? strtoupper($_POST['grade']) : '') {
        case 'A':
            echo "Excellent!";
            break;
        case 'B':
            echo "Good job!";
            break;
        case 'C':
            echo "Average";
            break;
        case 'D':
            echo "Below Average";
            break;
        case 'F':
            echo "Failed";
            break;
        default:
            echo "Invalid grade";
    }
    ?>
</body>
</html>
