# 🐙 GitHub CLI : installation & authentification

## 🤖 Qu'est-ce que GitHub CLI (gh) ?
`gh` est l'outil officiel pour utiliser GitHub directement depuis votre terminal. Il permet de gérer les Issues, les PR et les dépôts sans ouvrir votre navigateur.

## 📥 Installation
- **Ubuntu/Debian** : `sudo apt install gh`
- **Arch Linux** : `sudo pacman -S github-cli`
- **macOS** : `brew install gh`

## 🔐 Authentification
Pour connecter votre terminal à votre compte GitHub :
```bash
gh auth login
```
Suivez les instructions (choisissez GitHub.com, SSH ou HTTPS, et authentifiez-vous via le navigateur ou avec un jeton d'accès personnel).

## ✅ Vérifier le statut
```bash
gh auth status
```
Cela vous indiquera quel compte est actuellement connecté.
