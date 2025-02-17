<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Bienvenue sur mon site web personnel où je propose des services de développement web, design graphique et marketing digital.">
    <title>@</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Bienvenue sur mon site web</h1>
        <nav>
            <ul>
                <li><a href="index.html">Accueil</a></li>
                <li><a href="apropos.html">À propos</a></li>
                <li><a href="services.html">Services</a></li>
                <li><a href="contact.html">Contact</a></li>
                <li><a href="login.html">Se connecter</a></li>
                <li><a href="register.html">S'inscrire</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section>
            <h2>Présentation</h2>
            <p>Ceci est un exemple de site web. Vous pouvez le personnaliser en ajoutant votre propre contenu, images et styles.</p>
        </section>

        <section>
            <h2>Mes services</h2>
            <ul>
                <li>Développement web</li>
                <li>Design graphique</li>
                <li>Marketing digital</li>
            </ul>
        </section>

        <section>
            <h2>Connexion et Inscription</h2>
            <p>Les utilisateurs peuvent créer un compte et se connecter pour accéder à des fonctionnalités exclusives.</p>
            <a href="register.html">Créer un compte</a> | <a href="login.html">Se connecter</a>
        </section>
        
        <section>
            <h2>Publications</h2>
            <p>
                Créez une publication, identifiez des profils en utilisant le symbole "@" (exemple: @nom_utilisateur) 
                et insérez un média.
            </p>
            <form action="publish.html" method="post" enctype="multipart/form-data">
                <textarea name="publication" rows="4" cols="50" placeholder="Votre publication..."></textarea>
                <br>
                <label for="media">Ajouter un média :</label>
                <input type="file" id="media" name="media" accept="image/*, video/*">
                <br>
                <button type="submit">Publier</button>
            </form>
        </section>
        
        <section>
            <h2>Commentaires</h2>
            <div class="comments-container">
                <!-- Affichage des commentaires existants -->
            </div>
            <div class="comment-form">
                <p>Seuls le profil ayant publié et le profil identifié peuvent commenter la publication.</p>
                <!-- Ce formulaire doit être activé uniquement pour les profils autorisés via une logique côté serveur ou JavaScript -->
                <form action="comment.html" method="post">
                    <textarea name="comment" rows="3" cols="50" placeholder="Votre commentaire..." disabled></textarea>
                    <br>
                    <button type="submit" disabled>Commenter</button>
                </form>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Mon site web. Tous droits réservés.</p>
    </footer>
</body>
</html>
