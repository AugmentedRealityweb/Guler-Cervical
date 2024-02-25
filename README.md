<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Modele AR Optimizate</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background-image: url('fundal2.jpg');
      background-size: cover;
      background-position: center;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .model-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      max-width: 800px;
    }

    .model-section {
      margin: 10px;
      text-align: center;
    }

    model-viewer {
      width: 250px; /* Mărit pentru a oferi o vizualizare mai clară */
      height: 250px; /* Mărit pentru a oferi o vizualizare mai clară */
      margin: 0 auto;
      --model-viewer-auto-rotate-delay: 3s;
      --model-viewer-camera-controls-touch-action: pan-y;
      border-radius: 20px; /* Adăugat pentru a avea colțuri rotunjite */
      box-shadow: 0 4px 8px rgba(0,0,0,0.2); /* Adăugat pentru a adăuga o umbră, pentru un aspect mai estetic */
    }

    .ar-button,
    .back-link {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 10px 15px; /* Modificat pentru a oferi butoanelor o dimensiune mai mare și mai confortabilă */
      font-size: 1rem; /* Mărit pentru a îmbunătăți lizibilitatea */
      cursor: pointer;
      background-color: #007BFF;
      border: none;
      border-radius: 20px;
      color: white;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
      transition: background-color 0.3s, box-shadow 0.3s;
    }

    .ar-button:hover,
    .back-link:hover {
      background-color: #0056b3;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    }

    p {
      margin-top: 10px;
      color: #FFFFFF;
      font-size: 1.2em;
    }
  </style>
  <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
</head>
<body>

<div class="model-container">
  <!-- Model 1 -->
  <div class="model-section">
    <model-viewer
      src="cactus.glb"
      ios-src="cactus.usdz"
      ar
      ar-modes="webxr scene-viewer quick-look"
      camera-controls
      auto-rotate
      environment-image="neutral"
      shadow-intensity="1"
      loading="lazy"
      alt="Cactus Cary">
      <button slot="ar-button" class="ar-button">Activează modul AR</button>
    </model-viewer>
    <p>Cactus Cary</p>
  </div>

  <!-- Model 2 -->
  <div class="model-section">
    <model-viewer
      src="guler2.glb"
      ios-src="guler2.usdz"
      ar
      ar-modes="webxr scene-viewer quick-look"
      camera-controls
      auto-rotate
      environment-image="neutral"
      shadow-intensity="1"
      loading="lazy"
      alt="Guler Cervical">
      <button slot="ar-button" class="ar-button">Activează modul AR</button>
    </model-viewer>
    <p>Guler Cervical</p>
  </div>

  <!-- Model 3 -->
  <div class="model-section">
    <model-viewer
      src="scaun.glb"
      ios-src="scaun.usdz"
      ar
      ar-modes="webxr scene-viewer quick-look"
      camera-controls
      auto-rotate
      environment-image="neutral"
      shadow-intensity="1"
      loading="lazy"
      alt="Scaun">
      <button slot="ar-button" class="ar-button">Activează modul AR</button>
    </model-viewer>
    <p>Scaun</p>
  </div>
  <!-- Adaugă aici alte secțiuni de modele după necesități -->
</div>

</body>
</html>
