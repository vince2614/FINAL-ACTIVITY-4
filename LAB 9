<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="post" action="">
        Purchase Amount:
        <input type="number" name="amount" required 
        value="<?php echo isset($_POST['amount']) ? htmlspecialchars($_POST['amount']) : ''; ?>"><br><br>

        <input type="submit">
    </form>

    <?php
    if($_SERVER["REQUEST_METHOD"] == "POST") {

        $amount = $_POST['amount'];
        $discount = 0;

        if($amount >= 1000) {
            $discount = $amount * 0.20;
        } elseif ($amount >= 500) {
            $discount = $amount * 0.10;
        } else {
            $discount = 0;
        }

        $finalAmount = $amount - $discount;

        echo "Original Amount: $" . number_format($amount, 2) . "<br>";
        echo "Discount: $" . number_format($discount, 2) . "<br>";
        echo "Final Amount: $" . number_format($finalAmount, 2);
    }
    ?>
</body>
</html>
