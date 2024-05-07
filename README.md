C-simple-sell
 Résumé :
 
      •     J’ai créé bibliothèque comme des « #include stdio.h » :
 
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <unistd.h>
#include <sys/wait.h>
 
Pour prescrire et définir le type de données qui peuvent être utilisés dans ce programme.
Et ainsi avoir une portabilité des programmes sur différente plateforme.
 
      •     J’ai défini un constant « max_size » pour que ce soit plus simple et plus lisible
 
      •     On as définis plusieurs fonctions :
Comme ( token ) pour découper une chaîne en argument afin de traiter les éléments individuels rendre plus flexibles notre programme.
 
W Puis on a créé la fonction « main »
 
Donc le « int argc » c’est le nombre de string que j’ai mis dans ma ligne de commande
Ensuite j’ai le « argv » qui représente mon tableau de string avec les « * » pour désigner un pointeur donc pointeur de pointeur
 
Path le chemin adsolue pour y allé
 
Et du coup si « if » donc mon « argc » est inférieure a 2 je rentre dans le « mode itératif »
C'est pour ça qu’après on voie le " mode interactif "
 
Donc on rentre dans le boucle « while » qui est une boucle infini qui va s’arrête si on demande un existe.
 
Apres j’ai le « fgets » qui prend on compte chaque ligne de caractère entré, et donc « fgets » va prendre en compte le « stdin » qui est dans le 2eme string pour le rajouté dans le « 1er string » qui est la chaîne de caractère et si il y a une erreur ça renvoi 0.
 
Strcspn est a peut prêt pareil que « fgets » il va allez dans le string pour cherche le symbole « \n » pour ensuite le rajouté dans le string dans la quel on lui donne une valeur de 0 et du coup ça fais le « break »
 
« snprintf » est un print qui au lieu d’être printé vers le « stdio » va me mettre un tableau qui va récupéré tout les printf que j’aurais stipulé, comme un concaténée si on veux  et qui permet d’avoir un chemin complet
 
Après j’ai mis un token qui sont juste les argument pour la commande pour délimité l’espace que je veux supprimer, pour avoir au final
 
Créer un processus enfant pour exécuter d’autre commande comme si on avait plusieurs fenêtre, comme j’ai le processuel « main » j’ai le processus fils qui fais les calcul avec le « pid=fork »  « fork »  me donne le « pid » du processue et du coup si je suis = a 0 le processus enfant marche  et donc va faire le programme.
 
     - Attendre que le processus enfant se termine pour que le père prend le relais. Sinon
NULL
 
Et donc le « non interactif » est presque pareil sans la boucle « while » c’est une exécution simple, on peut voir qu’il y a pas de boucle « while » qui est fais, la juste on garde des argument de « argc » on regarde pas la premier case de commande car on la connais et donc on commence directement a partir de la deuxième case mais l’exécution est pareil qu’avant    
.
 
5. **Terminer le programme avec un code de retour 0.**
