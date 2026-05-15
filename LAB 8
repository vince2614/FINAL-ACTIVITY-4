<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="post" action="">
        Enter your age:
        <input type="number" name="age" required
        value="<?php echo isset($_POST['age']) ? htmlspecialchars($_POST['age']) : ''?>"><br><br>

        Citizenship:
        <input type="text" name="citizenship" required
        value="<?php echo isset($_POST['citizenship']) ? htmlspecialchars($_POST['citizenship']) : ''?>"><br>

        <input type="submit">
    </form>

    <?php
    if($_SERVER["REQUEST_METHOD"] == "POST") {

    $age = $_POST['age'];
    $citizenship = $_POST['citizenship'];

    if($age >= 18) {

        if (strtolower($citizenship) == "filipino") {
            echo "Eligible to vote";
        } else {
            echo "Not eligible to vote";
        }

      } else {
        echo "Not eligible to vote";
      }
    }

    ?>
</body>
</html>
