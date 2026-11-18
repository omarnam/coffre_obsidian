# Créer un dépôt GitHub

## 1. Prérequis

- Avoir un compte [GitHub](https://github.com/).
- Avoir installé Git sur son ordinateur.
- Avoir installé Obsidian si le dépôt sert à sauvegarder ses notes.

Vérifier l'installation de Git dans le terminal :

```bash
git --version
```

## 2. Créer un dépôt sur GitHub

1. Se connecter à [GitHub](https://github.com/).
2. Cliquer sur le bouton **New repository**.
3. Saisir le nom du dépôt, par exemple `mes-notes`.
4. Ajouter une description si nécessaire.
5. Choisir la visibilité :
   - **Public** : accessible à tous.
   - **Private** : accessible uniquement aux personnes autorisées.
6. Cliquer sur **Create repository**.

## 3. Préparer le dossier local

1. Ouvrir le terminal.
2. Se déplacer dans le dossier du projet :

```bash
cd chemin/vers/mon-projet
```

3. Initialiser Git :

```bash
git init
```

4. Ajouter les fichiers au suivi :

```bash
git add .
```

5. Créer le premier commit :

```bash
git commit -m "Initial commit"
```

## 4. Relier le dossier à GitHub

1. Copier l'URL HTTPS du dépôt créé sur GitHub.
2. Déclarer la branche principale :

```bash
git branch -M main
```

3. Ajouter le dépôt distant :

```bash
git remote add origin https://github.com/UTILISATEUR/mes-notes.git
```

```

4. Envoyer les fichiers sur GitHub :

```bash
git push -u origin main
```

Remplacer `UTILISATEUR` par son nom d'utilisateur GitHub.

## 5. Mettre à jour le dépôt

Après avoir modifié les fichiers, exécuter les commandes suivantes :

1. Ajouter les modifications :

```bash
git add .
```

2. Créer un commit :

```bash
git commit -m "Mise à jour des fichiers"
```

3. Envoyer les modifications sur GitHub :

```bash
git push
```

## 6. Récupérer les dernières modifications

Pour récupérer les modifications présentes sur GitHub :

```bash
git pull
```

## 7. Commandes Git essentielles

| Commande | Fonction |
|---|---|
| `git init` | Initialise un dépôt Git |
| `git status` | Affiche l'état des fichiers |
| `git add .` | Prépare les modifications |
| `git commit -m "message"` | Enregistre les modifications localement |
| `git push` | Envoie les commits sur GitHub |
| `git pull` | Récupère les modifications distantes |
| `git log` | Affiche l'historique des commits |
| `git remote -v` | Affiche les dépôts distants configurés |

## 8. Vérification finale

1. Ouvrir la page du dépôt sur GitHub.
2. Vérifier que les fichiers apparaissent.
3. Modifier un fichier localement, puis exécuter `git add`, `git commit` et `git push`.
4. Vérifier que la modification est visible sur GitHub.

**À retenir :** `add` prépare les modifications, `commit` les enregistre localement et `push` les envoie sur GitHub.