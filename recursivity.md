# Récursivité terminale
Un seul appel récursif est effectué par fonction.
```java
int sommeTerminale(int n, int accum) {
    if (n == 0) {
        return accum;
    } else {
        return sommeTerminale(n - 1, accum + n);
    }
}
```

# Récursivité linéaire
Une fonction et un calcul sont effectués par appel récursif.
```java
int sommeLineaire(int n) {
    if (n == 0) {
        return 0;
    } else {
        return n + sommeLineaire(n - 1);
    }
}
```

# Récursivité exponentielle
Deux appels récursifs sont effectués par fonction.
```java
int fibonacci(int n) {
    if (n <= 1) {
        return n;
    } else {
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
}
```

---------------------------------------
# Récursivité simple
La récursivité simple se produit lorsqu'une fonction s'appelle elle-même une seule fois, directement, dans son corps.
```java
int factorielle(int n) {
    if (n == 0) {
        return 1;
    } else {
        return n * factorielle(n - 1);
    }
}
```

# Récursivité multiple
La récursivité multiple se produit lorsqu'une fonction s'appelle elle-même plusieurs fois au cours d'une seule exécution. Chaque appel peut générer d'autres appels récursifs, ce qui peut entraîner une croissance rapide du nombre d'appels.
```java
int fibonacci(int n) {
    if (n <= 1) {
        return n;
    } else {
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
}
```

# Récursivité croisée
La récursivité croisée se produit lorsqu'une fonction A appelle une autre fonction B, et que cette fonction B appelle de nouveau la fonction A. C'est un échange récursif entre deux ou plusieurs fonctions.
```java
int pair(int n) {
    if (n == 0) {
        return 1;
    } else {
        return impair(n - 1);
    }
}

int impair(int n) {
    if (n == 0) {
        return 0;
    } else {
        return pair(n - 1);
    }
}
```

# Récursivité imbriquée
La récursivité imbriquée se produit lorsqu'une fonction appelle elle-même de manière récursive, mais cet appel récursif est lui-même placé dans un appel récursif. Autrement dit, une fonction s'appelle récursivement à l'intérieur d'un autre appel récursif.
```java
int fonctionImbriquee(int n) {
    if (n <= 1) {
        return n;
    } else {
        return fonctionImbriquee(fonctionImbriquee(n - 1));
    }
}
```
