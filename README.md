<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Convite</title>
    <style>
        button {
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>Daniel, aceita sair comigo?</h1>
    <button id="simButton">Sim</button>
    <button id="naoButton">Não</button>

    <script>
        const simButton = document.getElementById('simButton');
        const naoButton = document.getElementById('naoButton');

        simButton.addEventListener('click', () => {
            alert('Oba! Você aceitou!');
            window.location.href = 'https://www.youtube.com/watch?v=izGwDsrQ1eQ';
        });

        naoButton.addEventListener('mouseover', () => {
            const newX = Math.random() * (window.innerWidth - naoButton.offsetWidth);
            const newY = Math.random() * (window.innerHeight - naoButton.offsetHeight);
            naoButton.style.left = newX + 'px';
            naoButton.style.top = newY + 'px';
        });
    </script>
</body>
</html>
