# 🐚 Shells : Bash vs Zsh

## 📖 Qu'est-ce qu'un Shell ?
Le shell est l'interface textuelle qui interprète vos commandes. Bien que Bash soit le standard, Zsh est devenu très populaire pour ses fonctionnalités avancées.

## 🐢 Bash (Bourne Again Shell)
- **Standard** : Préinstallé sur la quasi-totalité des systèmes Linux et serveurs.
- **Stable** : Peu de changements, excellent pour les scripts de déploiement.
- **Moins complet** : L'auto-complétion de base est moins intelligente que celle de Zsh.

## 🏎️ Zsh (Z Shell)
- **Moderne** : Shell par défaut sur macOS et Kali Linux.
- **Auto-complétion puissante** : Propose des menus, gère les fautes de frappe.
- **Hautement personnalisable** : Grâce à des frameworks comme **Oh My Zsh**.
- **Correction d'erreurs** : "Did you mean...?"

## 🛠️ Oh My Zsh
C'est le framework le plus utilisé pour booster Zsh. Il permet d'installer facilement des thèmes et des plugins.

### Installation de Oh My Zsh :
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Plugins recommandés :
- `git` : Affiche la branche actuelle et l'état du dépôt.
- `zsh-autosuggestions` : Suggère des commandes basées sur votre historique.
- `zsh-syntax-highlighting` : Colore les commandes en temps réel (vert si ok, rouge si erreur).
