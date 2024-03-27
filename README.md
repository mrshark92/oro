<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tu Página de TradingView</title>
    <style>
        html, body {
            margin: 0;
            padding: 0;
            height: 100%;
            width: 100%;
            overflow: hidden; /* Esto eliminará la barra de desplazamiento si está presente */
        }
        .tradingview-widget-container {
            height: 100%;
            width: 100%;
            position: relative; /* Esto asegura que la posición se calcula en relación con el cuerpo */
        }
        .tradingview-widget-container__widget {
            height: 100%;
            width: 100%;
        }
        /* Opcional: esconde el texto de los derechos de autor si interfiere */
        .tradingview-widget-copyright {
            display: none;
        }
    </style>
</head>
<body>
    <!-- TradingView Widget BEGIN -->
    <div class="tradingview-widget-container">
      <div class="tradingview-widget-container__widget"></div>
      <script type="text/javascript" src="https://s3.tradingview.com/external-embedding/embed-widget-advanced-chart.js" async>
      {
      "autosize": true,
      "symbol": "FXOPEN:XAUUSD",
      "interval": "240",
      "timezone": "Etc/UTC",
      "theme": "light",
      "style": "1",
      "locale": "es",
      "enable_publishing": false,
      "backgroundColor": "rgba(0, 0, 0, 1)",
      "hide_top_toolbar": true,
      "save_image": false,
      "calendar": false,
      "studies": [
        "STD;MACD",
        "STD;Divergence%1Indicator",
        "STD;Stochastic"
      ],
      "container_id": "tradingview-widget-container__widget"
      }
      </script>
    </div>
    <!-- TradingView Widget END -->
</body>
</html>
