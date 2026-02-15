# 🌿 Git : installation & configuration

## 📥 Installation
- **Ubuntu / Debian** : `sudo apt install git`
- **Arch Linux** : `sudo pacman -S git`
- **Fedora** : `sudo dnf install git`

## ⚙️ Configuration initiale
Avant de commencer, vous devez vous identifier pour que vos commits soient signés.

```bash
git config --global user.name "Votre Nom"
git config --global user.email "votre@email.com"
```

### Vérifier la configuration
```bash
git config --list
```

## 🔑 Configuration de SSH (Recommandé)
Pour éviter de taper votre mot de passe à chaque fois, utilisez une clé SSH.

1. Générer une clé : `ssh-keygen -t ed25519 -C "votre@email.com"`
2. Copier la clé publique : `cat ~/.ssh/id_ed25519.pub`
3. Ajouter cette clé sur votre profil GitHub / GitLab.

## 📄 Le fichier .gitignore
Ce fichier à la racine de votre projet permet d'ignorer les fichiers inutiles (logs, dossiers de dépendances comme `node_modules`, fichiers de config secrets).

Exemple de `.gitignore` simple :
```text
node_modules/
.env
*.log
dist/
```
