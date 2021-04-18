# Devoir 2 CSI2532

## Q1: Normalisation

Considérez une relation avec le schéma R(A, B, C, D) et l'ensemble F des dépendances fonctionnelles:

```Bash
F = {
 AB → C,
 C → D,
 D → A
}
```

### a. Trouver toutes les clés candidates de R

Les clés candidates que j'ai obtenu sont: AB,DB,CB

### b. Indiquez toutes les violations de BCNF pour R et décomposez les relations en collections qui sont dans BCNF.

Les éléments suivants violent BCNF:

```
C -> D
D -> A
```
Pour être dans BCNF, voici les relations décomposées:
```
Relations will go here once I get them...
```

### c. Indiquez quelles dépendances, s'ils existent, qui ne sont pas conservées par la décomposition BCNF.

## Q2: Dépendances fonctionnelles

Une agence appelée InstantCover fournit du personnel à temps partiel / temporaire aux hôtels de toute l'Écosse. Le tableau suivant montre le temps inscrit par les personnels de l'agence travaillant dans deux hôtels.

NIN | contractNo | hoursPerWeek | eName | hotelNo | hotelLocation
----|------------|--------------|-------|---------|--------------
113567WD|C1024|16|John Smith|H25|Edinburgh
234111XA|C1024|24|Diane Hocine|H25|Edinburgh
712670YD|C1025|28|Sarah White|H4|Glasgow
113567WD|C1025|16|John Smith|H4|Glasgow

### a. Sur informations fournies, identifiez les quatre dépendances fonctionnelles décrites.

### b. Liste toutes les clés candidates.

### c. Normaliser la relation avec la troisième forme normale (3NF) montrer les relations résultantes.

## Q3: Langues pures

Considérez les relations suivantes:

```Bash
Sailors(sid, sname, rating, age)
Reserves(sid, bid, day)
Boat(bid, bname, bcolor)
```

Écrivez des expressions en algèbre relationnelle (RA), calcul relationnel tuple (TRC) ou calcul relationnel de domaine (DRC) comme indiqué pour les requêtes suivantes:

### a. (RA) Listez les couleurs des bateaux réservés par Albert.

[Question_a_images](Images/Q3_a.png)

### b. (RA) Listez les identifiants de tous les marins ayant une évaluation (rating) d'au moins 8 ou un bateau réservé 103.

### c. (TRC) Listez les noms et l'âge de tous les marins qui ont une évaluation inférieure à 3.

### d. (RDC) Listez les identifiants de tous les bateaux réservés le 2019-04-28.

### e. (RDC) Listez les couleurs de tous les bateaux réservés par le marin Lubber.

## Q4: RAID

Déclaration | Correspond à | Déclaration
------------|--------------|------------
1- Je peux utiliser une technique RAID niveau 0 car | | A - la tolérance aux pannes est importante pour mon application et je dois protéger mes données même si deux disques tombent en panne en même temps.
2- Je peux utiliser une technique RAID niveau 1 car | | B - Je n'inquiet pas de perdre les données. Mon objectif principal est de pouvoir lire et écrire à grande vitesse.
3- Je peux utiliser une technique RAID niveau 5 car | | C - J'ai 6 disques disponibles mais j'ai besoin de la capacité de 5 d'entre eux ce qui signifie que je ne peux pas gaspier l'espace qu'un seul disque pour assurer la redondance.
4- Je peux utiliser une technique RAID niveau 6 car | | D - Je n'ai que deux disques disponibles, ce qui représente plus du double de la capacité dont j'ai besoin pour mon application et je veut être capable de récupérer les données si nécessaire.
5- Je préfère utiliser une approche paritaire plutôt qu'une approche miroir car | | E - La tolérance aux pannes est importante pour mon application, mais je n'ai pas beaucoup d'espace disponible.

## Q5: Arbre B+

## Q6: Index Bitmap

## Q7: Hachage
