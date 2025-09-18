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

  <!-- 📦 Compression -->
  <section class="category">
    <h2>📦 Compression</h2>
    <div class="grid">
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://www.7-zip.org/a/7z2501-x64.exe')"> 7-Zip</label><p>Compression rapide — v25.01</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://github.com/peazip/PeaZip/releases/download/10.6.1/peazip-10.6.1.WIN64.exe')"> PeaZip</label><p>Compression avancée — v10.6.1</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://www.win-rar.com/fileadmin/winrar-versions/winrar-x64-621.exe')"> WinRAR</label><p>Archiveur puissant — v6.21</p></div>
    </div>
  </section>

  <!-- 👨‍💻 Développement -->
  <section class="category">
    <h2>👨‍💻 Développement</h2>
    <div class="grid">
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://www.python.org/ftp/python/3.13.7/python-3.13.7-amd64.exe')"> Python x64</label><p>Langage de programmation — v3.13.7</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://www.python.org/ftp/python/3.13.7/python-3.13.7-arm64.exe')"> Python arm64</label><p>Langage de programmation — v3.13.7</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://www.python.org/ftp/python/2.7.18/python-2.7.18.amd64.msi')"> Python 2.7</label><p>Langage classique — v2.7.18</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://github.com/git-for-windows/git/releases/download/v2.51.0.windows.1/Git-2.51.0-64-bit.exe')"> Git</label><p>Contrôle de version — v2.51.0</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://filezilla-project.org/download.php?type=client')"> FileZilla</label><p>Client FTP — v3.69.3</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://notepad-plus-plus.org/repository/8.x/8.8.5/npp.8.8.5.Installer.x64.exe')"> Notepad++</label><p>Éditeur de code — v8.8.5</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://winscp.net/download/WinSCP-6.5.3-Setup.exe')"> WinSCP</label><p>Client SCP — v6.5.3</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://the.earth.li/~sgtatham/putty/latest/w64/putty.exe')"> PuTTY</label><p>Client SSH — v0.83</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://github.com/WinMerge/winmerge/releases/download/v2.16.50.2/WinMerge-2.16.50.2-x64-Setup.exe')"> WinMerge</label><p>Comparateur de fichiers — v2.16.50.2</p></div>
      <div class="card"><label><input type="checkbox" onclick="autoDownload(this, 'https://update.code.visualstudio.com/latest/win32-x64-user/stable')"> Visual Studio Code</label><p>Éditeur moderne — v1.104.1</p></div>
    </div>
  </section>

  <!-- Tu peux ajouter ici les autres catégories : Sécurité, Média, Utilitaires, etc. -->

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
