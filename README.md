<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Titlul Paginii Web</title>
  <link rel="stylesheet" href="style.css">
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
