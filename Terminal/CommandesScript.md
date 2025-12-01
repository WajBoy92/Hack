#! /bin/bash : A mettre dans la premiere ligne de code d'un fichier pour le definir comme étant un script bash

echo texte : Affiche texte (= print() en python)
echo " Une phrase " : Utilisée des guillement simple ou double pour afficher un texte plus ou moins long 

x= 5 : Creer la variable x qui a pour texte 5
x=" Long variable " : Creer la variable x qui contient un texte plus long 

$x = appelle la variable x 

read x : L'utilisateur ecrira ce qu'il veut et son résultat sera stocké dans la variable x ( = input en python )

read -p "Texte : " x : Affiche un texte avant que l'utilisateur écrit une ce qui sera stocké dans la variable x ( Utile pour poser une question et attendre une reponse directement sans passé par un echo avant ) 
wait : attend que la commande finisse de s'exécuter avant de continuer le script 

timeout 60 [Commande] : Tue la commande sous 60 secondes si elle n'est paz fini 

while true ; do : Creer une boucle qui exécutera infiniment du code

break : Quitte une boucle 

[Commande] 2>/dev/null : Realise la commande dans un "trou noir", pour pas pollué le terminal de l'itilisateur 

if [Condition]; then : execute du code si la condition est vrai, peut contenir un else dans la meme colonne du if, ne pas oublier de mettre une indentation pour le code et obligatoirement finir un boucle if avec un fi 

sleep 60 : attend 60 secondes avant d'exécuter le reste du script 

##Stucture de la commande case 
read x
case "$x" in 
    [1] )
        Code
    [2] )
        Code
    *) (si tout etait faux, comme un else ) 
        Code
si x contient 1 alors le premier bloc s'excecutera, si il contient 2 le 2e s'excecutera, si il ne contient aucun d'entre eux alors le bloc *) s'excecutera 
C'est comme des if mais avec des vérifications plus precise 
##


