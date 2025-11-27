[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/FPU0LhLp)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=21853657&assignment_repo_type=AssignmentRepo)
# TP N°2 — Initiation à HTML & CSS avec GitHub Classroom & VS Code

**Université Cadi Ayyad**  
**Faculté des Sciences Semlalia – Marrakech**  
**Filière : IAP | Niveau : 2ème année | A.U : 2025/2026**  
**Encadrants : Pr. Abdelmoula ABOUHILAL & Pr. Naima BABA**  

---

## PARTIE 1 — Environnement de développement (VS Code et GitHub)

### Étape 1 : Création de compte GitHub
1. Rendez-vous sur [https://github.com](https://github.com) → *Sign up*  
2. Complétez votre profil (nom, photo, bio courte).

### Étape 2 : Installation de VS Code
- Téléchargez et installez **Visual Studio Code**.
- Installez les extensions suivantes :
  - `Live Server`
  - `GitHub Pull Requests and Issues`
  - `Prettier – Code Formatter`

### Étape 3 : Connexion à GitHub
Dans VS Code → **Source Control → Sign in with GitHub**

### Étape 4 : Acceptation du lien GitHub Classroom
1. Cliquez sur le lien d’invitation fourni dans GitHub Classroom.  
2. Acceptez le devoir.  
3. GitHub créera automatiquement un dépôt personnel.

### Étape 5 : Ouvrir le projet dans VS Code
- Copiez le lien de votre dépôt (bouton **Code → HTTPS**)  
- Ouvrez VS Code et clonez votre dépôt :

```bash
git clone https://github.com/votre_nom/tp-html-css-votre_nom.git
```

- Ouvrez le dossier dans VS Code.  
- Lancez **Live Server** pour visualiser vos pages.

---

## PARTIE 2 — Exercices HTML & CSS

Chaque exercice doit être placé dans un fichier séparé (`ex1.html`, `ex2.html`, etc.).  
Le code CSS est intégré directement dans les balises `<style>` pour simplifier l’apprentissage.

---

### 🧠 Exercice 1 — Page de base et couleur de fond
```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Exercice 1 - Ma première page</title>
  <style>
    body {
      background-color: #eaf6ff;
      font-family: Arial, sans-serif;
      color: #333;
      text-align: center;
    }
    h1 {
      color: #0078d7;
    }
  </style>
</head>
<body>
  <h1>Bienvenue sur ma première page HTML !</h1>
  <p>Cette page a été créée dans VS Code et suivie via GitHub Classroom.</p>
</body>
</html>
```

---

### Exercice 2 — Liens et texte stylisé
```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Exercice 2 - Liens et texte</title>
  <style>
    body {
      background-color: #fffbea;
      font-family: Verdana, sans-serif;
      line-height: 1.5;
      padding: 20px;
    }
    h2 {
      color: #ff6f00;
      text-transform: uppercase;
    }
    a {
      color: #0066cc;
      font-weight: bold;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
      color: #004080;
    }
  </style>
</head>
<body>
  <h2>Mon profil</h2>
  <p>Visitez mon profil GitHub :</p>
  <a href="https://github.com/votre_nom" target="_blank">Mon GitHub</a>
</body>
</html>
```

---

### Exercice 3 — Images et listes
```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Exercice 3 - Images et listes</title>
  <style>
    body {
      background-color: #f0f8ff;
      font-family: "Trebuchet MS", sans-serif;
    }
    ul {
      list-style: none;
      padding: 0;
    }
    li {
      background-color: #e0f7fa;
      margin: 10px;
      padding: 10px;
      border-radius: 8px;
      display: flex;
      align-items: center;
    }
    img {
      width: 50px;
      height: 50px;
      margin-right: 10px;
      border-radius: 50%;
    }
  </style>
</head>
<body>
  <h2>Mes hobbies</h2>
  <ul>
    <li><img src="musique.jpg" alt="Musique"> Musique</li>
    <li><img src="sport.jpg" alt="Sport"> Sport</li>
    <li><img src="voyage.jpg" alt="Voyage"> Voyage</li>
  </ul>
</body>
</html>
```

---

### Exercice 4 — Police et arrière-plan
```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Exercice 4 - Style et fond</title>
  <style>
    body {
      background: linear-gradient(to right, #89f7fe, #66a6ff);
      font-family: Georgia, serif;
      color: #222;
      text-align: center;
      padding: 50px;
    }
    h1 {
      color: white;
      text-shadow: 2px 2px 5px #000;
    }
    p {
      background-color: rgba(255, 255, 255, 0.8);
      padding: 15px;
      border-radius: 10px;
      width: 60%;
      margin: auto;
    }
  </style>
</head>
<body>
  <h1>Texte stylisé et dégradé</h1>
  <p>Cette page démontre l’usage d’un dégradé, de la propriété text-shadow et des bordures arrondies.</p>
</body>
</html>
```

---

### Exercice 5 — Carte de profil
```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Exercice 5 - Carte de profil</title>
  <style>
    body {
      background-color: #eef6f9;
      font-family: 'Poppins', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .card {
      background-color: white;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(0,0,0,0.2);
      width: 300px;
      padding: 20px;
      text-align: center;
    }
    .card img {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      margin-bottom: 15px;
    }
    .card h2 {
      color: #0078d7;
    }
    .card p {
      color: #555;
    }
    .card button {
      background-color: #0078d7;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 5px;
      margin-top: 10px;
      cursor: pointer;
    }
    .card button:hover {
      background-color: #005a9e;
    }
  </style>
</head>
<body>
  <div class="card">
    <img src="profil.jpg" alt="Photo de profil">
    <h2>Votre Nom</h2>
    <p>Étudiant en Informatique<br>Passionné par le Web</p>
    <button>Me contacter</button>
  </div>
</body>
</html>
```

---

## PARTIE 3 — Envoi et publication

### Étape 1 : Commit & Push
Après chaque exercice, exécutez :

```bash
git add .
git commit -m "Ajout exercice X"
git push
```

