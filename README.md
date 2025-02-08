<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio - Robson Junior</title>
    <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">

    <style>
        /* Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            transition: background-color 0.3s, color 0.3s;
            --bg-color: #f7f7f7;
            --text-color: #333;
            --header-bg: linear-gradient(135deg, #007BFF, #4A90E2);
            --header-text: #fff;
            --card-bg: #fff;
            --card-shadow: rgba(0, 0, 0, 0.1);
            --button-bg: #007BFF;
            --button-hover: #0056b3;
        }

        body.dark {
            --bg-color: #121212;
            --text-color: #f7f7f7;
            --header-bg: linear-gradient(135deg, #1E1E1E, #333333);
            --header-text: #f7f7f7;
            --card-bg: #1E1E1E;
            --card-shadow: rgba(255, 255, 255, 0.1);
            --button-bg: #4A90E2;
            --button-hover: #007BFF;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
        }

        header {
            background: var(--header-bg);
            color: var(--header-text);
            text-align: center;
            padding: 50px 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        header p {
            font-size: 1.2em;
        }

        .theme-toggle {
            position: fixed;
            top: 20px;
            right: 20px;
            background: var(--button-bg);
            color: #fff;
            border: none;
            padding: 10px 15px;
            border-radius: 20px;
            cursor: pointer;
            transition: background 0.3s;
        }

        .theme-toggle:hover {
            background: var(--button-hover);
        }

        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .card {
            background: var(--card-bg);
            border-radius: 10px;
            box-shadow: 0 4px 8px var(--card-shadow);
            padding: 20px;
            text-align: center;
            flex: 1 1 calc(33.333% - 40px);
            max-width: calc(33.333% - 40px);
            min-width: 300px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            overflow: hidden; /* Esconde o excesso de texto */
            height: 400px; /* Altura fixa */
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .card h2 {
            margin-bottom: 15px;
        }

        .card p {
            margin-bottom: 20px;
            overflow: hidden; /* Para limitar o texto */
            text-overflow: ellipsis; /* Adiciona "..." caso o texto seja muito longo */
            white-space: nowrap; /* Impede o texto de quebrar a linha */
        }

        .card a {
            display: inline-block;
            background: var(--button-bg);
            color: white;
            text-decoration: none;
            padding: 10px 20px;
            border-radius: 5px;
            transition: transform 0.2s, background 0.3s;
        }

        .card a:hover {
            background: var(--button-hover);
            transform: scale(1.05);
        }

        footer {
            background: var(--header-bg);
            color: var(--header-text);
            text-align: center;
            padding: 20px 10px;
            margin-top: 20px;
        }

        @media (max-width: 768px) {
            .card {
                flex: 1 1 100%;
                max-width: 100%;
                height: auto; /* Remove altura fixa em telas pequenas */
            }
        }
    </style>
</head>

<body>
    <header>
        <h1>Robson Junior</h1>
        <p>Bem-vindo ao meu portfólio!</p>
    </header>

    <button class="theme-toggle">Alternar Tema</button>

    <main class="container">
        <section class="card">
            <h2>Sobre Mim</h2>
            <p>Olá! Sou Robson Junior, um profissional dedicado e apaixonado pelo que faço. Busco ter a oportunidade de desenvolver-me profissionalmente, colocando em prática aspectos estudados anteriormente, contribuindo para o sucesso de projetos por meio do trabalho em equipe.</p>
        </section>

        <section class="card">
            <h2>Projetos</h2>
            <p>Confira alguns dos meus projetos e veja mais detalhes sobre meu trabalho.</p>
            <a href="https://github.com/RobsonJuniorFarias" target="_blank">Ver Projetos</a>
        </section>

        <section class="card">
            <h2>Contato</h2>
            <p>Deixo aqui abaixo, minhas redes sociais e currículo, fique a vontade:</p>
            <a href="https://www.instagram.com/robszz07/" target="_blank">Instagram</a><br><br>
            <a href="https://www.linkedin.com/in/robson-junior-9a7139287/" target="_blank">LinkedIn</a><br><br>
            <a href="curriculo_compressed.pdf" target="_blank">Baixar Currículo</a>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Robson Junior. Todos os direitos reservados.</p>
    </footer>

    <script>
        const themeToggle = document.querySelector('.theme-toggle');
        themeToggle.addEventListener('click', () => {
            document.body.classList.toggle('dark');
        });
    </script>
</body>

</html>
