# Imports
```py
from random import *
print(random())
```
Importe toutes les fonctions du modules random

```py
import random

print(random.random())
```
Importe le module random
```py
from random import random
print(random())
```
importe uniquement la fonction randint du module random

⚠️Il est déconseillé d'utiliser `import *` car en plus de charger inutilement la mémoire (avec les fonctions qui ne seront pas utilisées) peut générer des des conflits avec plusieurs fonctions ayant le meme nom.⚠️

Par exemple:
```py
from random import *
def random(a,b):
    return randint(a,b)
```
ici la fonction random du module random à été écrasé par la fonction random
