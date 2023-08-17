## Implémentation récursive:
```py
def recherche_dichotomique_recursive2(element, liste_triee):
   if len(liste_triee)==1 :
       return 0
   m = len(liste_triee)//2
   if liste_triee[m] == element :
       return m
   elif liste_triee[m] > element :
       return recherche_dichotomique_recursive2(element, liste_triee[:m])
   else :
       return m + recherche_dichotomique_recursive2(element, liste_triee[m:])
```