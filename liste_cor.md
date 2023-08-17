# La liste chainé implémentation avec les noeuds correction
```py
class Noeud:
    def __init__(self, donnee):
        """
        Initialise un nœud avec une donnée spécifiée.
        
        Args:
            donnee: La donnée à stocker dans le nœud.
        """
        self.donnee = donnee
        self.suivant = None

class ListeChainee:
    def __init__(self):
        """
        Initialise une liste chaînée vide.
        """
        self.tete = None

    def ajouter(self, donnee):
        """
        Ajoute un élément à la fin de la liste chaînée.
        
        Args:
            donnee: La donnée à ajouter.
        """
        nouveau_noeud = Noeud(donnee)
        if not self.tete:
            self.tete = nouveau_noeud
        else:
            courant = self.tete
            while courant.suivant:
                courant = courant.suivant
            courant.suivant = nouveau_noeud

    def retirer_a_index(self, index):
        """
        Retire l'élément à l'index spécifié de la liste chaînée.
        
        Args:
            index: L'index de l'élément à retirer.
        """
        if index < 0 or index >= self.longueur():
            raise IndexError("Index hors de la plage valide")
        
        if index == 0:
            self.tete = self.tete.suivant
            return
        
        courant = self.tete
        for _ in range(index - 1):
            courant = courant.suivant
        courant.suivant = courant.suivant.suivant

    def longueur(self):
        """
        Calcule la longueur de la liste chaînée.
        
        Returns:
            int: La longueur de la liste.
        """
        courant = self.tete
        length = 0
        while courant:
            length += 1
            courant = courant.suivant
        return length

    def afficher(self):
        """
        Affiche les éléments de la liste chaînée.
        """
        courant = self.tete
        while courant:
            print(courant.donnee, end=" -> ")
            courant = courant.suivant
        print("None")

# Exemple d'utilisation
liste = ListeChainee()
liste.ajouter(10)
liste.ajouter(20)
liste.ajouter(30)

liste.afficher()
liste.retirer_a_index(1)
liste.afficher()
```