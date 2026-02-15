# 🚀 Git avancé : réécriture d’historique

## ✏️ Modifier le dernier commit
Vous avez oublié un fichier ou fait une faute dans le message ?
`git commit --amend`

## 🧹 Rebase Interactif (Squash)
Pour nettoyer vos commits avant de faire une Pull Request (fusionner plusieurs petits commits en un seul propre).

```bash
git rebase -i HEAD~3  # Ouvre un éditeur pour les 3 derniers commits
```

Dans l'éditeur, remplacez `pick` par `squash` (ou `s`) pour les commits que vous voulez fusionner avec le précédent.

## 🚿 Nettoyer l'historique (Sensible)
Si vous avez committé par erreur un mot de passe ou un gros fichier binaire :
- **BFG Repo-Cleaner** : L'outil le plus simple pour supprimer des fichiers de tout l'historique.
- **git filter-repo** : L'alternative moderne recommandée par Git.

**⚠️ Rappel :** Réécrire l'historique nécessite souvent un `git push --force`. Soyez extrêmement prudent !
