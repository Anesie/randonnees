# ⛰️ Plateforme de Gestion de Randonnées

## 📖 Présentation
Ce projet est une application web full-stack permettant aux utilisateurs d'enregistrer, d'explorer et de noter des parcours de randonnées[cite: 3]. Il a été développé dans le cadre de la Licence MIASHS (Informatique et Cognition) à l'Université Grenoble Alpes (UGA).

L'application repose sur une architecture client-serveur développée en **Node.js** avec une base de données intégrée **SQLite**[cite: 2, 3]. Elle intègre un système d'authentification sécurisé et de multiples interactions asynchrones (AJAX) pour offrir une expérience utilisateur fluide sans rechargement de page[cite: 4].

## ✨ Fonctionnalités
Le projet intègre l'ensemble du "produit minimum viable" ainsi que toutes les fonctionnalités avancées requises[cite: 3] :

### 🗺️ Gestion des Randonnées
*   **Exploration :** Page d'accueil listant toutes les randonnées avec leur nom, point de départ et photo d'illustration[cite: 3, 4].
*   **Tri dynamique :** Possibilité de trier les randonnées par ordre alphabétique ou par score de popularité, le tout dynamiquement sans rechargement de page (AJAX)[cite: 3, 4].
*   **Détails :** Pages dédiées pour chaque randonnée affichant la description complète, l'adresse de départ et la note moyenne[cite: 3, 4].
*   **Contribution :** Formulaire de création de randonnée (nom, description, adresse, ajout de photo) redirigeant automatiquement vers la nouvelle fiche créée[cite: 3, 4].

### 🔐 Authentification & Sécurité
*   **Gestion des utilisateurs :** Formulaire unifié de connexion et d'inscription (avec case à cocher pour les nouveaux utilisateurs)[cite: 4].
*   **Sécurité des données :** Hachage cryptographique systématique des mots de passe avant l'enregistrement en base de données[cite: 4].
*   **Contrôle d'accès :** Redirection automatique vers la page de connexion si un utilisateur non-authentifié tente d'accéder à la page "Contribuer" (protection des routes)[cite: 4].
*   **Gestion des erreurs côté client :** Affichage de messages d'erreur asynchrones (mot de passe incorrect, identifiant inexistant/déjà pris) sans recharger la page[cite: 4].

### ⭐ Système de Notation
*   **Évaluation :** Les utilisateurs connectés peuvent attribuer une note de 1 à 5 à chaque randonnée[cite: 4].
*   **Unicité :** Une seule note autorisée par utilisateur et par randonnée[cite: 4].
*   **Expérience fluide :** Soumission des notes en AJAX avec gestion des erreurs réseau côté client (ex: perte de connexion serveur)[cite: 4].

## 🛠️ Technologies Utilisées
*   **Backend :** Node.js (version LTS)
*   **Base de données :** SQLite (Base de données relationnelle intégrée)
*   **Frontend :** HTML5, CSS3, JavaScript (Vanilla, Fetch API pour l'AJAX)[cite: 3]

## 🚀 Installation et Lancement
L'application est conçue pour fonctionner de manière autonome sans installation de logiciel tiers (hormis Node.js).

1. Clonez le dépôt sur votre machine locale :
   ```bash
   git clone https://github.com/Anesie/randonnees
  
