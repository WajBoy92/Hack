Voici une version corrigée et formatée de votre fichier au format Markdown pour qu'il s'affiche correctement :

```markdown
# Commandes utiles en Bash

```bash
#! /bin/bash  # A mettre dans la première ligne de code d'un fichier pour le définir comme étant un script bash
```

### Commandes de base
- `echo texte` : Affiche le texte (équivalent à `print()` en Python).
- `echo "Une phrase"` : Utiliser des guillemets simples ou doubles pour afficher un texte plus ou moins long.

### Variables
- `x=5` : Crée une variable `x` avec la valeur `5`.
- `x="Long texte"` : Crée une variable `x` contenant une chaîne de caractères.
- `$x` : Appelle la variable `x`.

### Lecture d'entrée
- `read x` : Permet à l'utilisateur de saisir une entrée qui sera stockée dans `x` (équivalent à `input()` en Python).
- `read -p "Texte : " x` : Affiche un message avant que l'utilisateur entre une réponse, qui sera stockée dans `x`.  
  *Exemple : Utile pour poser une question à l'utilisateur sans utiliser `echo` avant.*

### Contrôle des commandes
- `wait` : Attend que la commande en cours d'exécution se termine avant de continuer le script.
- `timeout 60 [Commande]` : Interrompt la commande si elle dépasse 60 secondes.

### Boucles
- `while true; do` : Crée une boucle infinie.  
    - Utilisez `break` pour quitter la boucle.

### Gestion des erreurs
- `[Commande] 2>/dev/null` : Exécute une commande sans afficher les erreurs dans le terminal (redirection vers un "trou noir").

### Conditions `if`
- `if [Condition]; then` : Exécute du code si la condition est vraie.
    - Peut contenir un `else`, mais n'oubliez pas de terminer par `fi`.
    - Exemple :
      ```bash
      if [ $x -eq 1 ]; then
          echo "x vaut 1"
      else
          echo "x ne vaut pas 1"
      fi
      ```

### Délai
- `sleep 60` : Met le script en pause pendant 60 secondes.

---

## Structure de la commande `case`

- Exemple :
    ```bash
    read x
    case "$x" in
        [1] )
            # Code à exécuter si x vaut 1
            ;;
        [2] )
            # Code à exécuter si x vaut 2
            ;;
        *)
            # Code par défaut (équivalent à else)
            ;;
    esac
    ```

- Explication : 
  - Si `x` contient `1`, alors le premier bloc s'exécutera.
  - Si `x` contient `2`, le second bloc s'exécutera.
  - Si aucune condition n'est remplie, le bloc `*` s'exécutera.
  - Les structures `case` permettent des vérifications plus précises que des conditions `if`.

---

Copiez/collez cette version corrigée et formatée directement dans le fichier Markdown pour qu'il s'affiche correctement sur GitHub. 😊