<?php
function maior($a, $b) {
    return (($a + $b + abs($a - $b)) / 2);
}

function maior_tres($a, $b, $c) {
    return maior(maior($a, $b), $c);
}

$entrada = readline();
$valores = explode(" ", $entrada);

$a = (int)$valores[0];
$b = (int)$valores[1];
$c = (int)$valores[2];

$maior= maior_tres($a, $b, $c);

echo $maior. " eh o maior\n";
?>
