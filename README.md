
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfólio - Roberto Alves Coelho</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background-color: #0d1117;
      color: #f0f6fc;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 40px 20px;
    }

    h1 {
      font-size: 2.8rem;
      color: #58a6ff;
      text-align: center;
    }

    .subtitle {
      color: #8b949e;
      font-size: 1.2rem;
      margin-bottom: 15px;
    }

    .description {
      max-width: 600px;
      text-align: center;
      line-height: 1.6;
      color: #c9d1d9;
      margin-bottom: 40px;
      font-size: 1rem;
    }

    .skills {
      width: 100%;
      max-width: 600px;
      margin-bottom: 30px;
    }

    .skill {
      margin-bottom: 15px;
    }

    .skill-name {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 5px;
      font-weight: 500;
    }

    .progress-bar {
      background-color: #21262d;
      border-radius: 8px;
      height: 10px;
      overflow: hidden;
    }

    .progress {
      height: 100%;
      background: linear-gradient(90deg, #58a6ff, #1f6feb);
      width: 0;
      transition: width 1.5s ease-in-out;
    }

    .icons {
      display: flex;
      gap: 20px;
      justify-content: center;
      margin-top: 30px;
      flex-wrap: wrap;
    }

    .icons i {
      font-size: 2rem;
      transition: transform 0.3s ease;
      color: #f0f6fc;
    }

    .icons i:hover {
      transform: scale(1.2);
      color: #58a6ff;
    }

    footer {
      margin-top: 40px;
      color: #8b949e;
      font-size: 0.9rem;
      text-align: center;
    }

    @media (max-width: 600px) {
      h1 {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>

  <h1>Roberto Alves Coelho</h1>
  <p class="subtitle">Desenvolvedor Web Jr | 37 anos</p>

  <p class="description">
    Sou apaixonado por tecnologia e atualmente curso <strong>Análise e Desenvolvimento de Sistemas</strong>.
    Meu foco principal é o <strong>front-end</strong>, onde me dedico a criar interfaces modernas, intuitivas e interativas.
  </p>

  <div class="skills">
    <div class="skill">
      <div class="skill-name">HTML <span>90%</span></div>
      <div class="progress-bar"><div class="progress" data-value="90"></div></div>
    </div>
    <div class="skill">
      <div class="skill-name">CSS <span>85%</span></div>
      <div class="progress-bar"><div class="progress" data-value="85"></div></div>
    </div>
    <div class="skill">
      <div class="skill-name">JavaScript <span>80%</span></div>
      <div class="progress-bar"><div class="progress" data-value="80"></div></div>
    </div>
    <div class="skill">
      <div class="skill-name">PHP <span>70%</span></div>
      <div class="progress-bar"><div class="progress" data-value="70"></div></div>
    </div>
    <div class="skill">
      <div class="skill-name">MySQL <span>70%</span></div>
      <div class="progress-bar"><div class="progress" data-value="70"></div></div>
    </div>
  </div>

  <div class="icons">
    <i class="fab fa-html5" title="HTML5" style="color:#e34c26"></i>
    <i class="fab fa-css3-alt" title="CSS3" style="color:#264de4"></i>
    <i class="fab fa-js-square" title="JavaScript" style="color:#f7df1e"></i>
    <i class="fab fa-php" title="PHP" style="color:#787cb5"></i>
    <i class="fas fa-database" title="MySQL" style="color:#00618a"></i>
  </div>

  <footer>© 2025 Roberto Alves Coelho — Desenvolvedor Web Jr</footer>

  <script>
    // Animação das barras de progresso
    document.addEventListener("DOMContentLoaded", () => {
      const progresses = document.querySelectorAll(".progress");
      progresses.forEach(bar => {
        const value = bar.getAttribute("data-value");
        setTimeout(() => {
          bar.style.width = value + "%";
        }, 300);
      });
    });
  </script>
</body>
</html>
