# 🛠️ Installation & mise à jour du système

## 📦 Gestionnaires de paquets
Chaque famille de distribution a son propre outil pour installer des logiciels :

- **Debian / Ubuntu / Mint** : `apt`
- **Arch / Manjaro** : `pacman`
- **Fedora / CentOS / RHEL** : `dnf`

## 🔄 Commandes de mise à jour

### Debian / Ubuntu
```bash
sudo apt update          # Met à jour la liste des paquets
sudo apt upgrade         # Installe les nouvelles versions des paquets
sudo apt full-upgrade    # Mise à jour complète (gère les changements de dépendances)
```

### Arch Linux
```bash
sudo pacman -Sy          # Met à jour la base de données
sudo pacman -Su          # Met à jour le système
sudo pacman -Syu         # Les deux en une seule commande (recommandé)
```

### Fedora
```bash
sudo dnf check-update    # Vérifie les mises à jour
sudo dnf upgrade         # Applique les mises à jour
```

## 🧹 Nettoyage du système
Pour libérer de l'espace après des installations :

- **APT** : `sudo apt autoremove && sudo apt autoclean`
- **Pacman** : `sudo pacman -Rns $(pacman -Qtdq)` (supprime les dépendances orphelines)
- **DNF** : `sudo dnf autoremove`
