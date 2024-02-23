<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modele AR Optimizate</title>
    <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-image: url('fundal.jpg'); /* Actualizare la noua imagine de fundal */
            background-size: cover;
            background-position: center;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .model-container {
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            width: 100%;
            max-width: 400px;
        }
        .model-section {
            margin: 10px;
            text-align: center;
        }
        model-viewer {
            width: 200px;
            height: 200px;
            margin: 0 auto;
        }
        .ar-button {
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 10px auto;
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
        .ar-button:hover {
            background-color: #0056b3;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }
        .navigation-buttons {
            display: flex;
            justify-content: space-around;
            width: 100%;
            margin-top: 20px;
        }
        a {
            text-decoration: none;
            color: white;
            background-color: #007BFF;
            padding: 10px 20px;
            border-radius: 20px;
            transition: background-color 0.3s;
        }
        a:hover {
            background-color: #0056b3;
        }
        p {
            margin-top: 10px;
            color: #FFFFFF;
            font-size: 1.2em;
        }
    </style>
</head>
<body>

<div class="model-container">
    <!-- Model 1: Cactus -->
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
    <!-- Model 2: Noodle -->
    <div class="model-section">
        <model-viewer 
            src="noodle.glb" 
            ios-src="noodle.usdz" 
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
        <p>Noodle Pack</p>
    </div>
    <!-- Model 3: Scaun -->
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
            min-camera-orbit="auto 0deg 0deg" 
            max-camera-orbit="auto 80deg auto">
            <button slot="ar-button" class="ar-button">Activează modul AR</button>
        </model-viewer>
        <p>Scaun Ikea</p>
    </div>
</div>

<div class="navigation-buttons">
    <a href="https://augmentedrealityweb.github.io/Produse/">Pagina Precedentă</a>
    <a href="https://augmentedrealityweb.github.io/Produse/">Pagina Următoare</a>
</div>

</body>
</html>
