# 🌿 Git : commandes fondamentales

## 🆕 Initialiser ou récupérer un projet
- `git init` : Crée un nouveau dépôt Git localement.
- `git clone <url>` : Copie un dépôt distant sur votre machine.

## 🔄 Le cycle de vie d'un fichier
1. **Modifier** des fichiers dans votre dossier.
2. `git status` : Voir quels fichiers ont été modifiés.
3. `git add <fichier>` : Ajouter le fichier à l'**Index** (Staging area).
   - `git add .` pour ajouter tous les fichiers.
4. `git commit -m "Message clair"` : Enregistrer les modifications dans l'**Historique**.
5. `git push` : Envoyer les modifications vers le dépôt distant.

## 🔍 Examiner l'historique
- `git log` : Liste tous les commits (Entrée pour descendre, Q pour quitter).
- `git log --oneline --graph --all` : Version visuelle et compacte de l'historique.
- `git diff` : Voir les changements non enregistrés.

## ⏪ Annuler des changements
- `git checkout -- <fichier>` : Annule les modifications non commitées d'un fichier.
- `git reset HEAD~1` : Annule le dernier commit mais garde les fichiers modifiés.
- `git reset --hard HEAD~1` : Annule le dernier commit et perd tous les changements (Attention !).
