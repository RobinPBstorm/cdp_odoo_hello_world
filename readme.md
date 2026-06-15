# Comment débuter avec git

## Installer Git

Installer git (partie software) pour exécuter de git

[Lien d'installation de git](https://git-scm.com/install/windows)

## Créer un compte github/gitlab

[homepage de github](https://github.com/)

ou

[Homepage de gitlab](https://about.gitlab.com/)

## Création d'un repository

Pour créer un nouveau nouveau repository:
- nom de dépôt unique (repository name)

- une description (optionel)
- changer la visibilité (qui peut voir le projet)

on peut choisir de rajouter des fichiers lors de la création du dépôt:
- readme.md (description du projet)
- .gitignore

## Initialiser le projet pour git

Dans le terminal, au chemin du projet,
```bash
git init
```

git va créer un dossier caché .git

## lister la modification non envoyée

```
git status
```

## préparer les fichiers pour l'envoi

Envoyer toute les modifications
```bash
git add .
```

Envoyer certain fichier
```bash
git add ./mon-fichier
```

## préparer le commit avec son message

```bash
git commit -m "mon message"
```

## Renommer la branche

```
git branch -M main
```

## Ajouter un dépôt

```bash
git remote add origin lien_du_depot
```

## Envoyer le commit sur le dépôt distant

La première fois pour relier la branche main locale à celle du dépôt (ou créer la branche distante):
```bash
git push --set-upstream origin main
```

Et les fois suivantes:
```bash
git push
```

## Créer une branche

```
git branch nom_branche
```