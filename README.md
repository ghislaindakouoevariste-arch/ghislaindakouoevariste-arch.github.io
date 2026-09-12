# Portfolio — DAKOUO Ghislain Evariste Gnizi

Site personnel d'un élève analyste statisticien de l'ISSEA (Yaoundé).
Page unique, bilingue français / anglais, avec thème sombre et clair.

## Contenu du dépôt

```
index.html              la page complète (HTML, CSS et JavaScript réunis)
favicon.svg             icône affichée dans l'onglet du navigateur
.nojekyll               indique à GitHub Pages de servir les fichiers tels quels
assets/                 photo de profil et captures des projets
certificats/            les 8 certificats en PDF, ouverts depuis la section Certifications
cv/                     le CV en PDF, ouvert depuis le bouton « Voir mon CV »
```

## Mettre le site en ligne avec GitHub Pages

1. Créer un dépôt public nommé exactement `ghislaindakouoevariste-arch.github.io`.
2. Y téléverser **le contenu** de ce dossier (pas le dossier lui-même) :
   `index.html` doit se trouver à la racine du dépôt.
3. Ouvrir `Settings` → `Pages`, choisir la branche `main` et le dossier `/ (root)`,
   puis enregistrer.
4. Le site est accessible quelques minutes plus tard à l'adresse
   `https://ghislaindakouoevariste-arch.github.io`.

Netlify fonctionne aussi : déposer le dossier sur https://app.netlify.com/drop met
le site en ligne immédiatement, sans configuration.

## Modifier le site

Tout est dans `index.html`.

- **Textes français** : directement dans le HTML.
- **Textes anglais** : dans l'objet `I18N.en` du script, en bas du fichier.
  Chaque texte traduisible porte un attribut `data-i18n="clé"` ; la même clé
  se retrouve dans `I18N.en`.
- **Certifications** : dans le tableau `CERTS` du script. Pour en ajouter une,
  copier un bloc existant, déposer le PDF dans `certificats/` et renseigner
  son chemin dans le champ `file`.
- **Couleurs** : dans le bloc `:root` en haut de la feuille de style
  (`--teal`, `--gold`), puis `[data-theme="dark"]` et `[data-theme="light"]`.
- **Niveaux de compétence** : attribut `data-w` de chaque `<i>` dans les barres,
  exprimé en pourcentage.

## Remplacer le CV

Déposer le nouveau fichier dans `cv/` sous le nom `CV_Ghislain_DAKOUO.pdf`,
ou modifier le lien du bouton « Voir mon CV » dans `index.html`.

## Contact

ghislaindakouoevariste@gmail.com
