<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Modele AR Optimizate - Guler Cervical</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background-color: #fff;
    }

    /* Hero Section */
    .hero {
      height: 50vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background-image: url('fundal2.jpg');
      background-size: cover;
      background-position: center;
    }

    .hero h1 {
      color: #ffffff;
      font-size: 2em;
      margin: 0;
    }

    /* Model Section */
    .model-section {
      text-align: center;
      margin: 20px auto;
      max-width: 800px;
    }

    model-viewer {
      width: 300px;
      height: 300px;
      margin: 0 auto;
      border-radius: 20px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      --model-viewer-auto-rotate-delay: 3s;
      --model-viewer-camera-controls-touch-action: pan-y;
    }

    .ar-button {
      padding: 5px 10px;
      font-size: 0.8rem;
      margin-top: 10px;
      background-color: #007BFF;
      color: white;
      border: none;
      border-radius: 20px;
      cursor: pointer;
      transition: background-color 0.3s, box-shadow 0.3s;
    }

    .back-link {
      display: inline-block;
      padding: 5px 10px;
      font-size: 0.8rem;
      background-color: #007BFF;
      color: white;
      text-decoration: none;
      border-radius: 20px;
      margin-top: 20px;
      cursor: pointer;
      transition: background-color 0.3s, box-shadow 0.3s;
    }

    .ar-button:hover,
    .back-link:hover {
      background-color: #0056b3;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    }

    @media (max-width: 768px) {
      .model-section {
        max-width: 100%;
      }

      model-viewer {
        width: 250px;
        height: 250px;
      }
    }
  </style>
  <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
</head>
<body>
  <div class="hero">
    <h1>Guler Cervical - Model 3D Interactiv</h1>
  </div>

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
      alt="Guler Cervical"
      min-camera-orbit="auto 0deg 0deg"
      max-camera-orbit="auto 80deg auto">
      <button slot="ar-button" class="ar-button">Activează modul AR</button>
    </model-viewer>

    <a href="https://augmentedrealityweb.github.io/toate-produsele/" class="back-link">Înapoi la meniul principal</a>
  </div>
</body
