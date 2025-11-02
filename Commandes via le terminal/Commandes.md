# Commandes du terminal Linux (bash)
  
## NAVIGATION
  `cd <dossier>` : Se déplace dans un dossier
  
  `cd ..` : Revient d'un dossier
  
  `cd ../..` : Revient de 2 dossier
  
  `cd /` : Revient à la racine du système

  `cd ~` : Revient à la racine de la session actuelle
  
  `ssh <IP>` ou `ssh <UTILISATEUR@IP>` : Se connecte en ssh à une session en route à condition d'avoir le mot de passe
  
  `su - <UTILISATEUR>`: Se connecte au terminal d'une autre session disponible sur l'OS en question
  
## CRÉATION
  `mkdir <NomDossier>` : Crée un dossier

  `rm <NomFichier>` : Supprime le fichier
  
  `rmdir <NomDossier>`: Supprime un dossier seulement si il est vide 
  
  `rm -r NomDossier` : Supprime un dossier et son contenu 
  
  `touch NomDuFichier` : Crée un fichier 
  
  `nano` : Crée un nouveau fichier puis permet d'écrire à l'intérieur, on modifie le nom du fichier en faisant Ctrl+O pour enregistrer le ficher sous.. et on quitte nano en fisant Ctrl+X 
  
  `l3afpad` : Pareil que nano mais avec un meilleur interface 

  `nano NomFichier` : Écrit à l'intérieur d'un fichier déjà existant 
  
  `cp Fichier NouveauNom` : Copie le fichier sous un autre nom  
  
  `zip -e` : Crée des dossiers zip avec mot de passe 

  `sed s/Bonjour/Hello/d  FichierFrançais.txt > FichierAnglais.txt : Collera le contenu du fichier français mais changera tout les Bonjour en Hello dans un nouveau dossier fichier anglais 

  `ifconfig wlan0 [Nouvelle IP]` : Change son adresse IP 
## ANALYSE
  `ls` / `ls -l` / `ls -la` : Liste les fichiers (+ détails, + fichiers cachés)

  `ls A*` : Liste les éléments qui commencent par "A"
  
  `lsblk` : Liste les partition 
  
  `fdisk -l` : Liste les partitions en donnant plus de détails 
  
  `cat <Fichier>`: Lit le contenu d'un fichier
  
  `nl <Fichier>`: Lit le contenu d'un fichier en numérotant chaque ligne, il ne numérote pas les lignes vide ( number lines )

  `grep <MOT> <Fichier>`: Recherche un mot précis dans un fichier ( Pareil que Ctrl+F )
 
  `head` <Fichier>: Lit les premières lignes d'un fichier

  `head -20 <Fichier>`: Lit le 20 premières lignes d'un fichier
 
  `tail <Fichier>`: Lit les dernières lignes d'un fichier

  `tail -20 <Fichier>`: Lit les 20 dernières lignes d'un fichier

  `nano Ctrl+W`: Recherche des éléments dans le fichier comme grep
  
  `find`: Trouve l'emplacement d'un fichier/Dossier sans être directement dans le bon dossier ( find . -name NomDuFichier/Dossier )
  
  `find . -name *.txt` : Recherche tout les fichier .txt à partir de la racine de l'OS 

  `df -h` : Voir l’espace disque

  `free -h` : Voir l’utilisation de la RAM

  `whoami` : Montre qui nous sommes actuellment dans le terminal 

  `ip a` : Donne l'adresse IP de la machine qui utilise le terminal 
  
  `ifconfig` : Donne le MAC de votre session, son IP local et public, le netmask et d'autres information  

  `ping SITE_WEB` : Envoie un ping à un site puis attends de recevoir un "pong", si ça marche alors la machine à accès a internet ( exemple: ping google.fr ) 

  `wc NOM_DU_FICHIER` : Compte le nombre de mots que contient le fichier 

  `wc -l NOM_DU_FICHIER` : Compte le nombre de lignes que contient le fichier 

  `ps aux` : Liste les processus en cours

  `apt-cache NOM_DE_L'OUTILS` : Affiche si l'outils est installable avec apt install et affiche son utilité ( affiche aussi les outils ayant un nom similaire ) 
