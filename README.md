1 -
<?php
$nome = "Maria";
$sexo = "feminino";
$idade = 22;

if ($sexo == "feminino" && $idade < 25) {
  echo "$nome - ACEITA";
} else {
  echo "$nome - NÃO ACEITA";
}
?>

2 - 
<?php
$livro = "Dom Casmurro";
$tipo = "aluno";

if ($tipo == "professor") {
  $dias = 10;
} else {
  $dias = 3;
}

echo "Livro: $livro<br>";
echo "Usuário: $tipo<br>";
echo "Devolução em: " . date("d/m/Y", strtotime("+$dias days"));
?>

3 - 
<?php
$alturaChico = 1.50;
$alturaJuca = 1.10; 
$crescimentoChico = 0.02;
$crescimentoJuca = 0.03; 
$anos = 0;

while ($alturaJuca <= $alturaChico) {
    $alturaChico += $crescimentoChico;
    $alturaJuca += $crescimentoJuca;
    $anos++;
}

echo "Serão necessários $anos anos para que Juca seja maior que Chico.";
?>
