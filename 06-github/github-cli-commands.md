# 🐙 GitHub CLI : commandes courantes

## 📁 Gérer les dépôts (repo)
- `gh repo create` : Créer un nouveau dépôt sur GitHub.
- `gh repo fork` : Forker un dépôt.
- `gh repo view --web` : Ouvrir la page du dépôt actuel dans le navigateur.

## 🔀 Gérer les Pull Requests (pr)
- `gh pr create` : Créer une Pull Request depuis votre branche actuelle.
- `gh pr list` : Voir les PR ouvertes.
- `gh pr checkout <numéro>` : Télécharger et basculer sur la branche d'une PR.
- `gh pr merge` : Fusionner la PR actuelle.

## 🐛 Gérer les Tickets (issue)
- `gh issue list` : Voir les tickets ouverts.
- `gh issue create` : Créer un nouveau ticket.
- `gh issue view <numéro> --web` : Voir un ticket dans le navigateur.

## 🛠️ Astuce : les alias de gh
Vous pouvez créer des raccourcis pour les commandes gh :
`gh alias set pv 'pr view --web'`
Désormais, `gh pv` ouvrira la PR en cours dans le navigateur.
