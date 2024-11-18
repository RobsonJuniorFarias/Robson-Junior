<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio - Robson Junior</title>
    <link rel="icon" href="https://img.icons8.com/ios-filled/50/000000/code.png" type="image/png">
    <style>
        /* Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background-color: var(--background-color, #ffffff);
            color: var(--text-color, #333333);
            line-height: 1.6;
            transition: background-color 0.3s, color 0.3s;
        }

        header {
            background-color: var(--header-color, #007BFF);
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
        }

        .card h2 {
            color: var(--header-color, #007BFF);
        }

        .card p {
            margin-bottom: 15px;
        }

        .card a {
            display: inline-block;
            background: var(--header-color, #007BFF);
            color: white;
            text-decoration: none;
            padding: 10px 15px;
            border-radius: 5px;
            transition: background 0.3s ease;
        }

        .card a:hover {
            background: var(--header-hover-color, #0056b3);
        }

        footer {
            background-color: var(--header-color, #007BFF);
            color: white;
            text-align: center;
            padding: 20px 10px;
            margin-top: 20px;
        }

        .theme-selector {
            text-align: center;
            margin: 20px 0;
        }

        .theme-selector label {
            font-weight: bold;
            margin-right: 10px;
        }

        .theme-selector input[type="color"] {
            cursor: pointer;
        }
    </style>
</head>
<body>

<header>
    <h1>Robson Junior</h1>
    <p>Bem-vindo ao meu portfólio!</p>
</header>

<div class="theme-selector">
    <label for="color-picker">Escolha a cor do tema:</label>
    <input type="color" id="color-picker" value="#007BFF">
</div>

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
    const colorPicker = document.getElementById('color-picker');
    colorPicker.addEventListener('input', (e) => {
        const color = e.target.value;
        document.documentElement.style.setProperty('--header-color', color);
        document.documentElement.style.setProperty('--header-hover-color', shadeColor(color, -20));
    });

    // Função para ajustar a tonalidade da cor
    function shadeColor(color, percent) {
        const f = parseInt(color.slice(1), 16);
        const t = percent < 0 ? 0 : 255;
        const p = percent < 0 ? percent * -1 : percent;
        const R = f >> 16;
        const G = (f >> 8) & 0x00FF;
        const B = f & 0x0000FF;
        return `#${(
            0x1000000 +
            (Math.round((t - R) * p) + R) * 0x10000 +
            (Math.round((t - G) * p) + G) * 0x100 +
            (Math.round((t - B) * p) + B)
        )
            .toString(16)
            .slice(1)}`;
    }
</script>

</body>
</html>
