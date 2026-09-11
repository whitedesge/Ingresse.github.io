<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ingresse</title>
    <style>
       body {
            background-color: var(--primary-color)      ;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: var(--secondary-color);
            transition: background-color 0.3s, color 0.3s;
        }
        :root{
            --primary-color: #c0c0c0;
            --secondary-color: #222;
        }
        body.dark-mode {
            background-color: #222;
            color: #f3f3f3;
            transition: background-color 0.3s, color 0.3s;
        }
        body.dark-mode #escuro {
            background-color: #f3f3f3;
            color: #222;
            transition: background-color 0.3s, color 0.3s;
        }
        #escuro {
            background-color: #222;
            color: #f3f3f3;
            border: 1px solid #ccc;
            padding: 5px 10px;
            cursor: pointer;
            margin-left: 5px;
            margin-top: 5px;
            transition: background-color 0.3s, color 0.3s;
            border-radius: 12px;
        }
        h1 {
            text-align: center;
            margin-top: 20px;
            font-family: 'Arial Black', sans-serif, monospace;
        }
        h3 {
            text-align: center;
            margin-top: 5px;
            font-family: 'Fira Sans', sans-serif, monospace;
        }
        footer {
            text-align: center;
            margin-top: 20px;
            padding: 10px;
            font-size: 14px;
        }
        p {
            font-family: 'Martel', serif;
            margin: 5px 5px 5px 5px;
        }
        main {
            padding: 20px;
        }
        .filmes-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 20px;
            max-width: 1100px;
            margin: 30px auto;
        }
        .filme-card {
            background: rgba(255, 255, 255, 0.08);
            border-radius: 18px;
            padding: 12px;
            text-align: center;
            box-shadow: 0 6px 18px rgba(0, 0, 0, 0.12);
        }
        .filme-card img {
            display: block;
            width: 100%;
            height: 260px;
            object-fit: cover;
            border-radius: 14px;
        }
        .filme-card p {
            margin: 10px 0 0;
            font-weight: bold;
            text-align: center;
        }
        body.dark-mode .filme-card {
            background: rgba(255, 255, 255, 0.04);
            box-shadow: 0 6px 18px rgba(0, 0, 0, 0.3);
        }
    </style>
    <script>
        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
        }
        
    </script>
</head>
<body>
    <header>
        <button id="escuro" onclick="toggleDarkMode()">Mudar Tema</button>
        <h1>Ingresse</h1>
        <h3>Bem-vindo ao Ingresse!</h3>
    </header>
    <main>
        <div class="filmes-grid">
            <div class="filme-card">
                <img src="AO.jfif" alt="Cartaz do filme A Odisseia">
                <p>A Odisseia</p>
            </div>
            <div class="filme-card">
                <img src="HAUND.jfif" alt="Cartaz do filme Homem-Aranha: Um Novo Dia">
                <p>Homem-Aranha: Um Novo Dia</p>
            </div>
            <div class="filme-card">
                <img src="images.jfif" alt="Cartaz do filme Jogos Vorazes: Amanhecer na Colheita">
                <p>Jogos Vorazes: Amanhecer da Colheita</p>
            </div>
            <div class="filme-card">
                <img src="PCUAD.jfif" alt="Cartaz do filme Patrulha Canina: Uma Aventura Dino">
                <p>Patrulha Canina: Uma Aventura Dino</p>
            </div>
            <div class="filme-card">
                <img src="RE.jfif" alt="Cartaz do filme Resident Evil">
                <p>Resident Evil</p>
            </div>
            <div class="filme-card">
                <img src="TS5.jfif" alt="Cartaz do filme Toy Story 5">
                <p>Toy Story 5</p>
            </div>
            <div class="filme-card">
                <img src="" alt="Sem mais filmes em cartaz :P">
                <p>Sem mais filmes em cartaz :P</p>
            </div>
        </div>
    </main>
    <footer>
        <p>&copy; 2026 Ingresse. Todos os direitos reservados.</p>
        <p style="font-size: 12px;">Desenvolvido por Guilherme Adorno Rodrigues</p>
        <p style="color: var(--primary-color); font-size: 12px;">Parabéns por encontrar meu segredo: [SEGREDO]</p>
    </footer>
</body>
</html>
