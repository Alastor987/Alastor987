<!---
Alastor987/Alastor987 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->[Uploading acceuil.html…]()<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mon Portfolio</title>
    <link rel="stylesheet" href="css/01.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="acceuil.html" id="link-accueil">Accueil</a></li>
                <li><a href="acquis.html" id="link-acquis">Acquis</a></li>
                <li><a href="stage.html" id="link-stage">Stage</a></li>
                <li><a href="contact.html" id="link-contact">Contact</a></li>
                <li>
                    <div class="language-selector">
                        <label for="languageSelect">Langue :</label>
                        <select id="languageSelect" onchange="changeLanguage(this.value)">
                            <option value="fr">Français</option>
                            <option value="en">English</option>
                        </select>
                    </div>
                </li>
            </ul>
        </nav>
    </header>

    <section class="image-container">
        <img src="image/ft-coding-career-freepik-web.jpg" alt="Coding Image">
    </section>

    <section id="home" class="hero">
        <h1>Bienvenue sur mon Portfolio</h1>
        <p>Découvrez mes projets et compétences.</p>
    </section>
    <section id="about" class="about">
        <div id="me"><img src="/Photo interdit/IMG_3541.jpg" alt="me" alternatif width=10% height=10% margin-left=120px></div>
        <h2><strong><u>À propos de moi</u></strong></h2>
        <p>Je m'appelle CHEUNG-WONG Davy j'ai 19 ans.<br> Je suis actuellement étudiant en BTS SIO SISR au Lycée La Mennais.</p>
    </section>

    <footer>
        <p>&copy; 2024 Mon Portfolio. Tous droits réservés.</p>
        <section id="download">
            <h2>Télécharger mon CV</h2>
            <a href="documents/CV.pdf" download="Mon_CV.pdf" class="download-link">Télécharger mon CV</a>
        </section>
    </footer>

    <script>
        // Textes en français et en anglais
        const translations = {
            fr: {
                accueil: "Accueil",
                aquis: "Acquis",
                stage: "Stage",
                contact: "Contact",
                aquisTitle: "Bienvenue sur mon portfolio",
                aquisText: "Découvrez mes projets et compétences.",
                aboutTitle: "À propos de moi",
                aboutText: "Je m'appelle CHEUNG-WONG Davy j'ai 19 ans.Je suis actuellement étudiant en BTS SIO SISR au Lycée La Mennais.",
                footer: "&copy; 2024 Mon Portfolio. Tous droits réservés."
            },
            en: {
                accueil: "Home",
                aquis: "Skills",
                stage: "Internship",
                contact: "Contact",
                aquisTitle: "Welcome to my portfolio",
                aquisText: "Discover my projects and skills.",
                aboutTitle: "About me",
                aboutText: "My name is CHEUG-WONG Davy i have 19 years. I am currently a student in BTS SIO SISR at La Mennais High School.",
                footer: "&copy; 2024 My Portfolio. All rights reserved."
            }
        };

        // Fonction pour changer la langue
        function changeLanguage(lang) {
            // Changer les textes des liens de navigation
            document.getElementById('link-accueil').textContent = translations[lang].accueil;
            document.getElementById('link-acquis').textContent = translations[lang].aquis;
            document.getElementById('link-stage').textContent = translations[lang].stage;
            document.getElementById('link-contact').textContent = translations[lang].contact;

            // Changer les textes des sections
            document.querySelector('#home h1').textContent = translations[lang].aquisTitle;
            document.querySelector('#home p').textContent = translations[lang].aquisText;
            document.querySelector('#about h2').textContent = translations[lang].aboutTitle;
            document.querySelector('#about p').textContent = translations[lang].aboutText;

            // Changer le texte du footer
            document.querySelector('footer p').innerHTML = translations[lang].footer;
        }
    </script>
</body>
</html>


