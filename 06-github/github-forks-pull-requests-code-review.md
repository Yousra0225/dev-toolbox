# 🐙 GitHub : forks, pull requests & code review

## 🍴 Le Fork
Un **Fork** est une copie d'un dépôt appartenant à quelqu'un d'autre sur votre propre compte GitHub. Cela vous permet d'expérimenter sans affecter le projet original.

## 🔀 Pull Requests (PR)
Une **Pull Request** est la méthode utilisée pour proposer vos changements au projet original (ou à la branche principale de votre équipe).

### Cycle d'une PR :
1. Vous travaillez sur une branche `feature`.
2. Vous poussez la branche sur GitHub : `git push origin feature`.
3. Sur GitHub, vous cliquez sur "Compare & pull request".
4. Vous décrivez vos changements.

## 🧐 Code Review
C'est l'étape où vos collègues (ou les mainteneurs du projet) lisent votre code avant de l'accepter.

- **Commentaires** : Ils peuvent poser des questions ou suggérer des améliorations.
- **Approve** : Le code est validé.
- **Request Changes** : Vous devez modifier votre code avant qu'il ne soit fusionné.

### Synchroniser son fork (Upstream)
Pour récupérer les nouveautés du projet original :
```bash
git remote add upstream <url_projet_original>
git fetch upstream
git checkout main
git merge upstream/main
```
