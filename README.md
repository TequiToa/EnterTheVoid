
# Enter The Void
This is my First **Linux Rice**, my goal is to have a highly custom and performing system to use daily to play games and code. 
Also learning more about linux and his packages and documenting everything :grin:.

/!\ under construction, in English and French /!\

| System| Technology| *Link*| 
|:------------- |:-------------|-------------| 
| DE      | KDE ou HerbsluftWM with polybar|
|Shell| zsh omzsh|
|Prompt|Starship|https://github.com/starship/starship
|Terminal|Kitty|https://sw.kovidgoyal.net/kitty/
|Icons|Papirus| 
|Color Scheme|Catppucin|https://github.com/catppuccin/catppuccin
|Notification daemon|Dunst

sudo xbps-install xorg sddm herbstluftwm polybar xsetroot feh 

## System Packages
### VPM
**VPM** pour "**Void Package Manager**", c'est un outil de gestion de paquets pour Void Linux. Il permet d'installer, de mettre à jour et de supprimer des paquets sur votre système Void. VPM utilise les dépôts officiels de Void pour les paquets, ainsi que les dépôts de la communauté pour certains paquets tiers. Il est similaire à d'autres gestionnaires de paquets tels que APT pour Debian et Ubuntu, ou Pacman pour Arch Linux.

[VPM Cheatsheet](./VPMCheatSheet.md)

### TEXT EDITOR
#### CLI
nano
#### CODE
VS CODE

### HTOP
**HTOP** est une alternative améliorée de la commande "top", qui affiche les processus système en temps réel et peut vous aider à diagnostiquer les problèmes de performances de votre système.

### neofetch
**neofetch** est un programme qui affiche des informations système telles que le nom de la distribution, la version du noyau et les spécifications de l'ordinateur. Cela peut être utile pour vérifier rapidement les caractéristiques de votre système.

## Graphics package
### Pilotes Nvidia 
Vous devez installer les pilotes Nvidia pour que votre carte graphique fonctionne correctement. Les pilotes propriétaires de Nvidia peuvent être téléchargés sur leur site web officiel ou installés à partir du gestionnaire de paquets de votre distribution Linux.

### Vulkan 
Si vous voulez jouer à des jeux qui prennent en charge la technologie **Vulkan**, vous devez installer le pilote **Vulkan** pour votre carte graphique Nvidia. **Vulkan** est une API de rendu graphique qui peut offrir de meilleures performances que OpenGL.

## Power Management 
Il est important de gérer l'énergie de votre ordinateur portable lorsque vous jouez à des jeux pour éviter les problèmes de surchauffe. Utilisez des outils tels que **tlp** ou **powertop** pour gérer l'énergie de votre système.

### TLP
**TLP** est un outil open source pour Linux qui permet d'optimiser l'utilisation de l'énergie sur les ordinateurs portables afin d'améliorer la durée de vie de la batterie. Il s'agit d'un programme en ligne de commande qui ajuste automatiquement les paramètres d'alimentation de divers composants matériels tels que le processeur, le disque dur, le Wi-Fi, le Bluetooth, etc. TLP permet également de surveiller l'état de la batterie et fournit des informations sur sa capacité, sa tension et son état de santé. Il est compatible avec la plupart des distributions Linux et peut être installé via les gestionnaires de paquets.
 https://linrunner.de/tlp/
 
### ACPI
**ACPI** (Advanced Configuration and Power Interface) est utilisé pour la gestion de l'énergie et des périphériques sur votre ordinateur portable. Bien que la prise en charge d'ACPI sous Linux soit généralement bonne, vous pouvez rencontrer des problèmes avec certains composants matériels. Assurez-vous que votre distribution Linux prend en charge ACPI et vérifiez si les fonctionnalités d'économie d'énergie fonctionnent correctement.

## Game Performances Packages
Gamemode et Magohud sont deux outils destinés aux joueurs sous Linux qui cherchent à améliorer les performances de leurs jeux.

### Gamemode
**Gamemode** est un démon système qui permet d'optimiser les performances du système pour les jeux. Il utilise des techniques d'optimisation telles que l'ajustement de la fréquence du processeur et la désactivation des services non essentiels pour améliorer les performances des jeux. Gamemode peut être utilisé avec n'importe quel jeu sous Linux et il est compatible avec différentes distributions Linux.

### Magohud
**Magohud**, quant à lui, est un script personnalisé qui permet d'afficher des statistiques de performances de jeux, telles que les FPS, la latence, la consommation de GPU et d'autres informations utiles en jeu. Le script Magohud s'appuie sur les bibliothèques de profilage et d'instrumentation disponibles sous Linux pour surveiller les performances du système en temps réel.

Les deux outils peuvent être utilisés conjointement pour optimiser les performances des jeux sous Linux. En effet, Gamemode permet d'optimiser le système pour les jeux, tandis que Magohud permet de surveiller les performances du système pendant le jeu.

En utilisant ces deux outils, les joueurs sous Linux peuvent améliorer considérablement les performances de leurs jeux, réduire la latence et les temps de chargement, et obtenir une meilleure expérience de jeu globale.

### Steam 
**Steam** est un service de distribution de jeux populaire pour Linux, avec une grande sélection de jeux disponibles pour jouer.
```bash
sudo vpm install steam
```
## Media Packages
### Videos Player
#### MPV
**MPV** est un lecteur multimédia open-source et gratuit pour les systèmes d'exploitation Linux, macOS et Windows. Il est basé sur MPlayer et mplayer2, qui sont des lecteurs multimédia populaires mais qui ne sont plus maintenus activement. Mpv prend en charge une large gamme de formats de fichiers multimédias et est connu pour sa légèreté et sa simplicité d'utilisation. Il est également entièrement personnalisable grâce à son support de scripts Lua et son architecture de plug-in.

#### VLC
**VLC** est un lecteur multimédia populaire qui peut lire une grande variété de formats de fichiers audio et vidéo.

#### ani-cli
**ani-cli** : https://github.com/pystardust/ani-cli

### Music player
[Music](./ChatGptSpotifyConfig.md)

### E-book and Manga Reader
#### cbz reader
**zathura**

## Font
Monolisa patched with nerdfonts : https://github.com/nibirrayy/MonoLisa-nerdpatched

## Other Packages
### Bottles
**Bottles** facilite grandement l'utilisation de Wine en fournissant une interface graphique intuitive pour la gestion des configurations et des environnements virtuels de Wine. Il permet également de créer et de gérer plusieurs configurations de Wine pour différentes applications Windows, ce qui peut être très utile si vous avez besoin de faire fonctionner plusieurs applications Windows sur votre système Linux.

De plus, Bottles offre une intégration transparente avec le système de fichiers Linux, ce qui permet d'accéder facilement aux fichiers de l'application Windows depuis votre système de fichiers Linux. Cela rend également les fichiers de l'application Windows disponibles pour les sauvegardes, les restaurations et les transferts de fichiers.

Bottles est disponible pour plusieurs distributions Linux, dont Ubuntu, Fedora, Debian, Manjaro et Arch Linux. Il est également open source et gratuit à utiliser.

[Additional Ressources and inspirations]
- https://www.reddit.com/r/unixporn/comments/138ht06/kde_catppuccin_setup_of_my_dreams/
- https://www.reddit.com/r/unixporn/comments/1354so3/oc_rofigames_a_small_rust_program_which_lets_you/
- https://i.redd.it/d68v5rl608ya1.png
