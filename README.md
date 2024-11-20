<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cambiar Idioma</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            padding: 20px;
            max-width: 800px;
            margin: auto;
        }
        button {
            background-color: #007BFF;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            border-radius: 5px;
            margin-bottom: 20px;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <button id="toggleButton">Cambiar a Inglés</button>

    <div id="content-es" style="display: block;">
        <h1>¡Hola! 👋</h1>
        <p>Soy <strong>Pablo</strong>, un apasionado <strong>desarrollador web</strong> y estudiante de tercer año de <strong>Ingeniería en Sistemas Informáticos</strong> en la Universidad de El Salvador.</p>
        <h2>👨‍💻 Sobre mí:</h2>
        <ul>
            <li>🔭 Actualmente, estoy trabajando en proyectos personales utilizando <strong>HTML, CSS, JavaScript</strong>, además de <strong>Java</strong> y <strong>SQL</strong>.</li>
            <li>🌱 Estoy aprendiendo <strong>Spring Boot</strong> y mejorando mis habilidades en <strong>diseño web responsivo</strong>.</li>
            <li>👯 Me interesa colaborar en proyectos de <strong>código abierto</strong>.</li>
            <li>💬 ¡Pregunta lo que quieras sobre <strong>desarrollo web</strong> o <strong>programación en Java</strong>!</li>
        </ul>
    </div>

    <div id="content-en" style="display: none;">
        <h1>Hi there! 👋</h1>
        <p>I'm <strong>Pablo</strong>, a passionate <strong>web developer</strong> and a third-year <strong>Computer Systems Engineering student</strong> at the University of El Salvador.</p>
        <h2>👨‍💻 About Me:</h2>
        <ul>
            <li>🔭 I’m currently working on personal projects using <strong>HTML, CSS, JavaScript</strong>, and backend development with <strong>Java</strong> and <strong>SQL</strong>.</li>
            <li>🌱 I’m learning <strong>Spring Boot</strong> and improving my skills in <strong>responsive web design</strong>.</li>
            <li>👯 I’m looking to collaborate on <strong>open-source projects</strong>.</li>
            <li>💬 Ask me anything about <strong>web development</strong> or <strong>Java programming</strong>!</li>
        </ul>
    </div>

    <script>
        const button = document.getElementById('toggleButton');
        const contentEs = document.getElementById('content-es');
        const contentEn = document.getElementById('content-en');

        button.addEventListener('click', () => {
            if (contentEs.style.display === 'block') {
                contentEs.style.display = 'none';
                contentEn.style.display = 'block';
                button.textContent = 'Cambiar a Español';
            } else {
                contentEs.style.display = 'block';
                contentEn.style.display = 'none';
                button.textContent = 'Cambiar a Inglés';
            }
        });
    </script>
</body>
</html>
