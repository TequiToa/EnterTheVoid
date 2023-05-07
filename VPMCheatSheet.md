## Cheat Sheet: VPM

### Basic Usage

- `vpm install <package>` : Installe un paquet
- `vpm remove <package>` : Désinstalle un paquet
- `vpm search <query>` : Recherche des paquets correspondant à une requête
- `vpm list` : Affiche la liste des paquets installés
- `vpm info <package>` : Affiche des informations sur un paquet
- `vpm upgrade` : Met à jour tous les paquets installés

### Advanced Usage

- `vpm hold <package>` : Empêche la mise à jour d'un paquet spécifique
- `vpm unhold <package>` : Permet la mise à jour d'un paquet spécifique
- `vpm clean-cache` : Nettoie le cache des paquets téléchargés
- `vpm clean-repo` : Supprime les paquets obsolètes du dépôt
- `vpm autoremove` : Supprime les paquets inutilisés qui ont été installés comme dépendances

### Configuration

- `vpm edit-config` : Ouvre le fichier de configuration de vpm dans l'éditeur par défaut
- `vpm update-config` : Met à jour le fichier de configuration avec les paramètres par défaut
