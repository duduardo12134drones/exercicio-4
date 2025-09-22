<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Faixa Etária</title>
</head>
<body>
    <h1>Verificação de Faixa Etária</h1>

    <script>
        var anoNascimento = prompt("Digite seu ano de nascimento:");
        anoNascimento = parseInt(anoNascimento);
        var idade = new Date().getFullYear() - anoNascimento;
        var faixaEtaria;
        if (idade >= 0 && idade <= 12) {
            faixaEtaria = "Criança";
        } else if (idade >= 13 && idade <= 24) {
            faixaEtaria = "Jovem";
        } else if (idade >= 25 && idade <= 59) {
            faixaEtaria = "Adulto";
        } else if (idade >= 60) {
            faixaEtaria = "Idoso";
        } else {
            faixaEtaria = "Idade inválida";
        }
        alert("Você tem " + idade + " anos e é " + faixaEtaria + ".");
    </script>
</body>
</html>
