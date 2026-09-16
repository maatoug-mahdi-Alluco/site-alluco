# GitHub + Vercel — étapes simples

## 1. Envoyer les fichiers sur GitHub

Le contenu de ce dossier doit être directement à la racine du repository.

```bash
git init
git add .
git commit -m "ALLUCO professional 3D website"
git branch -M main
git remote add origin https://github.com/maatoug-mahdi-Alluco/site-web-ia-3d.git
git push -u origin main
```

Si le repository existe déjà, remplace simplement son ancien contenu par ce projet puis commit/push.

## 2. Déployer

Utilise Vercel, pas Streamlit.

- Repository: `maatoug-mahdi-Alluco/site-web-ia-3d`
- Production branch: `main`
- Framework: Next.js
- Root Directory: `./`
- Build Command: `npm run build`
- Install Command: `npm install`
- Output Directory: automatique

Il n'y a aucun champ `Main file path` à renseigner pour Next.js.
