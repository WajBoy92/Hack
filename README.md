                                                 Outils de Hacking et Commandes Linux
                                                 
  ## À FAIRE TOUTE LES SEMAINES
  sudo apt update && sudo apt upgrade -> Met à jour la liste des paquets puis install les mises à jour 
  
  ## OUTILS DE HACKING
  __hydra__: BruteForce plusieurs système en ligne grâce à des wordlists _[ HowUseHydra à venir ]_
  
  __nmap__: Scanne une multitude de choses  
  
  __chntpw__: Modifie le fichier SAM windows pour effacer des mots de passe locals ou autres _[ HowUseCHNTPW à venir ]_
  
  __mimikatze__: Récupère des mots de passe local en clair ou hashé ( **souvent hashé** )
  
  __JohnTheRipper__ ou __john__: Casse des hash en BruteForce _[ HowUseJohnTheRipper à venir ]_
  
  __crunch__: Crée des wordlist personnalisable en fonction de nos besoins  
  
  __7-zip__: N'est pas un outils de hacking mais cette applications peut permettre d'envoyer des virus dans des zip sécurisés avec eds mots de passe par exemple sur discord 
  
  __wordlists__ ou __rockyou.txt__: Wordlist par défaut de Kali Linux
  
  __exiftool__: Analyse une image pour y donner les métadonnés
  
  __wireshark__: Puissant pour intercépeter des choses sur un Wi-Fi
  
  __zsteg__: Analyse une image et permet d'y donner les messages cachés  
  
  __aircrack-ng__: Analyse le trafic Wi-Fi, force la déconnexion des appareils, BruteForce le mdp Wi-Fi 
  
  __chrootkit__: Auto-Analyse son pc pour voir s'il y a des logiciel malveillant en cours
  
  __nikto__: Analyse un site, teste automatiquement des dizaines de milliers d'attaque pour nous dire qu'elles sont ses vulnérabilités

  
  ## NAVIGATION
  __cd__ : Se déplace dans un dossier
  
  __cd ..__ : Revient d'un dossier
  
  __cd__ ../.. : Revient de 2 dossier
  
  __cd/__ : Revient à la racine de l'OS

  __cd~__ : Revient à la racine de la session actuelle
  
  __ssh IP_DE_L'UTILISATEUR__ ou __ssh Nom_D'UTILISATEUR@IP_DE_L'UTILISATEUR__ : Se connecte en ssh à une session en route à condition d'avoir le mot de passe
  
  __su - NOM D'UTILISATEUR__: Se connecte au terminal d'une autre session disponible sur l'OS en question
  
  ## CRÉATION
  __mkdir NomDuDossier__: Crée un dossier

  __rm NomDuFichier__: Supprime le fichier
  
  __rm -r NomDeL'Élément__: Supprime l'élément
  
  __touch NomDuFichier__: Crée un fichier 
  
  __nano__: Crée un nouveau fichier puis permet d'écrire à l'intérieur, on modifie le nom du fichier en faisant Ctrl+O pour enregistrer le ficher sous.. et on quitte nano en fisant Ctrl+X 
  
  __nano NomDuFichier__: Écrit à l'intérieur d'un fichier déjà existant 
  
  __cp NOM_DU_FICHIER NOUVEAU_NOM__: Copie le fichier sous un autre nom  
  
  __zip -e__: Créer des dossiers zip avec mot de passe 

  ## ANALYSE
  __ls__: Liste les éléments disponible 
  
  __ls -l__: Liste + donne les détails ( date de création etc... ) 
  
  __ls -la__: Liste + détails + Éléments cachés
  
  __ls A*__: Liste les éléments qui commencent par A
  
  __lsblk__: Liste les partition 
  
  __fdisk -l__: Liste les partitions en donnant plus de détails 
  
  __cat__: Lit le contenu d'un fichier
  
  __grep__: Recherche quelque chose de précis dans un fichier ( Pareil que Ctrl+F )
  
  __nano Ctrl+W__: Recherche des éléments dans le fichier comme grep
  
  __find__: Trouve l'emplacement d'un fichier/Dossier sans être directement dans le bon dossier ( find . -name NomDuFichier/Dossier )
  
  __find . -name *.txt__: Recherche tout les fichier .txt à partir de la racine de l'OS 
  
  __df -h__: Voir l’espace disque
  
  __free -h__: Voir l’utilisation de la RAM
  
  __whoami__: Montre qui nous sommes actuellment dans le terminal 
  
  __ip a__: Donnes l'adresse IP de la machine qui utilise le terminal 
  
  __ping SITE_WEB__: Envoie un ping à un site puis attends de recevoir un "pong", si ça marche alors la machine à accès a internet ( exemple: ping google.fr ) 
  
  __wc NOM_DU_FICHIER__: Compte le nombre de mots que contient le fichier 
  
  __wc -l NOM_DU_FICHIER__: Compte le nombre de lignes que contient le fichier 


  ## GitHub
  __Git status__: Révèles si des modifications ont été faites et si il faut les monter ou non 
  
  __Git add Nom_Du_Dossier/Fichier__: Monter un Dossier/Fichier sur GitHub
  
  __Git commit -m "BLABLABLA"__: Fais un commentaire qui sera publié en même temps que les modifications
  
  __Git push__: Met les modification qu'on a réalisé à partir du terminal sur GitHub

  __git pull__: Met les modification qu'on a réalisé à partir de GitHub sur le terminal

  __git stash__: Met dans une corbeille se qu'on a modifié dans notre terminale mais cela peut être recupéré avec git stashpop

  __git stashpop__: Récupère les choses qui sont dans la corbeille GitHub
  
  __Git clone https://..__: Clone sur votre ordinateur un Dossier/Fichier/Code/Logiciel qui était sur GitHub

  __# Avant une ligne__ : Fait en sorte qu'une ligne soit un TITRE ( très gros ) un sous titre (##) ou alors un début de paragraphe (###), plus il y a de # et moins la ligne sera imposante (ces spécificité marche seulement sur des fichier.md)
  
  `__TEXTE__`: Les tirets du bas entre un texte le mettent en gras
  
   __- Avant une ligne__: Met une puce avant une lettre 

 ` Autour d'une ligne:  désactive la stylisation du code. Si on en met 3 autour d'une ligne on peut spécifié qu'elle sylisation de code nous voulons

 
 
 ## AUTRES
  __sudo__: SuperUserDO permet de dire au terminal qu'on a les permission pour effectuer notre commande ( mkdir test: Permission Denied | sudo mkdir test: OK ) 
  
  __sudo su__: Le terminal considèrera qu'on a les droits jusqu'à la fermeture de celui-ci ou si on quitte le mode avec " exit " ( mode root )
  
  __su - NOM D'UTILISATEUR__: Se connecte au terminal d'une autre session disponible sur l'OS en question 
  
  __COMMANDE1 &__: Lance la commande en arrière plan  
  
  __COMMANDE1 && COMMANDE2__: Execute la commande 2 si la commande 1 à fonctionnée
  
  __chmod__: Ajoute ou enlève des droits sur un fichier/dossier, exemple le droit de lecture/écriture/execution (chmod 777 donnes un accès complet au fichier/dossier )
  
  __mv fichier.txt /Dossier/HEY__: Déplace le fichier.txt dans /Dossier/HEY
  
  __mv X Y__: Renomme le dossier X par Y
  
  __cp fichier.txt /Dossier/HEY__: Déplace le fichier.txt dans /Dossier/HEY
  
  __cp X Y__: Copie le fichier X sous le nom de Y ( on a 2x le même fichier )
  
  __systemctl__: Gère les systèmes 
  
  __systemctl enable ssh__: Active le port 22 (SSH) 
  
  __systemctl start ssh__: Met en route le port 22 (SSH)
  
  __systemctl status ssh__: Regarde si le ssh est actif ou non 
  
  __ssh IP____DE____L'UTILISATEUR__ ou __ssh__ __Nom____D'UTILISATEUR@IP____DE____L'UTILISATEUR__: Se connecte en ssh à une session en route à distance à condition d'avoir le mot de passe
  
  __passwd__: Modifie le mot de passe de la session actuelle
  
  __passwd__ __NOM____D'UTILISATEUR__: Modifie le mot de passe de l'utilisateur local 
  
  __man__ __NOM____DE____L'OUTILS__ ou __NOM____DE____L'OUTILS__ __-h__ : Regarde le manuel de la commande pour comprendre ses variables ainsi que son utilité principal ( man -> manuel | -h -> help ) 
  
  __Ctrl+Z__: Arrête une commande
  
  __setxkbmap fr__: Met le clavier en AZERTY
  
  __shutdown__: Éteint l'ordinateur dans un délai de 1min ( s'annule avec shutdown -c )
  
  __shutdown now__: Éteint l'ordinateur 
  
  __reboot__: Redémarre l'ordinateur 
  
  __usermod -aG GROUPE UTILISATEUR__: Ajoute un utilisateur dans un groupe  
  
  __while true; do `[COMMANDE]`; done__: Répète la `COMMANDE` en boucle à l'infini extrèmement rapidement **ATTENTION VOTRE TERMINAL PEUT SATURÉ SELON LA COMMANDE**
  
  __while true; do `[COMMANDE]`; sleep1; done__: Répète la `COMMANDE` en boucle à l'infini mais sleep permet de dire un nombre de seconde entre chaque lancera, `sleep1 = 1 seconde`

__# SUIVIS D'UN TEXTE__: Permet de commenter, le texte est visible dans l'écriture d'un script mais il n'est pas prit en compte par le script, utile pour commenter une ligne de cmd 
