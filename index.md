<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Jet-Bomb: Order or Die</title>
  <style>
    body {
      background-color: black;
      color: white;
      font-family: monospace;
      text-align: center;
      padding-top: 20vh;
    }
    #content {
      display: none;
      animation: fadeIn 1s ease-in forwards;
      animation-delay: 3s;
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>
  <audio autoplay>
    <source src="/assets/audio/order_or_die_init.mp3" type="audio/mpeg" />
  </audio>

  <div id="content">
    <h1>Order or die?</h1>
    <img src="/assets/images/jetbomb_cover_cruise.jpg" alt="Jet-Bomb Cover" width="300" />
    <p>just you. Order or die?</p>
  </div>

  <script>
    setTimeout(() => {
      document.getElementById('content').style.display = 'block';
    }, 3000);
  </script>
</body>
</html>
