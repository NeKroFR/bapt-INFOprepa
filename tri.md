# Tri insertion  Θ(n²)
pseudo code:
```
procédure tri_insertion(tableau T)
  
       pour i de 1 à taille(T) - 1

            # mémoriser T[i] dans x
            x ← T[i]                            

            # décaler les éléments T[0]..T[i-1] qui sont plus grands que x, en partant de T[i-1]
            j ← i                               
            tant que j > 0 et T[j - 1] > x
                     T[j] ← T[j - 1]
                     j ← j - 1

            # placer x dans le "trou" laissé par le décalage
            T[j] ← x                            

```

# Tri selection Θ(n²)
pseudo code:
```
procédure tri_selection(tableau t)
      n ← longueur(t) 
      pour i de 0 à n - 2
          min ← i       
          pour j de i + 1 à n - 1
              si t[j] < t[min], alors min ← j
          fin pour
          si min ≠ i, alors échanger t[i] et t[min]
      fin pour
  fin procédure
```

Le tri par insertion a un meilleur comportement que le tri par sélection lorsque le tableau est presque trié donc entre les deux il vaut mieux choisir le tri insertion