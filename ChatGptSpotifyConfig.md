# Voici un résumé des étapes à suivre pour installer et configurer MPD, Ncmpcpp, Alsa, Spotifyd et Polybar sur Void Linux:
## Installer les paquets nécessaires:
```bash
sudo xbps-install mpd ncmpcpp alsa-utils spotifyd
```
## Configurer Alsa:
```bash
alsactl init
```
## Configurer MPD: Éditer le fichier de configuration /etc/mpd.conf et y ajouter les informations suivantes :
```bash
music_directory     "/home/<user>/Music"
playlist_directory  "/home/<user>/.mpd/playlists"
db_file             "/home/<user>/.mpd/mpd.db"
log_file            "/var/log/mpd/mpd.log"
pid_file            "/run/mpd/mpd.pid"
state_file          "/home/<user>/.mpd/mpdstate"
audio_output {
        type            "alsa"
        name            "My ALSA Device"
        device          "default"
}
```
## Démarrer le service MPD:
```bash
sudo ln -s /etc/sv/mpd /var/service/
```
## Configurer Ncmpcpp: Éditer le fichier de configuration ~/.ncmpcpp/config et y ajouter les informations suivantes :
```bash
mpd_host = "localhost"
mpd_port = "6600"
mpd_music_dir = "/home/<user>/Music"
```
## Configurer Spotifyd: Éditer le fichier de configuration /etc/spotifyd.conf et y ajouter les informations suivantes :
```bash
[global]
backend = alsa
device_name = default

[spotify]
username = <votre_nom_utilisateur_spotify>
password = <votre_mot_de_passe_spotify>
```
## Démarrer le service Spotifyd:
```bash
sudo ln -s /etc/sv/spotifyd /var/service/
```
## Ajouter Spotifyd à MPD: Éditer le fichier de configuration /etc/mpd.conf et y ajouter les informations suivantes :
```bash
audio_output {
        type            "fifo"
        name            "spotifyd"
        path            "/tmp/spotifyd.fifo"
        format          "44100:16:2"
}
```
## Démarrer le service Alsa:
```bash
sudo ln -s /etc/sv/alsa /var/service/
```
## Configurer Polybar: Éditer le fichier de configuration ~/.config/polybar/config et y ajouter les informations suivantes :
```bash
[module/spotify]
type = custom/script
exec = playerctl metadata --format '{{ artist }} - {{ title }}'
interval = 2
format-prefix = " "
click-left = "playerctl play-pause"
click-right = "playerctl next"
click-middle = "playerctl previous"
scroll-up = "playerctl next"
scroll-down = "playerctl previous"
```
## Redémarrer le service Polybar:
```bash
pkill polybar
polybar -r mybar &
```

Une fois ces étapes terminées, vous pourrez utiliser Ncmpcpp pour contrôler MPD et Spotifyd et afficher les informations de lecture en cours dans la barre Polybar.

Notez que les noms de fichiers et les chemins d'accès peuvent différer selon votre configuration. 
Il est important de remplacer <user> dans les exemples ci-dessus par votre nom d'utilisateur réel.
