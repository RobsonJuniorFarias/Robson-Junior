<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio - Robson Junior</title>
    <link rel="stylesheet" href="style.css">
    <link rel="icon" href="favicon.ico" type="image/x-icon">
</head>

<body>
    <header>
        <div class="logo">
            <h1>Robson Junior</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#projetos">Projetos</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
        <div class="theme-toggle">
            <button onclick="toggleTheme()">🌙 / 🌞</button>
        </div>
    </header>

    <section id="home" class="home-section">
        <div class="content">
            <h2>Bem-vindo ao meu portfólio!</h2>
            <p>Sou Robson Junior, apaixonado por tecnologia e inovação. Explore meu trabalho e entre em contato!</p>
        </div>
    </section>

    <section id="sobre" class="info-section">
        <h2>Sobre Mim</h2>
        <p>Sou desenvolvedor full-stack com foco em criar soluções eficazes e inovadoras. Tenho experiência em tecnologias como HTML, CSS, JavaScript, React, Node.js e muito mais. Meu objetivo é continuar aprendendo e crescer profissionalmente em um ambiente colaborativo.</p>
    </section>

    <section id="projetos" class="projects-section">
        <h2>Meus Projetos</h2>
        <div class="projects-container">
            <div class="project-card">
                <h3>Projeto 1</h3>
                <p>Descrição do projeto, tecnologias usadas e link para visualizar.</p>
                <a href="#">Ver Mais</a>
            </div>
            <div class="project-card">
                <h3>Projeto 2</h3>
                <p>Descrição do projeto, tecnologias usadas e link para visualizar.</p>
                <a href="#">Ver Mais</a>
            </div>
            <div class="project-card">
                <h3>Projeto 3</h3>
                <p>Descrição do projeto, tecnologias usadas e link para visualizar.</p>
                <a href="#">Ver Mais</a>
            </div>
        </div>
    </section>

    <section id="contato" class="contact-section">
        <h2>Entre em Contato</h2>
        <p>Vamos conversar! Me envie uma mensagem ou me siga nas redes sociais.</p>
        <a href="https://www.instagram.com/robszz07/" target="_blank">Instagram</a>
        <a href="https://www.linkedin.com/in/robson-junior-9a7139287/" target="_blank">LinkedIn</a>
        <a href="Robson Junior.pdf" target="_blank">Baixar Currículo</a>
    </section>

    <footer>
        <p>&copy; 2024 Robson Junior. Todos os direitos reservados.</p>
    </footer>

    <script src="script.js"></script>
    /* Resetando estilos padrão */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Cores e fontes */
:root {
    --bg-color-light: #f4f4f9;
    --bg-color-dark: #1f1f1f;
    --text-color-light: #333;
    --text-color-dark: #f4f4f9;
    --accent-color: #007BFF;
    --button-hover-color: #0056b3;
}

/* Corpo do site */
body {
    font-family: 'Arial', sans-serif;
    background-color: var(--bg-color-light);
    color: var(--text-color-light);
    transition: background-color 0.3s ease, color 0.3s ease;
}

/* Header */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: var(--accent-color);
    color: white;
}

header .logo h1 {
    font-size: 2.5rem;
}

header nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.1rem;
}

header .theme-toggle button {
    background-color: transparent;
    border: 1px solid white;
    padding: 10px;
    color: white;
    cursor: pointer;
}

header .theme-toggle button:hover {
    background-color: white;
    color: var(--accent-color);
}

/* Home Section */
.home-section {
    text-align: center;
    padding: 100px 20px;
    background-color: var(--accent-color);
    color: white;
}

.home-section h2 {
    font-size: 3rem;
    margin-bottom: 20px;
}

.home-section p {
    font-size: 1.3rem;
}

/* Informações e Projetos */
.info-section, .projects-section, .contact-section {
    padding: 60px 20px;
    text-align: center;
}

.info-section h2, .projects-section h2, .contact-section h2 {
    font-size: 2.5rem;
    margin-bottom: 20px;
}

.projects-container {
    display: flex;
    justify-content: space-around;
    gap: 20px;
}

.project-card {
    background-color: #fff;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    padding: 20px;
    width: 30%;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
}

.project-card a {
    display: inline-block;
    padding: 10px 20px;
    background-color: var(--accent-color);
    color: white;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 15px;
}

.project-card a:hover {
    background-color: var(--button-hover-color);
}

/* Links de contato */
.contact-section a {
    display: inline-block;
    margin: 10px 0;
    color: var(--accent-color);
    text-decoration: none;
    font-weight: bold;
}

.contact-section a:hover {
    text-decoration: underline;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background-color: var(--accent-color);
    color: white;
}

/* Modo Dark */
body.dark {
    background-color: var(--bg-color-dark);
    color: var(--text-color-dark);
}

body.dark header {
    background-color: #333;
}

body.dark .theme-toggle button {
    border: 1px solid #333;
}

/* Responsividade */
@media (max-width: 768px) {
    .projects-container {
        flex-direction: column;
        align-items: center;
    }

    .project-card {
        width: 80%;
        margin-bottom: 20px;
    }
}
// Função para alternar o tema claro/escuro
function toggleTheme() {
    document.body.classList.toggle('dark');
}

</body>

</html>
