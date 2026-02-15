# 🚀 Git avancé : stash & rebase

## 📦 Git Stash (Mettre de côté)
Vous travaillez sur quelque chose mais vous devez changer de branche en urgence sans committer ? Utilisez le stash.

- `git stash` : Met vos changements de côté dans une pile temporaire.
- `git stash list` : Voir vos éléments mis de côté.
- `git stash pop` : Récupère et applique les derniers changements mis de côté.
- `git stash apply` : Applique les changements sans les supprimer de la pile.

## 🔀 Git Rebase (Réorganiser)
Le rebase est une alternative au merge. Il permet de "déplacer" toute une branche au sommet d'une autre branche.

### Pourquoi ?
Pour garder un historique linéaire et propre, sans commits de fusion ("Merge branch...").

### Comment ?
1. `git checkout feature`
2. `git rebase main`

**Attention :** N'utilisez jamais `rebase` sur une branche partagée avec d'autres développeurs (car cela réécrit l'historique).
