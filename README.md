# EduTeam • Suivi collaboratif (Lite)

Application web **autonome** (un seul `index.html`) pour le suivi d'une classe entre PP et équipe éducative.

## Fonctionnalités
- Page d’accueil (cover) : **Entrer**, **Importer CSV**, **Démo**, **Mail**, **Aide**
- Fiches élèves avec **observations** (catégorie, état, auteur, date)
- **Fil d’équipe** (messages internes)
- **Filtres** + **recherche** + KPIs (barres)
- **Export CSV** des observations, **impression PDF**
- **Mail** : génère un brouillon (bilan classe / élèves ⚠️ / élève courant)
- Données **locales** (localStorage). Aucune donnée envoyée côté serveur pour cette version Lite.

## Démarrage
Ouvrez simplement `index.html` dans votre navigateur (Chrome/Edge/Firefox/Safari).  
Sur iPad/iPhone : via Safari → Partager → **Ajouter à l’écran d’accueil**.

### Modèle CSV
Voir `modele-eleves.csv`. Colonnes minimales : `Nom, Prénom`. Optionnel : `Classe, Sexe`.

## Déploiement GitHub Pages
1. Créez un repo vide sur GitHub (ex. `eduteam-lite`).
2. Dézippez ce dossier et placez vos fichiers dedans.
3. Dans le dossier, exécutez :
   ```bash
   git init
   git add .
   git commit -m "Init EduTeam Lite"
   git branch -M main
   git remote add origin https://github.com/<VOTRE_UTILISATEUR>/<VOTRE_REPO>.git
   git push -u origin main
   ```
4. Sur GitHub > Settings > **Pages** : Source = `main` (root).  
   L’app sera servie depuis `https://<VOTRE_UTILISATEUR>.github.io/<VOTRE_REPO>/`.

> Astuce : un fichier `.nojekyll` est inclus pour éviter les soucis de GitHub Pages.

## Licence
Ce projet est fourni **tel quel** pour vos tests internes. Ajoutez la licence de votre choix si vous le publiez.
