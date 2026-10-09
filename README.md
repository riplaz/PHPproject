# PHPproject

<?php
echo "<pre>";

echo "┌───┬" . str_repeat("──────┬", 9) . "──────┐\n";

echo "│   │";
for ($units = 0; $units <= 9; $units++) {
    printf("  %d   │", $units);
}
echo "\n";

for ($tens = 0; $tens <= 9; $tens++) {

    echo "├───┼" . str_repeat("──────┼", 9) . "──────┤\n";
    
    printf("│ %d │", $tens);
    
    for ($units = 0; $units <= 9; $units++) {
        $number = ($tens * 10) + $units;
        $square = $number * $number;
        
        printf(" %-4d │", $square);
    }
    
    echo "\n";
}

echo "└───┴" . str_repeat("──────┴", 9) . "──────┘\n";

echo "</pre>";
?>
