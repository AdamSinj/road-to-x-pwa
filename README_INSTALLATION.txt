ROAD TO X — PWA V2

Cette version reprend le format de données JSON de Road to X PC V12/V12.1 et utilise le même schéma Supabase.

INSTALLATION / MISE À JOUR iPhone
1. Déployer le contenu de ce dossier sur le même hébergement HTTPS que ta PWA actuelle (remplacer les anciens fichiers).
2. Sur iPhone, ouvrir l’URL dans Safari.
3. Actualiser la page, puis Partager > Ajouter à l’écran d’accueil.
4. Si l’ancienne icône reste sur l’écran d’accueil, supprimer l’ancien raccourci puis ajouter le nouveau.
5. Ouvrir Réglages dans l’app et se connecter au même projet Supabase. Si le PC contient les données les plus récentes, faire d’abord PC → cloud, puis récupérer le cloud sur iPhone.

FONCTIONS
- Accueil avec rang général et rang humain.
- Emploi du temps hebdomadaire et programme de colles.
- Calendrier avec samedi rouge, aujourd’hui jaune, colles orange.
- Objectifs, statistiques en trois vues, rangs, Dîn, hygiène, sujets et notes.
- Chronomètre horodaté : le temps continue de s’écouler en arrière-plan et se recalcule au retour dans l’app.

LIMITES iOS
Une PWA ne peut pas créer de fenêtre flottante au-dessus des autres apps, ni afficher un chrono personnalisé persistant sur l’écran verrouillé. Il faut une application iOS native et une Live Activity (ActivityKit) pour cela. Les widgets iOS nécessitent également une extension WidgetKit native.

STATISTIQUES
- Composition quotidienne : axe fixe 0–24 h, segments normalisés si les données se chevauchent.
- Camembert : uniquement les heures de travail enregistrées, ventilées par matière.
- Ratio quotidien : échelle fixe 0–100 %.
