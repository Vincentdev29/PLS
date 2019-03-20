# Java

Source [openclassrooms](https://openclassrooms.com/fr/courses/26832-apprenez-a-programmer-en-java)

## Sommaire

## Partie 1 - Bien commencer Java

### Variable et opérateur

#### Type de variable

```java
<Type> <Nom de variable>

byte  // 1 octet
short // 2 octets
int   // 4 octets
long anneeLumiere; // 8 octets
anneeLumiere = 9460700000000000L; // 'L' pour spécifier le type sinon variable alloué en type entier
float pi; // 4 octets
pi = 3.141592653f; // 'f' pour alloué en type float et '.' pour représenter la virgule
double division; // 8 octets
division = 0.3333333333334d; // 'd' pour typer la variable, contient plus de chiffre après la virgule comparé à float

char caractere; // Contient un caractère
caractere = 'A';

boolean question; // Contient un type booléen
question = true;

String chaine = "une chaine"; // Déclare un objet de type String/chaine de caractère
```

#### Les opérateurs arithmétiques

```java
int nbre1, nbre2, nbre3;  //Déclaration des variables

nbre1 = 1 + 3;            //nbre1 vaut 4
nbre2 = 2 * 6;            //nbre2 vaut 12
nbre3 = nbre2 / nbre1;    //nbre3 vaut 3
nbre1 = 5 % 2;            //nbre1 vaut 1, car 5 = 2 * 2 + 1
nbre2 = 99 % 8;           //nbre2 vaut 3, car 99 = 8 * 12 + 3
nbre3 = 6 % 3;            //là, nbre3 vaut 0, car il n'y a pas de reste

// Affectation particulière de variable s'applique aussi aux autres opérateurs
nbre1 = nbre1 + 1;
nbre1 += 1;
nbre1++;
++nbre1;

int k = (int)3/4 // Convertit en type entier le résultat de la division euclidienne qui est un float
// Les opérations sont soumises à une priorité.
```

```java
String chaine =
System.out.println("Imprime dans " + chaine);
```

### Lire les entrées clavier

#### La classe scanner

```java
import java.util.Scanner;

Scanner sc = new Scanner(System.in);
String str = sc.nextLine(); // Récupère l'entrée clavier via la console en type string
int entier = sc.nextInt(); // Récupère l'entrée clavier en type entier
// Existe aussi en d'autre type
```

### Les conditions

#### Structure if... else

**Opérateur logique**
* == : égalité

* != l’inégalité.

* < strictement inférieur

* <= inférieur ou égal

* > strictement supérieur

* >= supérieur ou égal

* && ET

* || OU

* ? : » : l'opérateur ternaire

* !(opération logique) :  négation de l'opération logique

```java
if(condition){
  // Code
}else { // else if(condition)

}
```

#### Structure switch
```java
switch (/*Variable*/){
  case /*Argument*/:
    /*Action*/;
    break;

  default:
    /*Action*/;
}
```

#### Condition ternaire

```java
int x = 10, y = 20;

int max = (x < y) ? y : x ; //Maintenant, max vaut 20
```

Décortiquons ce qu'il se passe :

    Ce qui se trouve entre les parenthèses est évalué : x est-il plus petit que y ? Donc, deux cas de figure se profilent à l'horizon :

        si la condition renvoie true (vrai), qu'elle est vérifiée, la valeur qui se trouve après le ? sera affectée ;

        sinon, la valeur se trouvant après le symbole: sera affectée.

### Les boucles

#### While
```java
while (/* Condition */)
{
  //Instructions à répéter
}
```

#### Do while
Exécution de la boucle minimum une fois
```java
do{
  //Instructions
}while(a < b);
```

#### For
```java
for(int i = 1; i <= 10; i++)
{
  System.out.println("Index numero : " + i;
}

// Exemple avec plusieurs incrément
for(int i = 0, j = 2; (i < 10 && j < 6); i++, j+=2)

// Parcours de tableau
for(<Type> <nomValeur> : <nomTableau>){}
```

### Les tableaux

#### Tableau a une dimension
```java
// Format
<type du tableau> <nom du tableau> [] = { <contenu du tableau>};

// Différente déclaration
int tableauEntier[] = new int[6];
int[] tableauEntier2 = new int[6];
```

#### Tableaux multidimensionnels
```java
int premiersNombres[][] = { {0,2,4,6,8},{1,3,5,7,9} };
```

#### Pointer un index dans un tableau
```java
tableau[0]; // Pointe sur l'index 0
tableau[0][1]; // Pointe sur l'index 0 de la dimension de premier niveau et sur l'index 1 de cette dimension
```

### LEs méthodes de classe

#### Méthodes utiles

**Chaines de caractères**
```java
toLowerCase() // Convertit en minuscule
toUpperCase() // Convertit en majuscule
length() // Retourne la longueur de la chaine
equals() // Vérifie  si deux chainse sont égales
charAt(<index chaine>) // Retourne le caractère de la chaine à l'index indiqué. L'index commence à 0.
substring(<index caractère début inclus>, <index caractère fin exlus>) // Extraction d'une partie de la chaine de caractère. L'index commence à 0.
indexOf(<chaine de caractère>) // Retourne l'index où se trouve la première occurence de la chaine en paramètre
lastIndexOf(<Chaine de caractère>) // Même résultat que précédement en partant de la définisse
```

#### Création de sa propre méthode
Exemple de méthodes
```java
public void function(){} // Le type void ne retourne pas de donnée

public void function(int i, int j, Strin chaine){} // Une méthode peut inclure un ou plusieurs paramètres de différent type

public int function(){ // Une méthode peut être typé autre que void, elle doit alors retourner une valeur du même type
  return 1;
}
```

#### Surcharge de méthode
C'est le fait d'avoir plusieurs méthodes portant le même typage et nom mais qui ne prend pas les même types ou nombre de paramètres. La surchage peut aussi s'appliquer au constructeur de classe.
```java
public void imprimmerChaine(String string){
  System.out.println(string);
}

public void imprimmerChaine(int entier){
  System.out.println(entier.toString());
}
```
