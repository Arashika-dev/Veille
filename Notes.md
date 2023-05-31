# Programmation impérative et procédurale

## Programmation impérative
Les « langages impératifs » sont les plus répandus parmi l’ensemble des langages de programmation et sont ceux qui sont les plus proches du fonctionnement des processeurs : exécuter une suite d’instructions élémentaires. Le programme est executé de haut en bas sans retour en arrière, si on veut réutilisé un bout de code, on doit l'écrire une nouvelle fois.

``` python
def calculer_somme(liste):
    somme = 0
    for element in liste:
        somme += element
    return somme

ma_liste = [1, 2, 3, 4, 5]
resultat = calculer_somme(ma_liste)
print(resultat)  # Affiche 15
```

Dans cet exemple, nous utilisons une boucle for pour parcourir chaque élément de la liste et ajouter sa valeur à la variable somme.

## Programmation procédurale
La programmation procédurale est un paradigme de programmation qui se concentre sur la division d'un programme en petites procédures ou fonctions. Chaque procédure accomplit une tâche spécifique et peut être appelée et exécutée à partir de différents endroits dans le programme. Cela permet de rendre le code plus modulaire, plus facile à comprendre et à maintenir.

``` c
#include <stdio.h>

int calculer_somme(int tableau[], int taille) {
    int somme = 0;
    for (int i = 0; i < taille; i++) {
        somme += tableau[i];
    }
    return somme;
}

int main() {
    int mon_tableau[] = {1, 2, 3, 4, 5};
    int resultat = calculer_somme(mon_tableau, 5);
    printf("%d\n", resultat);  // Affiche 15
    return 0;
}
```

Dans cet exemple, nous définissons une fonction calculer_somme qui prend un tableau et sa taille en arguments. La fonction parcourt ensuite chaque élément du tableau et ajoute sa valeur à la variable somme. Ensuite, dans la fonction main, nous créons un tableau et appelons la fonction calculer_somme en passant le tableau et sa taille.



## Différences ?
La principale différence entre la programmation **impérative** et la programmation **procédurale** réside dans leur approche de structuration du code. En programmation **impérative**, le code est structuré en séquences d'instructions précises qui décrivent comment les tâches doivent être effectuées. Il se concentre sur le contrôle du flux d'exécution et la manipulation des données.
En revanche, en programmation **procédurale**, le code est structuré en procédures ou fonctions, qui sont des blocs de code regroupés ensemble et nommés. Chaque procédure accomplit une tâche spécifique et peut-être appelée de différents endroits dans le programme. La programmation procédurale favorise la modularité et la réutilisabilité du code en divisant le programme en petites parties gérables.

