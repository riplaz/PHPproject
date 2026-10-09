<!DOCTYPE html>
<html>
<head>
    <title>Таблица квадратов</title>
    <meta charset="utf-8" />
</head>

<body>

<table border="1" cellpadding="5">

    <tr>
        <th>+</th>
        <th>0</th>
        <th>1</th>
        <th>2</th>
        <th>3</th>
        <th>4</th>
        <th>5</th>
        <th>6</th>
        <th>7</th>
        <th>8</th>
        <th>9</th>
    </tr>
    
    <?php
    for ($i = 0; $i < 10; $i++)
    {
        echo "<tr>";
        

        echo "<th>" . ($i * 10) . "</th>";
        
        for ($j = 0; $j < 10; $j++)
        {
            $num = $i * 10 + $j;
            echo "<td>" . ($num * $num) . "</td>";
        }
        
        echo "</tr>";
    }
    ?>
</table>

</body>
</html>
