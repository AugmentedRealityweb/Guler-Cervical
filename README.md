<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Titlul Paginii Web</title>
  <link rel="stylesheet" href="style.css">
  <style>
    .model-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      margin-top: 20px;
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
    .ar-button, .back-link {
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
    .ar-button:hover, .back-link:hover {
      background-color: #0056b3;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    }
  </style>
  <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
</head>
<body>
  <header>
    <img src="logo.png" alt="Logo">
    <h1>Sloganul companiei</h1>
  </header>

  <main>
    <section class="imagine-text">
      <img src="imagine1.jpg" alt="Imagine 1">
      <h2>Titlul Sectiunii 1</h2>
      <p>Textul sectiunii 1, descrierea continutului.</p>
    </section>

    <section class="caracteristici">
      <h2>Titlul Sectiunii 2</h2>
      <ul>
        <li>Caracteristica 1</li>
        <li>Caracteristica 2</li>
        <li>Caracteristica 3</li>
      </ul>
    </section>

    <section class="testimoniale">
      <h2>Titlul Sectiunii 3</h2>
      <p>"Testimonial 1 - descriere experienta pozitiva."</p>
      <p>"Testimonial 2 - descriere experienta pozitiva."</p>
    </section>

    <!-- Sectiunea AR -->
    <section class="ar-model">
      <div class="model-container">
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
    </section>

    <section class="contact">
      <h2>Contactati-ne</h2>
      <form action="/contact" method="post">
        <input type="text" name="nume" placeholder="Nume">
        <input type="email" name="email" placeholder="Email">
        <textarea name="mesaj" placeholder="Mesajul tau"></textarea>
        <button type="submit">Trimite</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2023 - Compania Ta</p>
    <a href="#">Link 1</a> | <a href="#">Link 2</a>
  </footer>
</body>
</html>
