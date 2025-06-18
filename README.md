<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Botão com Animação</title>
  <style>
    #meuBotao {
      padding: 15px 30px;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 10px;
      font-size: 18px;
      cursor: pointer;
      transition: transform 0.3s, opacity 0.3s;
    }

    #meuBotao.animar {
      transform: scale(0.9);
      opacity: 0.5;
    }
  </style>
</head>
<body>

  <button id="meuBotao">Clique aqui</button>

  <script>
    const botao = document.getElementById('meuBotao');

    botao.addEventListener('click', () => {
      botao.classList.add('animar');
      setTimeout(() => {
        window.location.href = 'https://google.com'; // Troca pelo seu link
      }, 300);
    });
  </script>

</body>
</html>
