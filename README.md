<!DOCTYPE html>
<html>
<head>
    <title>Redirecionamento com base no número digitado</title>
    <script>
        function redirecionarPagina() {
            var numero = document.getElementById("numero").value;
            var url = numero + ".html";
            window.location.href = url;
            return false; // Impede o envio padrão do formulário
        }
    </script>
</head>
<body>
    <h1>Digite um número da matricula e pressione o botão "Submit"</h1>
    <form onsubmit="return redirecionarPagina()">
        <label for="numero">Número:</label>
        <input type="text" id="numero" name="numero" required>
        <input type="submit" value="Submit">
    </form>
</body>
</html>
