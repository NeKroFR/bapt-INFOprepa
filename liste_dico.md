# Listes
```py
L = [] # Lste vide
L2 = [4, 5, 6]# Lste avec les valeurs 4,5,6

L.append(1)    # L = [1]
L.append(2)    # L = [1, 2]
L.append(4)    # L = [1, 2, 4]
L.append(3)    # L = [1, 2, 4, 3]
# Retire le dernier élément
L.pop()        # => 3 and L = [1, 2, 4]
# Ajoute à la fin de la liste
L.append(3)    # L = [1, 2, 4, 3].

# L[i] renvoie la valeur à l'index i de la liste (commence par 0)
L[0]   # => 1
# L[-1] dernier élément
L[-1]  # => 3

# Index en dehors de la liste -> erreur
L[4]  # IndexError
L[1:3]   # Return list from index 1 to 3 => [2, 4]
L[2:]    # Return list starting from index 2 => [4, 3]
L[:3]    # Return list from beginning until index 3  => [1, 2, 4]
L[::2]   # Return list selecting every second entry => [1, 4]
L[::-1]  # Return list in reverse order => [3, 4, 2, 1]
L.remove(2)  # L = [1, 3]
L.remove(2)  # ValueError car 2 n'est pas dans la liste
```
# Dictionnaire
```py
dico_vide = {}
dico = {"clé":"valeur"}
print(dico["clé"]) # renvoie "valeur"
dico["a"] = "b" # => dico = {"clé":"valeur","a":"b"}
#parcours par clé:
for clé in dico.keys():
    print(clé)
# 'clé' et 'a' vont être affichés
# parcours par valeur:
for val in dico.values():
    print(val)
# 'valeur' et 'b' vont être affichés
# parcourir les deux
for key, val in dico.items():
    print(key, val)
# "clé", "valeur"
# "a","b"
```
⚠️Les dictionnaires ne sont pas triés donc les éléments peuvent être affichés dans le désordre⚠️