## GitHub
  `Git status` : Voir l'état du repo 

  `Git add .` ou `Git add Fichier` : Ajoute des Dossier ou Fichier

  `Git commit -m "BLABLABLA"` : Valide en laissant un commentaire

  `Git push` : Met les modification qu'on a réalisé à partir du terminal sur GitHub

  `git pull` : Met les modification qu'on a réalisé à partir de GitHub sur le terminal

  `git stash`/`git stashpop` : Sauvegarder/restaurer des changements temporaires 

  `git stashpop` : Récupère les choses qui sont dans la corbeille GitHub

  `Git clone URL` : Clone un dépôt

**Astuce Markdown :**
- `#` TITRE, `##` sous-titre, etc.
- `__texte__` : gras
- `-` : puce
- `` `code` `` : style code

## AUTRES
  `sudo` : SuperUserDO permet de dire au terminal qu'on a les permission pour effectuer notre commande ( mkdir test: Permission Denied | sudo mkdir test: OK ) 

  `sudo su` : Le terminal considèrera qu'on a les droits jusqu'à la fermeture de celui-ci ou si on quitte le mode avec " exit " ( mode root )

  `su - NOM D'UTILISATEUR` : Se connecte au terminal d'une autre session disponible sur l'OS en question 

  `COMMANDE1 &` : Lance la commande en arrière plan  

  `COMMANDE1 && COMMANDE2` : Execute la commande 2 si la commande 1 à fonctionnée

  `chmod` : Ajoute ou enlève des droits sur un fichier/dossier, exemple le droit de lecture/écriture/execution (`chmod 777` donnes un accès complet au fichier/dossier )

  `mv fichier.txt /Dossier/HEY` : Déplace le fichier.txt dans /Dossier/HEY

  `mv X Y` : Renomme le dossier X par Y

  `cp fichier.txt /Dossier/HEY` : Déplace le fichier.txt dans /Dossier/HEY

  `cp X Y` : Copie le fichier X sous le nom de Y ( on a 2x le même fichier )

  `systemctl` : Gère les systèmes 

  `systemctl enable ssh` : Active le port 22 (SSH) 

  `systemctl start ssh` : Met en route le port 22 (SSH)

  `systemctl status ssh` : Regarde si le ssh est actif ou non 

  `ssh IP_DE_L'UTILISATEUR` ou `ssh Nom_D'UTILISATEUR@IP_DE_L'UTILISATEUR` : Se connecte en ssh à une session en route à distance à condition d'avoir le mot de passe

  `passwd` : Modifie le mot de passe de la session actuelle

  `passwd NOM_D'UTILISATEUR` : Modifie le mot de passe de l'utilisateur local 

  `man NOM_DE_L'OUTILS` ou `NOM_DE_L'OUTILS -h` : Regarde le manuel de la commande pour comprendre ses variables ainsi que son utilité principal ( man -> manuel | -h -> help ) 

  `Ctrl+Z` : Arrête une commande

  `Ctrl+D` : Redonne accès à notre prompte

  `setxkbmap fr` : Met le clavier en AZERTY

  `shutdown` : Éteint l'ordinateur dans un délai de 1min ( s'annule avec `shutdown -c` )

  `shutdown now` : Éteint l'ordinateur 

  `reboot` : Redémarre l'ordinateur 
  
  `COMMANDE1 ; COMMANDE2` : La 2e commande sera lancée juste après la 1ere automatiquement

  ` COMMANDE1 && COMMANDE2` : La 2e commaned sera lancée uniquement si la 1ere à bien marcher  

  `usermod -aG GROUPE UTILISATEUR` : Ajoute un utilisateur dans un groupe  

  `while true; do [COMMANDE]; done` : Répète la `COMMANDE` en boucle à l'infini extrèmement rapidement **ATTENTION VOTRE TERMINAL PEUT SATURÉ SELON LA COMMANDE**

  `while true; do [COMMANDE]; sleep1; done` : Répète la `COMMANDE` en boucle à l'infini mais sleep permet de dire un nombre de seconde entre chaque lancera, `sleep1 = 1 seconde`

  `# SUIVIS D'UN TEXTE` : Permet de commenter, le texte est visible dans l'écriture d'un script mais il n'est pas prit en compte par le script, utile pour commenter une ligne de cmd 
