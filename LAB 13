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
        <input type="number" name="num1" required
        value="<?php echo isset($_POST['num1']) ? htmlspecialchars($_POST['num1']) : ''?>"><br><br>
        Enter the second number:
        <input type="number" name="num2" required
        value="<?php echo isset($_POST['num2']) ? htmlspecialchars($_POST['num2']) : ''?>">
        <br><br>
        <input type="submit" value="Calculate">

        Operator:
        <select name="operator" required>
            <option value="+">+</option>
            <option value="-">-</option>
            <option value="*">*</option>
            <option value="/">/</option>
        </select><br><br>
    </form>

    <?php
    if ($_SERVER["REQUEST_METHOD"] == "POST") {
        $num1 = $_POST['num1'];
        $num2 = $_POST['num2'];
        $operator = $_POST['operator'];
        
        switch ($operator) {
            case '+':
                $result = $num1 + $num2;
                break;
            case '-':
                $result = $num1 - $num2;
                break;
            case '*':
                $result = $num1 * $num2;
                break;
            case '/':
                if ($num2 != 0) {
                    $result = $num1 / $num2;
                } else {
                    echo "Cannot divide by zero.";
                    exit;
                }
                break;
            default:
                echo "Invalid operator.";
                exit;
        }

        echo "Result: " . $result;
    }
    ?>
</body>
</html>
