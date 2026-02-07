# Parlement JPV

Site internet du Parlement JPV — Initiative du CVL du Lycée Jean-Pierre Vernant

## À propos

Le **Parlement JPV** est une initiative lycéenne qui vise à promouvoir la parole, le débat démocratique et l'engagement citoyen chez les élèves.

## Publication du site

Ce site est automatiquement publié sur GitHub Pages via GitHub Actions.

### Configuration requise

Pour publier le site, il faut :

1. **Activer GitHub Pages dans les paramètres du dépôt** :
   - Allez dans `Settings` > `Pages`
   - Sous "Build and deployment", sélectionnez `Source: GitHub Actions`
   - Le site sera publié à l'adresse : `https://parlementjpv.github.io/parlement-jpv/`

2. **Le workflow se déclenchera automatiquement** :
   - À chaque push sur la branche `main` ou `master`
   - Ou manuellement via l'onglet "Actions" dans GitHub

### Structure du projet

```
parlement-jpv/
├── index.html              # Page d'accueil du site
├── .github/
│   └── workflows/
│       └── deploy.yml      # Workflow de déploiement GitHub Actions
└── README.md               # Ce fichier
```

## Développement local

Pour tester le site localement :

```bash
# Serveur Python simple
python3 -m http.server 8000

# Ou avec Node.js
npx serve .
```

Puis ouvrez http://localhost:8000 dans votre navigateur.

## Contribution

Pour modifier le site :

1. Clonez le dépôt
2. Modifiez `index.html`
3. Testez localement
4. Committez et pushez vos changements
5. Le site sera automatiquement mis à jour via GitHub Actions

## Licence

© Parlement JPV — Lycée Jean-Pierre Vernant
