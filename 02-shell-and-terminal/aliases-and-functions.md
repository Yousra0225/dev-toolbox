# ⚙️ Alias et fonctions pour automatiser

## 📝 Les Alias
Un alias est un raccourci pour une commande longue ou complexe. On les définit généralement dans `.bashrc` ou `.zshrc`.

### Exemples d'alias utiles :
```bash
alias ll='ls -lah'               # Liste détaillée avec fichiers cachés
alias gs='git status'            # Raccourci git ultra fréquent
alias update='sudo apt update && sudo apt upgrade'
alias ..='cd ..'
alias ...='cd ../..'
```

## 🛠️ Les Fonctions
Les fonctions sont plus puissantes que les alias car elles acceptent des arguments.

### Exemple : Créer un dossier et y entrer immédiatement
```bash
mkd() {
    mkdir -p "$1"
    cd "$1"
}
```

### Exemple : Extraire n'importe quelle archive
```bash
extract() {
    if [ -f $1 ] ; then
        case $1 in
            *.tar.bz2)   tar xjf $1     ;;
            *.tar.gz)    tar xzf $1     ;;
            *.bz2)       bunzip2 $1     ;;
            *.rar)       unrar x $1     ;;
            *.gz)        gunzip $1      ;;
            *.tar)       tar xf $1      ;;
            *.tbz2)      tar xjf $1     ;;
            *.tgz)       tar xzf $1     ;;
            *.zip)       unzip $1       ;;
            *.Z)         uncompress $1  ;;
            *.7z)        7z x $1        ;;
            *)           echo "'$1' cannot be extracted via extract()" ;;
        esac
    else
        echo "'$1' is not a valid file"
    fi
}
```

## 🔄 Appliquer les changements
Après avoir modifié votre fichier de config (`.bashrc` ou `.zshrc`), n'oubliez pas de recharger :
`source ~/.zshrc` (ou `.bashrc`)
