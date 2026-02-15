# 🌿 Git : branches et fusion

## 🎋 Pourquoi utiliser des branches ?
Les branches permettent de travailler sur une nouvelle fonctionnalité ou un correctif sans polluer le code principal (`main` ou `master`).

## 🛠️ Gérer les branches
- `git branch` : Liste les branches locales.
- `git branch <nom>` : Crée une nouvelle branche.
- `git checkout <nom>` : Bascule sur une branche.
- `git checkout -b <nom>` : Crée et bascule sur la branche en une commande.
- `git branch -d <nom>` : Supprime une branche (si elle a été fusionnée).

## 🔀 Fusionner (Merge)
Pour ramener les changements d'une branche `feature` vers `main` :

1. Aller sur main : `git checkout main`
2. Fusionner : `git merge feature`

### ⚠️ Résoudre les conflits
Si Git ne peut pas fusionner automatiquement :
1. Il marque les fichiers en conflit.
2. Vous devez ouvrir les fichiers et choisir quelle version garder.
3. `git add <fichier>`
4. `git commit` (pour finaliser la fusion).
