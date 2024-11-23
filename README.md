<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulaire de Recherche</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f5f5f5;
        }
        #searchForm {
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px;
        }
        #searchForm div {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        #searchForm img {
            width: 40px;
            height: 40px;
        }
        #query {
            flex: 1;
            padding: 8px;
            font-size: 14px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        button {
            padding: 8px 16px;
            font-size: 14px;
            color: #fff;
            background-color: #007BFF;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <form id="searchForm" aria-labelledby="search-form">
        <div>
            <img src="logo.png" alt="Logo de Web Market">
            <input type="text" id="query" name="query" placeholder="Rechercher un produit, service ou information..." required aria-label="Entrez votre recherche">
            <button type="submit" aria-label="Soumettre la recherche">Rechercher</button>
        </div>
    </form>

    <script>
        document.getElementById('searchForm').addEventListener('submit', function(event) {
            event.preventDefault();
            let query = document.getElementById('query').value;
            if (query.trim() !== "") {
                alert(`Résultats pour : ${query}`);
            } else {
                alert("Veuillez entrer un terme de recherche.");
            }
        });
    </script>
</body>
</html>
