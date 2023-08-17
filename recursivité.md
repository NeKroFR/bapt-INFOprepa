# Fonction non récursive
```py
def factorial(n):
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result
```
# Fonction récursive
```py
def factorial(n):
    if n == 1: # cas de base
        return 1
    else: # recurence
        return n * factorial(n - 1) 
```
⚠️Toujours s'assurer d'atteindre le cas de base⚠️
```py
def rebourd(n):
    if n == 0: 
        print("0\nBOOM") 
    else:
        print(n)
        return rebourd(n-1)
rebourd(5) #marche
rebourd(-1) #erreur
```
par exemple cette fonction ne l'atteind jamais si n<0 c'est une boucle infinie
## le code renvoie:
```
5
4
3
2
1
0
BOOM
-1
-2
-3
-4
-5
-6
-7
-8
-9
...
```
