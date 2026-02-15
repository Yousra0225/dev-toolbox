# 🌊 GitFlow : modèle de branches

## 💡 Qu'est-ce que GitFlow ?
GitFlow est un modèle d'organisation des branches pour Git. Il est particulièrement adapté aux projets qui ont des cycles de sortie (releases) planifiés.

## 🎋 Les branches principales
1. **main (ou master)** : Contient le code en production. Chaque commit sur cette branche est une version stable.
2. **develop** : C'est la branche d'intégration. Tout le développement se passe ici avant d'aller en production.

## 🎋 Les branches de support
- **feature/** : Pour développer de nouvelles fonctionnalités. Part de `develop`, revient dans `develop`.
- **release/** : Pour préparer une nouvelle version (tests finaux, corrections mineures). Part de `develop`, revient dans `main` et `develop`.
- **hotfix/** : Pour corriger un bug critique en production. Part de `main`, revient dans `main` et `develop`.

## 🎨 Schéma simplifié
```text
main      --------------------------- [v1.0] --- [v1.1]
             \                        /           /
develop       \--- [feature] --------/--- [release] ---
```
