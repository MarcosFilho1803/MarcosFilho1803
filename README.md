
### index.html

O arquivo HTML principal que contém a estrutura do dashboard.

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard</title>
    <link rel="stylesheet" href="styles.css"> <!-- Link para seu arquivo CSS -->
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            display: flex;
            height: 100vh;
            overflow: hidden;
        }
        .sidebar {
            width: 250px;
            background-color: #333;
            color: white;
            display: flex;
            flex-direction: column;
            padding: 1rem;
        }
        .sidebar a {
            color: white;
            text-decoration: none;
            margin: 1rem 0;
            padding: 0.5rem;
            border-radius: 4px;
            transition: background 0.3s;
        }
        .sidebar a:hover {
            background-color: #575757;
        }
        .header {
            background-color: #4CAF50;
            color: white;
            padding: 1rem;
            text-align: center;
            width: 100%;
            position: fixed;
            top: 0;
            left: 250px;
            box-sizing: border-box;
        }
        .main {
            margin-left: 250px;
            margin-top: 60px;
            padding: 1rem;
            overflow-y: auto;
            flex-grow: 1;
        }
        .card {
            background: white;
            border-radius: 4px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            margin-bottom: 1rem;
            padding: 1rem;
        }
    </style>
</head>
<body>
    <div class="sidebar">
        <h2>Dashboard</h2>
        <a href="#overview">Visão Geral</a>
        <a href="#reports">Relatórios</a>
        <a href="#analytics">Análises</a>
        <a href="#settings">Configurações</a>
    </div>
    <div class="header">
        <h1>Dashboard</h1>
    </div>
    <div class="main">
        <div class="card">
            <h2>Visão Geral</h2>
            <p>Conteúdo de visão geral aqui.</p>
        </div>
        <div class="card">
            <h2>Relatórios</h2>
            <p>Conteúdo de relatórios aqui.</p>
        </div>
        <div class="card">
            <h2>Análises</h2>
            <p>Conteúdo de análises aqui.</p>
        </div>
        <div class="card">
            <h2>Configurações</h2>
            <p>Conteúdo de configurações aqui.</p>
        </div>
    </div>
</body>
</html>
