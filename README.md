<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Somni Silvestre</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f6f6eb;
      color: #2b4829;
    }
    header, footer {
      background-color: #4caf50;
      color: white;
      text-align: center;
      padding: 10px;
    }
    #languageSelector {
      margin: 10px;
    }
  </style>
</head>
<body>
  <header>
    <h1 id="title">Bienvenidos a Somni Silvestre</h1>
    <p id="description">Cuidando el entorno, un paso a la vez.</p>
    <select id="languageSelector">
      <option value="es">Español</option>
      <option value="en">English</option>
      <option value="fr">Français</option>
    </select>
  </header>
  <main>
    <h2 id="aboutUs">Sobre nosotros</h2>
    <p>Somos una empresa dedicada a promover materiales reciclables y ecológicos.</p>
  </main>
  <footer>
    <p>© 2024 Somni Silvestre. Todos los derechos reservados.</p>
  </footer>
  <script>
    const translations = {
      es: {
        title: "Bienvenidos a Somni Silvestre",
        description: "Cuidando el entorno, un paso a la vez.",
        aboutUs: "Sobre nosotros",
      },
      en: {
        title: "Welcome to Somni Silvestre",
        description: "Caring for the environment, one step at a time.",
        aboutUs: "About Us",
      },
      fr: {
        title: "Bienvenue à Somni Silvestre",
        description: "Prendre soin de l'environnement, un pas à la fois.",
        aboutUs: "À propos de nous",
      }
    };

    document.getElementById('languageSelector').addEventListener('change', (event) => {
      const lang = event.target.value;
      document.getElementById('title').textContent = translations[lang].title;
      document.getElementById('description').textContent = translations[lang].description;
      document.getElementById('aboutUs').textContent = translations[lang].aboutUs;
    });
  </script>
</body>
</html>
