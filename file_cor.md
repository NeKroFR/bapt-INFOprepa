# La file correction
```py
class FileDynamique:
    def __init__(self):
        """ Instancie une file vide """
        self.F = []

    def enfiler(self, element):
        """ Enfile un élément en queue de file """
        self.F.append(element)

    def defiler(self):
        """ Défile ( si la file n'est pas vide ! ) un élément en tête de file, et le renvoie """
        if self.estVide():
            return "File vide !"
        v = self.F[0]
        self.F.pop(0)
        return v

    def estVide(self):
        """ Renvoie True si la file est vide, False sinon """
        return self.F == []


#tests
F = FileDynamique()
print(F.estVide())
F.enfiler(12)
F.enfiler(13)
print(F.estVide())
print(F.defiler())
print(F.defiler())
print(F.defiler())
```