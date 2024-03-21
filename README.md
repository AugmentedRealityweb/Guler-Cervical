<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Modele AR Optimizate - Guler Cervical</title>
 <style>
 body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-image: url('fundal7.jpg');
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
 }
 .model-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
 }
 .model-section {
  text-align: center;
 margin-top: 38px; /* Mută modelul 3D cu aproximativ 1cm mai jos */
 }
 model-viewer {
  width: 188px;
  height: 188px;
  margin: 0 auto;
  border-radius: 20px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
  --model-viewer-auto-rotate-delay: 2s;
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
  margin-top: 50px - 57px; /* Distanța față de model */
  cursor: pointer;
  transition: background-color 0.3s, box-shadow 0.3s;
 }
.ar-button:hover,
 .back-link:hover {
  background-color: #0056b3;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
 }
p {
  color: #FFFFFF;
  font-size: 1.2em;
  margin-top: 10px;
 }
 </style>
 <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
</head>
<body>
<div class="model-container">
 <!-- Model Guler Cervical -->
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
 </div>
 <a href="https://augmentedrealityweb.github.io/toate-produsele/" class="back-link">Înapoi la meniul principal</a>
</div>
</body>
