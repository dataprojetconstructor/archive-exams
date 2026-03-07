# Archives des Épreuves - Sciences Économiques & Gestion

Ce dépôt héberge le site web d'archivage des épreuves d'examens pour la faculté des Sciences Économiques et de Gestion. 
Il s'agit d'une initiative étudiante indépendante visant à centraliser et pérenniser l'accès aux anciens sujets.

🔗 **Accéder au site :** [https://votre-pseudo.github.io/votre-repo/](remplacez-ce-lien)

## 🎯 Objectif
Fournir une interface simple, rapide et accessible (mobile & PC) pour rechercher et télécharger les épreuves passées, classées par :
- **Filière** (Économie, Gestion...)
- **Niveau** (L1 à M2)
- **Semestre** (Harmattan / Mousson)
- **Année Académique**

## 🛠 Comment ça marche ? (Technique)
Ce site est **statique** et hébergé gratuitement via GitHub Pages. Il ne nécessite aucune base de données complexe (SQL).

- **Frontend :** HTML5, CSS3 (Style classique/universitaire), JavaScript (Vanilla).
- **Données :** Toutes les informations des épreuves sont stockées dans le fichier `data.json`.
- **Fichiers :** Les documents PDF sont stockés dans le dossier `/files`.

## 📝 Guide Administrateur : Ajouter une épreuve

Pour ajouter un nouveau sujet d'examen, suivez ces étapes :

1. **Préparer le fichier :**
   - Nommez le PDF de manière claire (ex: `microeco_L1_2024.pdf`).
   - Placez-le dans le dossier `files/`.

2. **Mettre à jour la base de données :**
   - Ouvrez le fichier `data.json`.
   - Ajoutez un nouveau bloc en haut de la liste (n'oubliez pas la virgule après l'accolade fermante du bloc précédent si vous ajoutez à la suite).
   - **Format obligatoire :**

```json
{
    "annee": "2023-2024",
    "semestre": "Harmattan",
    "matiere": "Nom de la Matière",
    "filiere": "Economie",
    "niveau": "L1",
    "fichier": "files/nom_du_fichier.pdf"
} 


⚠️ Avertissement
Ce site n'est pas le site officiel de l'université ou de l'établissement. Les documents sont partagés à but pédagogique.
🤝 Contribuer
Les étudiants souhaitant partager une épreuve manquante peuvent l'envoyer par email (voir pied de page du site).
