# 🌊 GitFlow : commandes et bonnes pratiques

## 🛠️ Utiliser GitFlow
Il existe un outil en ligne de commande pour simplifier l'utilisation de ce modèle : `git-flow`.

### Initialisation
```bash
git flow init  # Acceptez les noms de branches par défaut
```

### Travailler sur une fonctionnalité
```bash
git flow feature start mon-nom-de-feature
# ... faire des commits ...
git flow feature finish mon-nom-de-feature
```

### Préparer une version (Release)
```bash
git flow release start 1.0.0
# ... derniers réglages ...
git flow release finish 1.0.0
```

## ✅ Bonnes pratiques
1. **Ne jamais travailler directement sur main** : Tout doit passer par une branche `feature` ou `develop`.
2. **Faire des petits commits** : Plus facile à relire et à annuler si besoin.
3. **Utiliser des messages de commit explicites** : Expliquez *pourquoi* vous avez fait ce changement.
4. **Rester synchronisé** : Faites souvent des `git pull` pour éviter les gros conflits à la fin.
