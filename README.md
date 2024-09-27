<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Animación para mi Enamorado</title>
  <style>
    body {
      background-color: #f0f8ff;
      font-family: 'Arial', sans-serif;
      text-align: center;
    }

    h1 {
      color: #003366;
    }

    .road {
      width: 100%;
      height: 200px;
      background: linear-gradient(#555, #333);
      position: relative;
      margin: 50px 0;
    }

    .car {
      width: 100px;
      height: 50px;
      background: red;
      border-radius: 10px;
      position: absolute;
      top: 50px;
      left: -100px;
      animation: drive 10s linear infinite;
    }

    .car::before {
      content: '';
      position: absolute;
      top: 35px;
      left: 10px;
      width: 20px;
      height: 20px;
      background: black;
      border-radius: 50%;
    }

    .car::after {
      content: '';
      position: absolute;
      top: 35px;
      right: 10px;
      width: 20px;
      height: 20px;
      background: black;
      border-radius: 50%;
    }

    @keyframes drive {
      from {
        left: -100px;
      }
      to {
        left: 100%;
      }
    }

    .poem {
      font-size: 20px;
      color: #003366;
      margin-top: 30px;
      line-height: 1.6;
    }

    .heart {
      color: red;
    }
  </style>
</head>
<body>
  <h1>Para mi amor, que siempre conduce mi corazón</h1>
  
  <div class="road">
    <div class="car"></div>
  </div>

  <div class="poem">
    <p>Como un coche que avanza sin parar,</p>
    <p>Mi amor por ti no deja de acelerar,</p>
    <p>En el mundo de sistemas y lógica sin fin,</p>
    <p>Tu amor es el código que siempre me hace sentir.</p>
    <p>Eres la constante en mi ecuación de la vida,</p>
    <p>El ingeniero de mi corazón, con suavidad tan querida.</p>
    <p>Que esta ruta nos lleve siempre más allá,</p>
    <p>Te amo hoy, mañana, y por toda la eternidad <span class="heart">&hearts;</span></p>
  </div>
</body>
</html>
