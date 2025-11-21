# Backloggd Tierlist

Outil local permettant de récupérer ses jeux Backloggd via un script, puis de générer une tierlist personnalisée depuis une page web.

---

## Structure du projet

Le projet fonctionne en deux étapes :

### 1. Extraction depuis Backloggd
- Aller sur : `https://backloggd.com/u/<votre_nom>/games/played`
- Ouvrir la console (F12) et coller le script d’extraction fourni dans l’onglet "Console".
- Le script récupère tous vos jeux joués et télécharge un fichier JSON contenant :
  {
    "title": "...",
    "cover_url": "..."
  }
- Placer ce fichier JSON dans le même dossier que `index.html`. (Remplace le placeholder actuelle)

### 2. Générateur de tierlist (index.html)
- Ouvrir la page HTML en double-cliquant sur le fichier.
- La page charge automatiquement votre JSON et affiche toutes les jaquettes dans UNRANKED.

---

## Fonctionnalités principales

- Glisser-déposer des jeux entre catégories.
- Ajouter, renommer, recolorer, supprimer ou réorganiser des catégories.
- Import/export de la tierlist en JSON pour sauvegarde.
- Export PNG de la tierlist.

---

## Notes

- Si vous rafraîchissez la page, votre tierlist sera réinitialisée. Pensez à sauvegarder régulièrement en exportant le JSON.
- L’export PNG prend en compte le niveau de zoom de la page. N’hésitez pas à zoomer ou dézoomer pour faciliter le tri ou améliorer le rendu lors de l’export PNG.
