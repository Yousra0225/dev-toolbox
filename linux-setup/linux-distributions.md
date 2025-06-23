# 🐧 Linux et les distributions

## Qu’est-ce que Linux ?

Linux est un **noyau** (kernel), c’est-à-dire le cœur d’un système d’exploitation.  
Les systèmes GNU/Linux que l’on utilise (Ubuntu, Fedora, Arch...) sont des distributions : des combinaisons du noyau Linux + des outils/utilitaires + une gestion des paquets.

## 🌱 Distributions
```bash
                        [ Linux Kernel ]
                               |
    ------------------------------------------------
    |                    |                         |
 [Debian]            [Arch Linux]              [RedHat/Fedora]
    |                    |                         |
[Ubuntu]           [Manjaro..]     [Fedora, CentOS..]
    |
[Linux Mint]
```

Une **distribution** linux est un _ensemble prêt à l'emploi_ basé sur Linux.  
Chaque distribution a ses particularités :

| Distribution | Gestionnaire de paquets | Particularités                 |
| ------------ | ----------------------- | ------------------------------ |
| Debian       | `apt`                   | Très stable, base de Ubuntu    |
| Ubuntu       | `apt` (Debian-based)    | Stable, support large          |
| Arch Linux   | `pacman`                | Rolling release, très custom   |
| Manjaro      | `pacman` + GUI          | Arch friendly, plus accessible |
| Fedora       | `dnf`                   | Innovant, proche de RedHat     |
