# Présentation de Kali Linux Live boot 

## Qu'est-ce que c'est Kali Linux en Live boot ?
Une session __Kali Linux__ en Live boot consiste à utilisé Kali Linux depuis une clé USB transportable

### Points positifs: 
- Transportable est bootable sur tout les PC d'on le BIOS n'est pas vérrouillez ( très utile pour l'attaque `Chntpw` ) 

- Installation très simple et rapide

- Utilisation total de Kali Linux avec une dizaines d'outils de hacking assez puissant préinstaller 
### Points négatifs:
- Perte de toute l'activité réaliser à chaque extinction de l'ordinateur 

- clavier en qwerty par défaut ( peut être mit en azerty avec la commande `setxkbmap fr` mais doit être fait à chaque nouvelle connexion 

- Pas de clé usb -> Pas de Kali Linux en session Live boot 

- La clé USB servira seulement à être sur Kali, tout le contenu qui étaient dedans seront définitivement supprimées ( sauvegardez les éléments important ailleurs avant k'installation )

- La clé USB peut se perdre facilement

## Configuration du BIOS pour être sur qu'il est possible de boot via une clé usb
1. Redémarrez votre pc et DÈS que quelque chose apparaît à l'écran ( souvent la marque du PC ) appuyez sur la touche qui vous permet d'accèdez à vôtre BIOS, faites une recherche google rapide pour connaître quelle est cette touche sur votre ordinateur car ce n'est pas la même selon les marques/modèlles
2. Cherchez un onglet comme 'Sécurité'  'Advances' ou même 'Boot' 
3. Une fois dessus désactiver/disable la sécurité au boot si ce n'est pas déjà fait ( Secure Boot: Disable ) 

## Installation 

1. Rendez-vous sur le site officiel de Kali Linux -> Download -> Live Boot ( Lien qui mène directement à la fin du chemin: https://www.kali.org/get-kali/#kali-live ) 
2. Téléchargez l'ISO du milieu
3. Rendez-vous sur le site officiel de Rufus
4. Descendez légèrement et téléchargez la version type portable
-__CETTE ÉTAPE ENTRAINERA LA SUPPRESSION DÉFINITIVE DU CONTENU DE VOTRE CLÉ USB, SOYEZ SUR DE NE RIEN AVOIR D'IMPORTANT DESSUS AVANT DE CONTINUER !__ 
5. Ouvrez Rufus, branchez votre clé usb sur votre ordinateur et complétez comme ceci: 
``` Péripherique: Votre Clé USB 
Type de démarrage: Selection -> Cherchez votre ISO Kali Linux et mettez le 
Schéma de partition: GPT
Système de destination: UEFI (non CSM)
Nom du volume: Clé Live Kali
Système de fichiers: NTFS
Taille d'unité d'allocation: Laissez par défaut
Démarrez
Oui a tout ```

**INSTALLATION TERMINÉE**

## Démarrez Kali Linux live boot 

1. Redémarrez vôtre PC et DÈS que quelques chose apparaît, appuyez sur la touche de selection de système d'exploitation de démarrage 
2. Sélectionnez vôtre clé Kali Linux et faites ENTRÉE 
3. Choisissez `Live (amd64)` et faites ENTRÉE 

**VOUS ÊTES SUR VÔTRE SESSION LIVE KALI**

### Pétites aides pour facilité vos utilisation 

À partir de votre terminal, vous pouvez mettre votre clavier en azerty en entrant `setxkbmap fr` 

Si votre session se vérrouille pour inactivité, le mot de passe est `kali`
