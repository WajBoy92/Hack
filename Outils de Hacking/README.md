# Qu'est-ce que le dossier Outils de Hacking ?

__Outils de Hacking__ est un dossier dans lequel il sera expliqué comment utilisé une multitude d'outils de hacking grâce au sous dossier __How To Use__

# Comment savoir si un outils de hacking est expliqué dans le dossier How To Use ?

Dans ce fichier, il y aura plusieurs outils de hacking intéressant, ils seront rangé par catégories.

À la fin de chaque ligne expliquant le fonctionnement d'un outil, il y aura soit écrit:

- `[How To Use DISPONIBLE]`: Alors vous pouvez lire le fichier qui explique comment utiliser l'outil en question en vous rendant sur le dossier __How To Use__ 
- `[How To Use à venir]`: Le fichier expliquant comment utiliser l'outils __arrivera prochainement__ et il est sûrement en cours de rédaction, d'ici maximum 2 semaine il sera disponible dans le dossier __How To Use__ 
- __Rien d'écrit__ : L'outil __ne sera pas__ dans __How To Use__ avant un bon moment

## Installation 

`apt-cache NOM_DE_L'OUTIL` : Affiche si l'outils est installable avec apt install et affiche son utilité ( affiche aussi les outils ayant un nom similaire )
`apt install/remove NOM_DE_L'outil` : Install/Désinstall l'outil de hacking
`apt-get install/remove NOM_DE_L'OUTIL` : Install/Désinstall l'outil de hacking déjà disponible dans le système local
`apt-get purge NOM_DE_L'OUTIL` : Supprime l'outil de hacker ET les fichiers de configuration de celui-ci 
## OUTILS DE HACKING

### Brute Force | Wordlists | Création de Wordlist
  __hydra__ : BruteForce plusieurs système en ligne grâce à des wordlists _[ HowToUse à venir ]_
  
  __JohnTheRipper__ ou __john__ : Casse des hash en BruteForce __[ HowToUse DISPONIBLE ]__
  
  __crunch__ : Crée des wordlist personnalisable en fonction de nos besoins 
  
  __wordlists__ ou __rockyou.txt__ : Wordlist par défaut de Kali Linux
  
  __aircrack-ng__ : Brute force le handshake ( Brute Force Wi-Fi )

### Analyse | Espionnage 
  __nmap__ : Scanne une multitude de choses et scanne aussi le réseaux Wi-Fi
  
  __wireshark__ : Puissant pour intercépeter des choses sur un Wi-Fi, Attaque Man-In-The-Middle 
  
  __exiftool__ : Analyse une image pour y donner les métadonnées 
  
  __zsteg__ : Analyse une image et permet d'y donner des éléments cachés
  
  __nikto__ : Analyse un site, teste automatiquement des dizaines de milliers d'attaque pour nous dire qu'elles sont ses vulnérabilités
  
  __chrootkit__ : Auto-Analyse son pc pour voir s'il y a des logiciel malveillant en cours
  
  __airodump-ng__ : Analyse les réseaux Wi-Fi à proximité, Analyse les appareils qui s'y connecte, Récupère le handshake lorsque quelqu'un se connecte au Wi-Fi sur écoute
 
### Wi-Fi
  __nmap__ : Scanne une multitude de choses et scanne aussi le réseaux Wi-Fi
  
  __wireshark__ : Puissant pour intercépeter des choses sur un Wi-Fi, Attaque Man-In-The-Middle
  
  __aircrack-ng__ : Brute force le handshake ( Brute Force Wi-Fi )
  
  __airodump-ng__ : Analyse les réseaux Wi-Fi à proximité, Analyse les appareils qui s'y connecte, Récupère le handshake lorsque quelqu'un se connecte au Wi-Fi sur écoute
  
  __airmon-ng__ : Active le mode moniteur sur votre PC ( Permet d'utilisé les outils comme __mdk4__ __airodump-ng__ )
  
  __aireplay-ng__ : Lance des attaques de désauthentification Wi-Fi
  
  __mdk4__ : Attaques de désauthentification Wi-Fi très puissante, création de faux Wi-Fi brouillant les pistes ( avis subjectif -> c'est mieux que __aireplay-ng__ )

### Autres
  __chntpw__ : Modifie le fichier SAM windows pour effacer des mots de passe local ou autres _[ HowToUse à venir ]_
  
  __mimikatze__ : Récupère des mots de passe local en clair ou hashé ( **souvent hashé** ) 
  
  __7-zip__ : N'est pas un outils de hacking mais cette applications peut permettre d'envoyer des virus dans des zip sécurisés avec mots de passe par exemple sur discord
  
  __msfconsole__ : Permet de crée des exploits selon la cible et de les executer 

  __msfvenome__ :
# 
Vous pouvez me contacter sur mon discord __en bio__ si vous avez besoin de plus d'explication ou si vous voulez me demander de commencer l'écriture d'un outil de hacking 

