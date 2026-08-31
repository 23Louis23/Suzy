# Suzy Training App

App de suivi pour le cycle **Renfo** de Suzy (6 semaines, 3 séances par semaine). Elle utilise la **même base de données Supabase** que les apps de Jox, Loan, Fifi, Manon et Lucie & Yo — pas besoin de recréer un compte ou un projet.

## Particularité par rapport aux autres apps

Pas de suivi Hooper (charge interne) sur cette app, à la demande. Il n'y a donc que 2 onglets : **Séance** et **Tableau de bord** (pas d'onglet "Historique", qui n'existait que pour l'historique Hooper sur les autres apps). Le bouton "Effacer toutes les données" a été déplacé dans l'onglet Tableau de bord.

## 1. Base de données

✅ Déjà faite — cette app utilise le même projet Supabase que les autres, avec la colonne `athlete` ("Suzy") qui sépare ses données de celles des autres athlètes.

## 2. Configurer l'appli

✅ Déjà fait — `index.html` contient l'URL et la clé Supabase (les mêmes que pour les autres), et un code d'accès (`8214` par défaut, modifiable en cherchant `APP_PIN` dans le fichier).

## 3. Déployer sur Vercel (gratuit) — sans rien installer

Même procédure que pour les autres athlètes :

1. Crée un nouveau repo GitHub (ex: `suzy-training-app`).
2. Upload les 2 fichiers (`index.html`, `README.md`) via "uploading an existing file" sur la page du repo.
3. Va sur [vercel.com/new](https://vercel.com/new), importe ce nouveau repo, déploie avec les réglages par défaut.
4. Récupère l'URL propre du projet (ex: `https://suzy-training-app.vercel.app`, pas l'URL avec un hash aléatoire) dans la section "Domains" du projet.

## 4. Utilisation

Envoie l'URL + le code `8214` à Suzy. Chaque séance permet de renseigner les charges (avec 2 cases pour les exercices en superset), une note sur les abdos et une note générale de séance. Le tableau de bord affiche l'évolution des charges par exercice, semaine après semaine.
