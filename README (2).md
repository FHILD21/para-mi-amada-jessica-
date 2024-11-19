<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mensaje Especial</title>
  <style>
    .message {
      font-size: 24px;
      margin: 20px;
      font-weight: bold;
      text-align: center;
    }
    .buttons {
      margin-top: 20px;
      text-align: center;
    }
    .button {
      font-size: 18px;
      padding: 10px 20px;
      margin: 10px;
      color: white;
      background-color: #4CAF50;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      text-decoration: none;
    }
    .button.no {
      background-color: #f44336;
    }
  </style>
</head>
<body>
  <div style="text-align: center;">
    <h1>Un Mensaje para Ti MI FUTURA ESPOSITA💓</h1>
  </div>
  
  <img src="https://i.imgur.com/JHTocYe.gif" alt="Oso pidiendo perdón" style="display: block; margin: 0 auto;">
  
  <div class="message">¿ME PERDONAS MI AMORCITA HERMOSA??</div>
  
  <div class="buttons">
    <a href="#" id="yesButton" class="button">Sí</a>
    <a href="#" id="noButton" class="button no">No</a>
  </div>

  <script>
    // Al hacer clic en el botón "Sí"
    document.getElementById('yesButton').addEventListener('click', function(event) {
      event.preventDefault(); // Evita que se siga el enlace
      // Abre una nueva ventana con el mensaje y el nuevo GIF
      window.open('data:text/html,<html><body style="text-align: center; font-family: Arial, sans-serif;"><h1>Gracias mi amorcito, te amo y te amaré siempre 💖</h1><img src="https://i.imgur.com/a5aJQvU.gif" alt="Te Amo GIF" style="width: 200px;"><br><p>Te amo muchísimo!</p></body></html>', '_blank');
    });

    // Al hacer clic en el botón "No"
    let noButtonClickCount = 0; // Contador para aumentar el tamaño de la letra en "No"
    
    document.getElementById('noButton').addEventListener('click', function(event) {
      event.preventDefault(); // Evita que se siga el enlace
      noButtonClickCount++; // Aumenta el contador
      // Abre una nueva ventana con el mensaje y el nuevo GIF de "No"
      window.open('data:text/html,<html><body style="text-align: center; font-family: Arial, sans-serif;"><h1>¿Segura?</h1><img src="https://i.imgur.com/wXq6hIn.gif" alt="Seguro GIF" style="width: 200px;"><br><div class="buttons"><a href="#" id="yesButton" class="button">Sí</a><a href="#" id="noButton" class="button no" style="font-size: ' + (18 + noButtonClickCount * 5) + 'px;">No</a></div></body></html>', '_blank');
    });
  </script>
</body>
</html>
