

# Portfolio — Adamou Hassane Boubacar (Modèle Tailwind)

Prototype de portfolio moderne en français, basé sur Tailwind via CDN (facile pour prototyper et déployer). Ce modèle a été personnalisé pour `Boubacar` — étudiant en télécommunications et réseaux informatiques.

Fichiers créés :
 - `index.html` — page principale (hero, à propos, projets, contact, footer) personnalisé pour `Adamou Hassane Boubacar`.

Aperçu local :
1. Ouvre `c:/Users/PC/Documents/Projet1/Portofolio/index.html` dans ton navigateur.
2. Option recommandée : installe l'extension "Live Server" dans VS Code et lance "Open with Live Server" pour rechargement en direct.

Contenu personnalisé :
- Bio : étudiant en télécommunications et réseaux informatiques.
- Projets : simulation réseau (VMware Workstation), installation & configuration de systèmes, configuration d'équipements réseau.
- Email de contact : `boubacar67op@gmail.com`.
- CV ajouté : `assets/Boubacar_CV.pdf` (présent dans le dossier `assets`).

Personnalisation rapide :
- Remplace les textes de projet par des liens vers tes rapports ou dépôts.
- Ajoute une photo professionnelle dans le dossier et mets à jour la balise `<img>`.

Déployer :
- GitHub Pages : push du dossier sur un repo et activer GitHub Pages sur la branche `main`.
- Vercel / Netlify : glisse-dépose du dossier ou connecte le repo.

Déploiement automatique (préparé) :
- Un workflow GitHub Actions (`.github/workflows/deploy.yml`) a été ajouté pour déployer automatiquement le contenu du dépôt sur la branche `gh-pages` à chaque push sur `main`.

Étapes recommandées pour GitHub Pages (PowerShell) :
1. Crée un repository sur GitHub (nom par ex. `portfolio`).
2. Dans le dossier du projet, initialise git et pousse sur GitHub :

```powershell
cd 'C:\Users\PC\Documents\Projet1\Portofolio'
git init
git add .
git commit -m "Initial commit - portfolio"
git branch -M main
git remote add origin https://github.com/TON_COMPTE_GITHUB/portfolio.git
git push -u origin main
```

Remplace `TON_COMPTE_GITHUB` par ton nom d'utilisateur GitHub. Après le push, GitHub Actions déclenchera le déploiement vers la branche `gh-pages`. Sur la page du repo -> `Actions`, tu peux suivre le workflow. Quand il est terminé, ton site sera disponible à `https://TON_COMPTE_GITHUB.github.io/portfolio`.

Si tu préfères déployer via Vercel (plus simple pour les mises à jour instantanées) :
- Crée un compte sur `vercel.com` et connecte ton repo GitHub, ou utilise "Import Project" et choisis le dossier. Vercel détecte automatiquement un site statique.

Dis-moi quelle option tu veux utiliser (GitHub Pages ou Vercel/Netlify) — je peux te guider pas-à-pas et renommer le CV si tu veux que le fichier porte ton nom complet.

Script d'aide pour push (PowerShell)
- J'ai ajouté un script `push.ps1` à la racine du projet pour automatiser l'initialisation git, la configuration du remote et le push vers GitHub.
- Pour l'utiliser :
	1. Ouvre PowerShell.
	2. Va dans le dossier du projet : `cd 'C:\Users\PC\Documents\Projet1\Portofolio'` ou laisse vide si tu lances depuis le dossier.
	3. Exécute :

```powershell
.\push.ps1
```

Le script te demandera l'URL du repository GitHub (ex: `https://github.com/TON_COMPTE_GITHUB/portfolio.git`). Si tu as l'authentification à deux facteurs (2FA), utilise un Personal Access Token (PAT) comme mot de passe lors du push.

Si tu veux, je peux renommer automatiquement `assets/Boubacar_CV.pdf` en `assets/Adamou_Hassane_Boubacar_CV.pdf` et mettre à jour le lien dans `index.html` (dis "renomme CV" si tu veux que je le fasse).

Prochaines options — veux-tu que je :
- ajoute une photo, optimise les images et les miniatures,
- applique une palette couleur personnalisée et une police, ou
- convertisse le template en `React + Tailwind` pour plus d'évolutivité ?
