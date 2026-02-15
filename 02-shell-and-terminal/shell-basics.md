# 🧠 Principes de base du shell

## 🖊️ Le Prompt
Le prompt est la ligne de texte qui indique que le terminal est prêt à recevoir une commande. Il contient souvent :
`utilisateur@machine:~/dossier$ `

## 📦 Les Variables d'environnement
Elles stockent des informations utilisées par le système et les programmes.
- `echo $USER` : Affiche l'utilisateur actuel.
- `echo $PATH` : Affiche les dossiers où le shell cherche les exécutables.
- `export MY_VAR="hello"` : Définit une nouvelle variable pour la session.

## 🔗 Le Piping (Redirection)
L'une des plus grandes forces de Linux : envoyer la sortie d'une commande vers une autre.

- `|` (Pipe) : Envoie le résultat à la commande suivante.
  - Exemple : `ls -l | grep ".txt"` (Lister les fichiers et ne garder que ceux contenant ".txt").
- `>` : Redirige la sortie vers un fichier (écrase le contenu).
- `>>` : Redirige la sortie vers un fichier (ajoute à la fin).
- `<` : Lit l'entrée depuis un fichier.

## 🏃 Exécution de scripts
- Un script doit commencer par un **Shebang** (ex: `#!/bin/bash`).
- Il doit être exécutable : `chmod +x mon_script.sh`.
- Lancer le script : `./mon_script.sh`.
