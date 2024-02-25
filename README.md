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
      flex-wrap: wrap; /* Optimize layout for multiple models */
      justify-content: center;
      max-width: 800px; /* Adjust for larger screens */
    }

    .model-section {
      margin: 10px;
      text-align: center;
    }

    model-viewer {
      width: 170px;
      height: 170px;
      margin: 0 auto;
    }

    .ar-button,
    .back-link {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 5px 10px;
      font-size: 0.8rem;
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

    .back-button {
      display: flex;
      justify-content: center;
      width: 100%;
      padding: 20px;
    }
  </style>
</head>
<body>

<div class="model-container">
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
      min-camera-orbit="auto 0deg 0deg"
      max-camera-orbit="auto 80deg auto">
      <button slot="ar-button" class="ar-button">Activează modul AR</button>
    </model-viewer>
    <p>Cactus Cary</p>
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
      min-camera-orbit="auto 0deg 0deg"
      max-camera-orbit="auto 80deg auto">
      <button slot="ar-button" class="ar-button">Activează modul AR</button>
    </model-viewer>
    <p>Guler Cervical</p>
  </div>

  <div class="model-section">
    <model-viewer
      src="scaun.glb"
      ios-src="scaun.usdz"
      ar
      ar
