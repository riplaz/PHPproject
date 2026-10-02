# PHPproject

<?php
echo "<pre>";

echo "     0    1    2    3    4    5    6    7    8    9\n\n";

for ($tens = 0; $tens <= 9; $tens++) {
    
    echo $tens . "    ";
    
    for ($units = 0; $units <= 9; $units++) 
    {
        $number = ($tens * 10) + $units;
        $square = $number * $number;
        
        echo $square;
        
        if ($square < 10) {
            echo "    ";
        } elseif ($square < 100) {
            echo "   ";
        } elseif ($square < 1000) {
            echo "  ";
        } else {
            echo " ";
        }
    }
    
    echo "\n";
}

echo "</pre>";
?>
