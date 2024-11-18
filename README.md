<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio - Robson Junior</title>
    <link rel="icon" href="https://img.icons8.com/ios-filled/50/32a852/code.png" type="image/png">
    <style>
        /* Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background-color: #e8f5e9;
            color: #333;
            line-height: 1.6;
            transition: background-color 0.3s, color 0.3s;
        }

        body.dark-mode {
            background-color: #2c2c2c;
            color: #f0f0f0;
        }

        header {
            background-color: #32a852;
            color: white;
            text-align: center;
            padding: 50px 10px;
        }

        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1.2em;
        }

        .container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            padding: 20px;
            text-align: center;
            transition: background-color 0.3s, color 0.3s;
        }

        .card.dark-mode {
            background-color: #444;
            color: #f0f0f0;
        }

        .card h2 {
            color: #32a852;
        }

        .card p {
            margin-bottom: 15px;
        }

        .card a {
            display: inline-block;
            background: #32a852;
            color: white;
            text-decoration: none;
            padding: 10px 15px;
            border-radius: 5px;
            transition: background 0.3s ease;
        }

        .card a:hover {
            background: #248f40;
        }

        footer {
            background-color: #32a852;
            color: white;
            text-align: center;
            padding: 20px 10px;
            margin-top: 20px;
        }

        .theme-toggle {
            position: fixed;
            top: 20px;
            right: 20px;
            background: #32a852;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 10px 15px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .theme-toggle:hover {
            background: #248f40;
        }
    </style>
</head>
<body>

<header>
    <h1>Robson Junior</h1>
    <p>Bem-vindo ao meu portfólio!</p>
</header>

<button class="theme-toggle" onclick="toggleTheme()">Alternar Tema</button>

<main class="container">
    <section class="card">
        <h2>Sobre Mim</h2>
        <p>Olá! Sou Robson Junior, um profissional dedicado e apaixonado pelo que faço. Ter a oportunidade de desenvolver-me profissionalmente, colocando em prática aspectos estudados anteriormente. Fazer um bom trabalho em equipe.</p>
    </section>

    <section class="card">
        <h2>Projetos</h2>
        <p>Confira alguns dos meus projetos e veja mais detalhes sobre meu trabalho.</p>
        <a href="https://github.com/RobsonJuniorFarias" target="_blank">Ver Projetos</a>
    </section>

    <section class="card">
        <h2>Contato</h2>
        <p>Vamos nos conectar! Siga-me nas redes sociais:</p>
        <a href="https://www.instagram.com/robszz07/" target="_blank">Instagram</a><br><br>
        <a href="https://www.linkedin.com/in/robson-junior-9a7139287/" target="_blank">LinkedIn</a><br><br>
        <a href="https://www.canva.com/design/DAFhBeKrj-A/sZSwqw4ggGVMS_dqlxHuuw/edit" target="_blank">Baixar Currículo</a>
    </section>
</main>

<footer>
    <p>&copy; 2024 Robson Junior. Todos os direitos reservados.</p>
</footer>

<script>
    // Alternar entre tema claro e escuro
    function toggleTheme() {
        document.body.classList.toggle('dark-mode');
        document.querySelectorAll('.card').forEach(card => card.classList.toggle('dark-mode'));
    }

    // Navegação suave
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function(e) {
            e.preventDefault();
            document.querySelector(this.getAttribute('href')).scrollIntoView({
                behavior: 'smooth'
            });
        });
    });

    // Mensagem de boas-vindas
    window.onload = function() {
        alert('Bem-vindo ao meu portfólio!');
    };
</script>

</body>
</html>
