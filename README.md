<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplu UI/UX</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Bine ai venit pe pagina mea!</h1>
        <nav>
            <ul>
                <li><a href="#despre">Despre</a></li>
                <li><a href="#servicii">Servicii</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="despre">
            <h2>Despre</h2>
            <p>Acesta este un mic exemplu de pagină web pentru a ilustra principii de bază UI/UX.</p>
        </section>
        <section id="servicii">
            <h2>Servicii</h2>
            <p>Oferim consultanță și design web pentru proiectele tale.</p>
        </section>
        <section id="contact">
            <h2>Contact</h2>
            <p>Poți să ne contactezi la email@example.com.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Exemplu UI/UX. Toate drepturile rezervate.</p>
    </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header {
    background-color: #007BFF;
    color: white;
    padding: 20px;
    text-align: center;
}

header nav ul {
    list-style-type: none;
    padding: 0;
}

header nav ul li {
    display: inline;
    margin: 0 10px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    padding: 20px;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}
