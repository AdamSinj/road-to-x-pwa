ROAD TO X — PWA V1 (prototype web installable)

IMPORTANT
Cette PWA est une première version web indépendante de l'application Windows. Elle reprend les données principales du format JSON V12 (agenda, objectifs, séances de travail, sujets traités, notes et jalons TIPE). Elle n'est pas encore une reproduction exhaustive de toutes les rubriques PC (colloscope, rangs détaillés, hygiène, Dîn, etc.).

HÉBERGEMENT GRATUIT AVEC GITHUB PAGES
1. Créer/ouvrir un compte sur https://github.com
2. Créer un dépôt public nommé road-to-x-pwa.
3. Dans le dépôt, cliquer Add file > Upload files.
4. Décompresser ce ZIP puis téléverser TOUS les fichiers et dossiers contenus dans Road_to_X_PWA_V1 (index.html, app.js, style.css, manifest.json, sw.js, icons/).
5. Cliquer Commit changes.
6. Ouvrir Settings > Pages.
7. Dans Build and deployment, choisir Deploy from a branch, puis Branch: main et Folder: / (root), puis Save.
8. Attendre la publication. L'adresse sera https://TON-PSEUDO.github.io/road-to-x-pwa/ (remplacer TON-PSEUDO par le pseudo GitHub exact).

INSTALLER SUR IPHONE
1. Ouvrir l'adresse publiée dans Safari (pas dans un navigateur intégré à une autre application).
2. Appuyer sur Partager.
3. Choisir Ajouter à l'écran d'accueil.
4. Activer « Ouvrir comme app web » si l'option apparaît, puis Ajouter.

SYNCHRONISATION SUPABASE
1. Ouvrir ⚙ dans Road to X.
2. Saisir la même URL Supabase, la même clé publique anon/publishable et le même compte que sur le PC.
3. Saisir l'e-mail et le mot de passe Supabase, puis « Se connecter et récupérer mes données ».
4. Si des données existent dans le cloud, confirmer leur récupération pour charger le même payload que le PC.

PRUDENCE DONNÉES
- La première connexion peut remplacer les données locales de cet iPhone par celles du cloud : choisir soigneusement.
- Les modifications sont envoyées automatiquement au cloud après un court délai lorsque la session est active.
- La PWA ne synchronise pas directement avec le fichier JSON local du PC : elle passe par la même table Supabase road_to_x_sync.
- Ce prototype est à tester avant de lui confier les seules copies de données importantes. Faire régulièrement un export JSON depuis Plus > Données.
- Ne jamais publier de mot de passe ou de clé secrète dans GitHub. La PWA ne contient aucune clé privée, uniquement la clé publique Supabase.
