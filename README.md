<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ultra Fast Blinking Clock</title>
  <link href="https://fonts.cdnfonts.com/css/ds-digital" rel="stylesheet">
  <style>
    body {
      margin: 0;
      background-color: black;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .clock {
      font-family: 'DS-Digital', sans-serif;
      font-size: 48rem;
      color: white;
      display: flex;
      gap: 1rem;
    }

    .digit {
      animation: blink 0.05s infinite alternate;
    }

    .digit:nth-child(1) {
      animation-delay: 0s;
    }

    .digit:nth-child(2) {
      animation-delay: 0.025s;
    }

    .digit:nth-child(3) {
      animation-delay: 0.05s;
    }

    @keyframes blink {
      from {
        opacity: 1;
      }
      to {
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="clock">
    <span class="digit">1</span>
    <span class="digit">0</span>
    <span class="digit">1</span>
  </div>
</body>
</html>
