<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Télécharge Essentiel</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Inter', sans-serif;
      background: #f5faff;
      color: #003366;
      padding: 20px;
    }
    h1, h2 {
      text-align: center;
      color: #0055aa;
    }
    nav {
      background: #e0f0ff;
      border: 1px solid #cce5ff;
      border-radius: 10px;
      padding: 10px 20px;
      margin-bottom: 30px;
    }
    nav ul {
      list-style: none;
      padding: 0;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
    }
    nav li a {
      text-decoration: none;
      color: #0055aa;
      font-weight: 600;
      padding: 5px 10px;
      border-radius: 5px;
      transition: background 0.3s;
    }
    nav li a:hover {
      background: #cce5ff;
    }
    .category {
      margin-bottom: 50px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background: #ffffff;
      padding: 15px;
      border-radius: 10px;
      border: 2px solid #cce5ff;
      box-shadow: 0 2px 5px rgba(0,0,0,0.05);
    }
    .card label {
      display: flex;
      align-items: center;
      font-weight: 600;
      color: #003366;
    }
    .card input[type="checkbox"] {
      margin-right: 10px;
      transform: scale(1.2);
    }
    .card p {
      font-size: 0.95em;
      color: #555;
      margin-top: 5px;
    }
    footer {
      text-align: center;
      margin-top: 60px;
      font-size: 0.9em;
      color: #777;
    }
  </style>
</head>
<body>
  <h1>🛠️ Télécharge Essentiel</h1>
  <p style="text-align:center;">Cochez un logiciel pour lancer le téléchargement automatiquement.</p>

  <!-- 🔗 Menu de navigation -->
  <nav>
    <ul>
      <li><a href="Index2.html">🏠 Accueil</a></li>
      <li><a href="Classificationinfotmatique.html">📚 Classification informatique</a></li>
      <li><a href="Essai8.html">🧪 Essai 8</a></li>
      <li><a href="Index4.html">📄 Index 4</a></li>
      <li><a href="Index6.html">📄 Index 6</a></li>
      <li><a href="Modification2025.html">🛠️ Modification 2025</a></li>
      <li><a href="Tableaupc.html">💻 Tableau PC</a></li>
    </ul>
  </nav>

  <!-- 📦 Compression -->
  <section class="category">
    <h2>📦 Compression</h2>
    <div class="grid">
      <!-- cartes compression -->
    </div>
  </section>

  <!-- 👨‍💻 Développement -->
  <section class="category">
    <h2>👨‍💻 Développement</h2>
    <div class="grid">
      <!-- cartes développement -->
    </div>
  </section>

  <footer>
    &copy; 2025 Télécharge Essentiel — Site rapide, gratuit et sans pub
  </footer>

  <script>
    function autoDownload(checkbox, url) {
      if (checkbox.checked) {
        const link = document.createElement('a');
        link.href = url;
        link.download = '';
        document.body.appendChild(link);
        link.click();
        document.body.removeChild(link);
      }
    }
  </script>
</body>
</html>
<h1>📁 Télécharge Essentiel</h1>

<div class="grid">
  <div class="card">
    <h2>📚 Classification informatique</h2>
    <p>Explore les catégories d’usages informatiques.</p>
    <a href="Classificationinfotmatique.html">Accéder</a>
  </div>

  <div class="card">
    <h2>🧪 Essai 8</h2>
    <p>Page de test et d’expérimentation.</p>
    <a href="Essai8.html">Accéder</a>
  </div>

  <div class="card">
    <h2>🏠 Index 2</h2>
    <p>Page d’accueil alternative.</p>
    <a href="Index2.html">Accéder</a>
  </div>

  <div class="card">
    <h2>📄 Index 4</h2>
    <p>Contenu complémentaire ou structuré.</p>
    <a href="Index4.html">Accéder</a>
  </div>

  <div class="card">
    <h2>📄 Index 6</h2>
    <p>Suite ou extension du contenu.</p>
    <a href="Index6.html">Accéder</a>
  </div>

  <div class="card">
    <h2>🛠️ Modification 2025</h2>
    <p>Page dédiée aux mises à jour.</p>
    <a href="Modification2025.html">Accéder</a>
  </div>

  <div class="card">
    <h2>💻 Tableau PC</h2>
    <p>Tableau comparatif des configurations.</p>
    <a href="Tableaupc.html">Accéder</a>
  </div>
</div>

