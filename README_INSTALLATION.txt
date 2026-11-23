ROAD TO X V13 — VERSION IPHONE (PWA)
====================================

Cette version est une application web installable (PWA), pas un fichier IPA natif
à installer depuis l'App Store. Elle s'ajoute à l'écran d'accueil de l'iPhone et
s'ouvre dans une fenêtre dédiée.

PUBLICATION SUR GITHUB PAGES
1. Décompresse cette archive.
2. Ouvre ton dépôt GitHub qui héberge déjà Road to X PWA.
3. Remplace à la racine les fichiers index.html, app.js, style.css, manifest.json
   et sw.js, ainsi que le dossier icons, par ceux de cette archive.
4. Valide avec Commit changes et attends la publication automatique de GitHub Pages.
5. Ouvre l'adresse HTTPS du site dans Safari sur l'iPhone.
6. Dans Safari : Partager → Sur l'écran d'accueil → Ajouter.

MISE À JOUR DE L'ANCIENNE APPLICATION
- La clé de cache a été passée à road-to-x-v13 ; le service worker supprime l'ancien
  cache au moment de l'activation.
- Ferme complètement l'ancienne PWA, rouvre le site publié dans Safari, puis relance
  l'icône Road to X depuis l'écran d'accueil.
- Si l'ancienne interface reste affichée, supprime le raccourci, vide les données du
  site dans Réglages iOS > Safari > Avancé > Données de sites, puis ajoute le raccourci
  à nouveau après avoir ouvert la nouvelle version.

SYNCHRONISATION PC ↔ IPHONE
- Connecte-toi avec le même projet Supabase, la même clé publique et le même compte
  que sur le PC.
- La V13 fusionne les données au démarrage et lorsque tu reviens dans l'application
  après l'avoir quittée. Les boutons Récupérer et Envoyer restent disponibles.
- Le renouvellement du jeton de session est automatique ; une reconnexion manuelle
  reste nécessaire une fois si l'ancienne session ne possède pas de refresh token.
- Pour une fusion atomique côté serveur, lance une seule fois le SQL fourni dans
  Backend/schema_v13_sync.sql depuis le SQL Editor de Supabase.

FONCTIONS V13 SUR IPHONE
- Chronomètre et choix de toutes les matières, y compris Chimie.
- Objectifs Cours / DM / TD pondérés.
- Statistiques et alertes de régularité des matières et des sujets.
- Historique d'hygiène sur sept jours, couleurs du brossage, journal alimentaire
  quantifié et rang alimentaire.
- Rangs de travail, humain, alimentaire et Dîn ; page Dîn séparée.
- Emploi du temps du lundi au vendredi, notes, colles, calendrier et temps numérique.

À SAVOIR
Le suivi Temps numérique sur iPhone affiche les données produites par l'extension
installée sur ton navigateur PC. L'extension de suivi elle-même est destinée aux
navigateurs Chromium sur ordinateur, pas à Safari iOS.

CORRECTIF V13.1 : rang humain + alimentaire dans Hygiène, rang Dîn dans Dîn, trois rangs personnels ensemble dans Rang. Les rangs restent visibles en haut de chaque rubrique.
