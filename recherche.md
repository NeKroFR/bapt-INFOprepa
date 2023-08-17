# Recherche dans une liste
```py
def recherche_val(L, val):
    """
    fonction qui renvoie True si la valeur est dans la liste
    """
    for v in L:
        if v == val:
            return True
    return False
```
# Recherche du maximum dans une liste de nombres
```py
def MAXIMUM(L):
    """
    fonction qui renvoie la valeur max d'une liste
    """
    maxi = L[0]
    for x in L:
        if x > maxi:
            maxi = x
    return maxi
```

# calcul de la moyenne et de la variance. 
```py
def Moyenne(L):
    """
    fonction qui renvoie la moyenne des valeurs d'une liste
    """
    somme = 0
    for v in L:
        somme += v
    return v/len(L)

def variance(L):
    """
    Fonction qui renvoie la variance des valeurs d'une liste
    """
    var = sum((x - Moyenne(L)) ** 2 for x in L) / len(L)
    return var

```