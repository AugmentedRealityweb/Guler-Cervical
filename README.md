<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modele AR Optimizate - Guler Cervical</title>
    <link rel="stylesheet" href="style.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
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
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        .model-section {
            text-align: center;
        }
        model-viewer {
            width: 250px;
            height: 250px;
            margin: 0 auto;
            border-radius: 20px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            --model-viewer-auto-rotate-delay: 3s;
            --model-viewer-camera-controls-touch-action: pan-y;
        }
        /* Restul stilurilor pentru .ar-button, .back-link, etc. */
    </style>
    <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
</head>
<body>
    <header>
        <!-- Header content aici, dacă dorești să păstrezi antetul -->
    </header>
    <main>
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
    </main>
    <footer>
        <!-- Footer content aici, dacă dorești să adaugi un subsol paginii -->
    </footer>
</body>
</html>
