<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form  method="post" action="">
        Enter Student Grade: 
        <input type="number" name="grade" max="100"
        value="<?php echo isset($_POST['grade']) ? htmlspecialchars($_POST['grade']) : ''; ?>">
        <input type="submit">
    </form>

    <?php
    if(isset($_POST['grade'])) {
        $grade = $_POST['grade'];

        if($grade >= 90 && $grade <= 100) {
            echo "Excellent";
        } elseif ($grade >= 80) {
            echo "Good";
        } elseif ($grade >= 70) {
            echo "Average";
        } else {
            echo "Failed";
        }      
    }
    ?>
</body>
</html>
