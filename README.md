# PHP--hit-counter
php

<?
$file = "stat.txt"; // файл статистики
$f = fopen($file, "r"); // открываем файл статистики
$count = fgets($f, 100); // в переменную записоваеться значение счётчика в файле
fclose($f);
$count++; // увеличиваем значение счётчика на 1
$f = fopen($file, "w"); // открываем файл статистики
fputs($f, $count);
fclose($f);
echo "$count"; // вывод значения счётчика
?>

# file " stat.txt"
