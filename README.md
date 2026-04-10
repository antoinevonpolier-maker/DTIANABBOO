# VACOA — Générateur de Dossier Technique

Outil HTML autonome pour transformer un CV ou un DT source (PDF/TXT ou texte collé) en dossier technique au format VACOA.

## Usage

1. Ouvrir `vacoa_dt_generator.html` (ou le publier comme `index.html`).
2. Choisir l’entreprise au démarrage : **NAVYS**, **VACOA** ou **GINKO**.
3. Déposer un CV/DT source ou coller le texte.
4. Renseigner le contact consultant (nom/email).
5. Cliquer sur **Générer le Dossier Technique**.
6. Exporter via **Télécharger PDF** ou **Imprimer**.

## Déploiement GitHub Pages (simple)

1. Créer un dépôt GitHub.
2. Ajouter le fichier en le renommant `index.html`.
3. Aller dans **Settings > Pages**.
4. Choisir **Deploy from a branch** puis la branche `main` et le dossier `/ (root)`.
5. Partager l’URL GitHub Pages générée.

## Mode "vraie IA" (backend recommandé)

Le front peut appeler un backend si vous renseignez **URL backend IA** dans le formulaire.

### Backend local rapide

1. Aller dans le dossier `backend`.
2. Copier `.env.example` en `.env` et renseigner `ANTHROPIC_API_KEY`.
3. Installer et démarrer :
   - `npm install`
   - `npm start`
4. Renseigner dans l’UI : `http://localhost:8787/api/generate-dt`

## Confidentialité

- Le traitement est local navigateur (pas de clé API requise).
- Aucune sauvegarde serveur n’est effectuée par cette page HTML.
