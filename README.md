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
      width: 250px;
      height: 250px;
      margin: 0 auto;
      --model-viewer-auto-rotate-delay: 3s;
      --model-viewer-camera-controls-touch-action: pan-y;
      border-radius: 20px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }

    .ar-button,
    .back-link {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 10px 15px;
      font-size: 1rem;
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
</div>

</body>
</html>
