<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Robson Junior - Desenvolvedor Junior</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Calibri, sans-serif;
      background-color: #E4F2E7;
      color: #2D3E40;
      line-height: 1.6;
    }

    header {
      background-color: #387373;
      color: white;
      text-align: center;
      padding: 40px 20px;
    }

    header h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }

    section {
      max-width: 900px;
      margin: 40px auto;
      padding: 20px;
    }

    .card {
      background-color: #93BFB7;
      border-radius: 12px;
      padding: 30px;
      margin-bottom: 30px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .card h2 {
      margin-bottom: 15px;
      font-size: 1.5em;
    }

    .button {
      display: inline-block;
      background-color: #387373;
      color: white;
      padding: 10px 20px;
      border-radius: 8px;
      text-decoration: none;
      margin: 10px 5px 0 0;
      transition: background 0.3s ease;
    }

    .button:hover {
      background-color: #2d5c5c;
    }

    footer {
      background-color: #387373;
      color: white;
      text-align: center;
      padding: 20px;
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 1.8em;
      }

      .card {
        padding: 20px;
      }
    }
        h1{
        text-align: center;
    }
    .card1 {
        background-color: #387373;
        border-radius: 12px;
        padding: 30px;
        margin-bottom: 30px;
        color: white;
    }
  </style>
<body>
    <section class="card1">
    <h1>Robson Junior</h1>
    <p style="text-align: center;">Desenvolvedor em formação • Foco em Back e Front-End</p>
    </section>
    <section class="card">
        <h2>Quem é o Robson?</h2>
        <p>Olá, sou o Robson Junior! Tenho 17 anos e sou apaixonado por tecnologia. Com quase 3 anos de experiência na área de TI, hoje foco meus estudos em programação — especialmente em desenvolvimento Front-End (HTML, CSS, JavaScript) e Back-End (Node.js). Valorizo o trabalho em equipe, comunicação e sempre busco contribuir para o crescimento dos projetos em que participo. Seja bem-vindo ao meu portfólio!</p>
    </section>

    <section class="card">
        <h2>Projetos</h2>
        <p>Tenho alguns projetos e aprendizados no meu GitHub. Você pode acessar clicando no botão abaixo</p>
        <a href="https://github.com/RobsonJuniorFarias" target="_blank" class="button">Ver no GitHub</a>
    </section>
 
   <section class="card">
        <h2>Contato & Redes</h2>
        <p>Deixo aqui, minhas redes socias e meu currículo, caso tenha interesse.</p>
        <a href="https://www.instagram.com/robszz07/" target="_blank" class="button">instagram</a>
        <a href="https://www.linkedin.com/in/robson-junior-9a7139287/" target="_blank" class="button">Linkedin</a>
        <a href="Currículo _ Vagas.com.pdf" target="_blank" class="button">Curriculo</a>
    </section>
    <footer style="background-color: #387373;">
    <p>&copy; 2024 Robson Junior • Todos os direitos reservados</p>
  </footer>

</body>
</html>