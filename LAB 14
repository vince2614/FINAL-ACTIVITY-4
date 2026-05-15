<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="post" action="">
        Menu (1-3):
        <input type="number" name="menu" required
        value="<?php echo isset($_POST['menu']) ? htmlspecialchars($_POST['menu']) : ''?>">
        <input type="submit" value="Submit">
    </form>

    <?php
    switch(isset($_POST['menu']) ? $_POST['menu'] : '') {
        case '1':
            echo "Add.";
            break;
        case '2':
            echo "Edit.";
            break;
        case '3':
            echo "Delete.";
            break;
        default:
            echo "Invalid selection.";
    }
    ?>
</body>
</html>
