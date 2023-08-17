# La pile correction
```py
class PileDynamique():
    def __init__(self):
        """
        création d'une pile vide.
        """
        self.P = []

    def est_vide(self):
        """
        savoir si la pile est vide ( méthode est_vide() ). La question est : comment repérer le niveau auquel correspond le sommet de la pile ?
        """
        return len(self.P) == 0 # ou self.P = []

    def empiler(self, element):
        """
        empilage d'un élément ( méthode empiler() ).
		"""
        self.P.append(element)

    def depiler(self):
        """
        dépilage d'un élément ( méthode depiler() ). La méthode devra bien entendu au préalable vérifier que la pile n'est pas vide ! Elle devra de plus renvoyer l'élément dépilé.
        """
        if self.est_vide():
            return "Pile vide !"
        v = self.P[-1]
        self.P.pop()
        return v

# tests
P = PileDynamique()
print(P.est_vide())
P.empiler(12)
P.empiler(13)
print(P.est_vide())
print(P.depiler())
print(P.depiler())
print(P.depiler())
```