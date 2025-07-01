# John The Ripper 

## Description
John The Ripper est un outils de hacking à utilisé via le terminal qui permet de faire du brute-force sur un mot de passe hashé pour voir le mot de passe en clair. Il peut par exemple
brute-force un dossier zip avec demande de mot de passe 

## Condtition D'utilisation
- Avoir une session Kali Linux par n'importe quelle moyen ( Machine Virtuelle | Session Live avec Clé USB | Système d'exploitation entier )
- Avoir en sa possession le mot de passe hashé, john n'attaque pas les mots de passes sans avoir le hash
- Avoir une version récente de __John__ ```bash sudo apt update && sudo apt upgrade && sudo apt install john -y ```
- Avoir l'outil __zip__ ```bash sudo apt install zip -y ```
- Avoir une __wordlist__ ```bash sudo apt install wordlists ```
## Sommaire
1. Création d'un fichier qu'on va rangé dans un dossier zip et exigé un mot de passe pour y voir le contenu 
2. Attaque par Brute force du dossier zip

# 1 CRÉATION D'UN DOSSIER ZIP AVEC MOT DE PASSE + AJOUT D'UN FICHIER DEDANS 

Cet étape est très simple, pour ce faire ouvrez votre terminal et faites les commandes commandes : 

```bash
nano test.txt
 # Écrivez ce que vous souhaitez 
Ctrl+O
ENTRÉE
Ctrl+X
 # Vous venez de crée un fichier nommé test.txt et d'écrire à l'intérieur 
zip -e SERCRET.zip test.txt
 # La commande créera un dossier zip appelé SECRET dans lequel sera rangé le fichier déjà existant test.txt  
Enter password: azerty
Confirm password azerty
```
#### Qu'est-ce que ça a fait ?
- Vous venez de crée un dossier zip nommé __SECRET.zip__ dans lequel est rangé vôtre fichier __test.txt__
- Il est impossible de lire le contenu du zip sans mettre le mot de passe
- Les commandes `cat` et `nano` révèleront le contenu du fichié en hashé car le dossier est crypté
- Même si vous essayer de télécharger le zip et de l'ouvrir/l'extraire via l'interface graphique normal, il sera demandé un mot de passe 
- Le mot de passe qui permet l'ouverture du dossier est __azerty__

# 2 ATTAQUE PAR BRUTE-FORCE DU MOT DE PASSE HASHÉ QUI PROTÈGE LE DOSSIER ZIP 
Cet étape est aussi très simple, continuez sur un terminal contant vôtre dossier __SECRET.zip__ puis faites les commandes suivantes : 
```bash
zip2john SECRET.zip > hash.txt
 # John à crée un fichier nommé hash.txt et y a écrit le hash du mot de passe qui protège le dossier zip 
john --wordlists=/usr/share/wordlists/rockyou.txt
 # Lance une attaque par brute-force avec la wordlists rockyou.txt 
john --show hash.txt
 # Montre le mot de passe trouvé```
Vous pouvez essayer la commande `john hash.txt --incremental`, ça lancera une attaque par brute-force en essayant __absolument toutes__ les combinaisons possibles. Je ne recommendes pas cette approches car l'attaque est __très lente__ si le mot de passe est un minimum long, elle peut même prendre __plusierus jours__ pour un mot de passe __assez simple__ 

** Vous avez Réussi votre attaque avec JohnTheRipper ** 

#
Si vous avez besoin d'aide supplémentaire, je vous invite à vous renseigner sur internet/ChatGPT/Reddit, et au pire des cas vous pouvez me contactez via mon discord en __bio__ 
