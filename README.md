# raspberry-pi
information sur le raspberry pi
### avec Wiki
link wili
##commande pour raspbery pi:  
>cat /proc/cpuinfo  
## Commande générales:  
**apt-get update :** Met à jour votre version de Raspbian.  
**apt-get upgrade :** Met à niveau tous les logiciels que vous avez installés.  
**clear :** Efface l’écran du terminal des commandes et du texte précédemment exécutés.  
**date :** Affiche la date actuelle.  
**find / -name exemple.txt :** Rrecherche dans le système entier le fichier exemple.txt et génère une liste de tous les répertoires qui contiennent le fichier.  
**nano example.txt :** Ouvre le fichier example.txt dans “Nano”, l’éditeur de texte de linux.  
**poweroff :** Arrêt immédiat du raspberry PI.  
**raspi-config :** Ouvre le menu des paramètres de configuration.  
**reboot :** Pour rebooter immédiatement le Raspberry PI.  
**shutdown -h now :** Pour éteindre immédiatement le Raspberry PI.  
**shutdown -h 01:22 :** Pour éteindre le Raspberry PI à 1:22 AM.  
**startx :** Ouvrir l’interface graphique GUI (Graphical User Interface).  
## Commande sur fichier et répèrtoire:  
**cat exemple.txt :** Affiche le contenu du fichier exemple.txt.  
**cd /abc/xyz :** Change de répertoire courant pour le répertoire /abc/xyz.  
**cp XXX :** Copie le fichier ou le répertoire XXX et le colle à un emplacement spécifique. Par exemple: cp exemplefile.txt /home/pi/office/ copie exemplefile.txt du répertoire courant et le colle dans le répertoire /home/pi/ directory. Si le fichier n’est pas présent dans le répertoire courant, vous pouvez ajouter son chemin en préfixe (par exemple : cp /home/pi/documents/examplefile.txt /home/pi/office/ copie le fichier du répertoire documents dans le répertoire office).  
**ls -l :** Liste tous les fichiers du répertoire en cours, ainsi que la taille du fichier, la date de modification et les autorisations.  
**mkdir exemple_directory :** Créer dans le répertoire courant un nouveau répertoire exemple_directory.  
**mv XXX :** Déplace un fichier ou un répertoire nomé XXX à un emplacement spécifique.Par exemple, mv exemplefile.txt /home/pi/office/ déplace exemplefile.txt dans le répertoire /home/pi/office. Si le fichier n’est pas présent dans le répertoire courant, vous pouvez ajouter son chemin en préfixe (par exemple :. cp /home/pi/documents/exemplefile.txt /home/pi/office/ déplace le fichier du répertoire documents dans le répertoire office). Cette commande peut aussi être utilisé pour renommer des fichier (mais seulement dans le même répertoire). par exemple, mv examplefile.txt newfile.txt renomme examplefile.txt en newfile.txt, et conserve le fichier dans le même répertoire.  
**rm example.txt :** Effacer le fichier example.txt.  
**rmdir example_directory :** Effacer le répertoire example_directory (seulement si il est vide).  
**scp user@10.0.0.32 :/some/path/file.txt :** Copier un fichier à travers SSH. Peut être utilisé pour télécharger un fichier à partir d’un ordinateur de bureau / ordinateur portable sur le Raspberry Pi. user@10.0.0.32 est le nom d’ utilisateur et l’adresse IP locale du bureau / ordinateur portable et /some/path/file.txt est le chemin d’accès et le nom du fichier sur le bureau / ordinateur portable.  
**touch :** Crée un nouveau fichier vide dans le répertoire courant.  
## Commande réseau internet:  
**ifconfig :** Pour vérifier l’état de la connexion réseau que vous utilisez (pour voir si wlan0 dispose d’ une adresse IP par exemple).  
**iwconfig :** Pour vérifier quel réseau l’adaptateur sans fil utilise par exemple.  
**iwlist wlan0 scan :** Affiche une liste des réseaux sans fil actuellement disponibles sur wlan0.  
**iwlist wlan0 scan | grep ESSID :** Utilisez grep avec le nom d’un champ pour répertorier uniquement les champs dont vous avez besoin (par exemple, pour lister les ESSID uniquement).  
**nmap :** Analyse votre réseau et répertorie les périphériques connectés, le numéro de port, le protocole, le système d’exploitation, l’état (ouvert ou fermé), les adresses MAC et d’autres informations.  
**ping :** Teste la connectivité entre deux périphériques connectés sur un réseau. Par exemple, ping 10.0.0.32 envoie un paquet à l’appareil à IP 10.0.0.32 et attend une réponse. Il fonctionne également avec les adresses de sites Web.  
**wget http://www.website.com/example.txt :** Télécharge le fichier example.txt depuis le Web et l’enregistre dans le répertoire courant.  
## Commande information système:  
**cat /proc/meminfo :** Affiche des détails sur votre mémoire.  
**cat /proc/partitions :** Affiche la taille et le nombre de partitions sur votre carte SD ou votre disque dur.  
**cat /proc/version :** Affiche la version de la Rasperry Pi que vous utilisez.  
**df -h :** Affiche des informations sur l’espace disque disponible.  
**df / :** Indique la quantité d’espace disque disponible.  
**dpkg –get-selections | grep XXX :** Affiche tous les packages installés qui sont liés à XXX.  
**dpkg –get-selections :** Affiche tous les paquets installés.  
**free :** Indique la quantité de mémoire libre disponible.  
**hostname -I :** Affiche l’adresse IP de votre Raspberry Pi.  
**lsusb :** Liste tous les périphériques USB connectés à votre Raspberry Pi.  
Touche HAUT : En appuyant sur la touche HAUT, vous entrez la dernière commande entrée dans l’invite de commande. C’est un moyen rapide de corriger les commandes qui ont été faites par erreur.  
**vcgencmd measure_temp :**Affiche la température de la CPU.  
**vcgencmd get_mem arm && vcgencmd get_mem gpu :** Affiche la mémoire divisée entre le processeur et le GPU.  
