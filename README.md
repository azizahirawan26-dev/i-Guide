<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>i-GUIDE Imigrasi Banggai</title>
  <style>
    body {
      font-family: "Segoe UI", Arial, sans-serif;
      background: #f5f7fa;
      margin: 0;
      padding: 0;
      text-align: center;
      color: #333;
    }
    header {
      background: #003366;
      color: white;
      padding: 20px 10px;
    }
    h1 {
      margin: 0;
      font-size: 24px;
    }
    .language-buttons {
      margin: 20px;
    }
    button {
      margin: 5px;
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      background-color: #0078d7;
      color: white;
      cursor: pointer;
      transition: background 0.3s;
    }
    button:hover {
      background-color: #005fa3;
    }
    .content {
      max-width: 700px;
      margin: 40px auto;
      background: white;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      padding: 30px;
    }
    footer {
      background: #003366;
      color: white;
      padding: 10px;
      margin-top: 40px;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <header>
    <h1>🌐 i-GUIDE Imigrasi Banggai</h1>
    <p>Panduan digital layanan keimigrasian</p>
  </header>

  <div class="language-buttons">
    <button onclick="setLanguage('id')">Bahasa Indonesia 🇮🇩</button>
    <button onclick="setLanguage('en')">English 🇬🇧</button>
    <button onclick="setLanguage('zh')">中文 🇨🇳</button>
  </div>

  <div class="content" id="content">
    <!-- Konten default Bahasa Indonesia -->
    <h2>Selamat Datang di i-GUIDE</h2>
    <p>
      i-GUIDE Imigrasi Banggai merupakan panduan digital yang membantu masyarakat 
      memahami layanan keimigrasian dengan cepat, mudah, dan transparan.
    </p>
    <p>
      Melalui panduan ini, Anda dapat menemukan informasi mengenai prosedur pembuatan paspor, 
      izin tinggal, dan layanan keimigrasian lainnya.
    </p>
  </div>

  <footer>
    © 2025 Kantor Imigrasi Kelas II Non TPI Banggai | Direktorat Jenderal Imigrasi
  </footer>

  <script>
    function setLanguage(lang) {
      const content = document.getElementById("content");

      const data = {
        id: `
          <h2>Selamat Datang di i-GUIDE</h2>
          <p>
            i-GUIDE Imigrasi Banggai merupakan panduan digital yang membantu masyarakat 
            memahami layanan keimigrasian dengan cepat, mudah, dan transparan.
          </p>
          <p>
            Melalui panduan ini, Anda dapat menemukan informasi mengenai prosedur pembuatan paspor, 
            izin tinggal, dan layanan keimigrasian lainnya.
          </p>
        `,
        en: `
          <h2>Welcome to i-GUIDE</h2>
          <p>
            i-GUIDE Banggai Immigration is a digital guide designed to help the public 
            understand immigration services quickly, easily, and transparently.
          </p>
          <p>
            Through this guide, you can find information about passport issuance, 
            residence permits, and other immigration services.
          </p>
        `,
        zh: `
          <h2>欢迎来到 i-GUIDE</h2>
          <p>
            邦加依移民局的 i-GUIDE 是一个数字指南，旨在帮助公众快速、便捷、
            透明地了解移民服务。
          </p>
          <p>
            通过本指南，您可以了解护照办理、居留许可及其他移民服务的相关信息。
          </p>
        `
      };

      content.innerHTML = data[lang];
    }
  </script>
</body>
</html>
