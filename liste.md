# La liste chainé

En python les "list" sont en réalité des tableaux standards

![alt-text](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAX8AAACECAMAAABPuNs7AAAAjVBMVEX9/f3////8/Pz+/v7s7OyBgYH5+fmhoaHX19fp6enR0dGampqPj4+1tbXl5eX29vYAAADFxcV9fX3b29uSkpKJiYnNzc2wsLDg4OClpaXHx8dxcXG6urp3d3d/f39tbW1iYmI3NzdZWVkuLi5HR0dQUFBVVVVEREQpKSkaGhoiIiI+Pj4LCwstLS0kJCT7LoRdAAAXqElEQVR4nO1dC4OiOs8mba0gSEXuAgM6OrNz2fP/f96XFFRQwPHsnvX9dsjM7nAppTxN0yRtU4NxBvgPf4yJ/iAxo4acMya5BPyZKuDPEWcG/SAh+sBhokeQ0vgbfJnNZsVsoj9K63Wi+Z8ZMM+FsMREf5IsEZgkgPAfzBfAoSWG+PH34hjOx6M3b+QxfLM3P/4fvWwgj7te0Dr+8tfUJxxsE874G3VvMNGfIjbh/1Ca8H8s9eKPFgGv9VL6g0aZNhFq46wx0hjd5/oMbxu1IUEp6SKdSVZf0ckxMacjMjYY3XvoN/8v0TX+BJNSEvHTsKJZzLiUaB4Q5ISgBNRW8cfQadBwoCqShsTUUhsS+EcqfYbXGQdJl7jSqQ1FOcJjP/p/iS7xxyPV9NQEn7RiicgzsFJJaGp7jXwV5K0g8JGxEW4OCrt0Q9eTgYBj9WA9kVEBiw3VFOIuycZWWEVg5lMFHOma/62X3f7z8DJTZJRBtNKSBBYrYIobiKnmX0IYDTcusYo4cbZkriDxhC0Ka0mRjKEGo8ApsRa4AjqXlKOEeDvhf6Rr/JFVva2rlLIsBHixor/AzBVIblkC5ZAQrmJKCoRdMEUySSVKiUOMYgtNCk45oB2HQDNlqaBkTLkCawRvWxLQ5Mg/JvyPdIU/yhrwthaXsyL7WED0WRS7HyYg/pDus5eZoaqi/LAg3wsuXnNqCvF+vWPF52vpe1W2DwGyqsg+YwD7Z1l8FCrZFbtKyviwK9XyrSwP+wn/I/XpP7B5dkl8J2El/ZVrQPpG8sd7c91klQOopJphHSH+2xx5XB0CBYb6WGJXwFX+7kO15rDcCu+HCyorpQLh/oghfjMhWfkA69cJ/yMN4c+VXQTV3tislOT+SiD+s7eszF5ytS7mHwV4Hwjrs4dSiZm7gw3qIwblZWH4zwKqOUD0bKUVyqCgBLeYBds5LA8AS+xG+CR/zjSAv4D0mQQOyn8LIH/j0QqWP7Va9JQBzErwnl2w3nNUdlBfSlaees5BrSKwCP8UO+5nN37GW0XJDlgdWxtzA7ZYSRRLE/4n6sd/ayG+TrDb8+if0g4/PNSDQK0PduCo/G0evhagdtW8ePZQAVWOU2yFetrbxr5Kyx8R8b9cbF1Z7O31oeDBNgifbYgPqD3Zr4Hz8jLhf6Qe+wu1dB/P3cgUCakuUWShlPdRcJibyJdgbnyBnYJYLFAfQvkj/ShCrUctIikWESpH4ArUPBMF0owS5aKAinzLAuEDqp+mZ6pkCH80Jb5Z1fTwP1qqZFtpLykZwWSJad8Cw0NkYc5BOyDwDzkfdEqtN3FKoF0OvHmAUhqnP/U98rqyIfp2rolr/fPBw5Dse9XAFf6wcQInQHKIgjY5dC0I6UAn6Uuhb19dP97E62FgNyl6KHDm8L0mAFzjn+buCCWLwkpG7lvraOxpywstNxnOYFF8d/kPc78tDUggnM5Q8oMVwnH4DG8YKMvx/9YTodU60fm2iINv61xqkuQ07Tytnib8TeMsAtAMJpfl8QxTIf68GaXB7lKSb7M9aAOha7TSS9ZRaBjh30h4cojibdnpc9V6wr+NvzTIc3kk0oDa+NeNgLya5/w6+EtM0rrZxZ/mHOHjasJ/BH9pl+IEyQX+sKmyMju4nfza+BvMTYsh/kdTQ2zsOOlMuZvw7+DPId5u3TP+XfljKD9x5/sOA3fw57IKV0P4cwXx08b+EbGJ//vwpzEsyF+8rUsDYfWlLv+TcFc/zJaAwgoLXWifmoP40wgZUtbpcSf8T/jTuFZ0EObWotFGnfiy/8W+Ncw6FtMV/otB/LFWseXIwxIm/u+VPxLcNyd3fsxd3igxF/hjAzH/sSS05M8d+NNAM4f1y6T/GP3yx2BWmqbhm23BcZb0hf4jjZ8x6uyt+Qx34M8FMLGfMZjwv8Cf1/zPiD8h0vLnqEQysGbkbKNjbBXzF0nTIc7ZXeBv9OPfVCbzfq6TJGk7HL49/gak5hECThCLheJGI5HI2EX8ycFp6DUbkWV03TWsiz+TwoPWmUH4Q9O+GJTVusyCDv6z7+7/4Yh/W56Q1/h0yhr8Gwki26yvrxD+bXVeu6fPj2v8aR4LvRm1Ku2TaD1O/ofv7f/EPybIs0NetU+Q78FF+QONA19qJbVNqP8n0HXo8/aJQf6f+hmD/A/0284C8f/e/I/yx+84zDr+MyThnL1rff57x+168y9uJ/POqXGRxyR/IC1a7vkgDJyw46IP93bHYX9B9iFsXwvCzqkTFLvzeaifDzvJy46/6O+nS/wlU4k1SuKXbo/fdy3Bvjf+ehyXBnYfQt3e/jvQFf9jh2k8igX1moHvzf8GPAx9TfKb8z+tVHmcBk7GwvfW/7/X1z+eJvwfSxP+j6UJ/8fShP9jacL/sTTh/1ia8H8sTfg/lib8H0sT/o+lCf/H0oT/Y2nC/7E04f9YmvB/LE34P5Ym/B9LE/6PpQn/x9KE/2Npwv+xNOH/WLqefyWbTUg4RfY0JOjpQJezolh9t3uJAk5KfiOASb1i/nTGWLvK6wC6zYFedfm388MV/6vjHiSMKS4Z1PEF9CYNLaK4ARc50WIM1lqqNEBStifYcQmsHe6AHRfTS07Yq79+NlzP/NvjYkfgiq7zvoUuOvrwxSXkWay8WxGsKIru+UlaDNNa/67fWefPKTKE0ayV+XvpSv5IQ+X00bBYIv9xHY6YXQoVyD1+iT8m5SVFFh5HrI6TdcooqtrrH2Xq1+uPKEQWyLmr/nYBdMX/UiY/6ADyJ714RYKfcgrkfFypVa9ymddLW3hrEQtKqW0KrHWluds82yx4MdKkzkmf5+/n9Ah6GTXrbrAZQewoVd95IED/MfXIn+TZBBRCyYZz0w6SJHtPPRDzYKlXWoMZBAlEJviRGdgsCWwB4Fl5MJcSnlOQvh1sgC3M3InlwkmxLbHYsbEnWYrYyYHFn+uloNgnbuqkzHu2AhsrxJ8HMebuWbDwI3yKwkSXqcDG4oW2xY2/NWj9tf4JyfOCeG6+ZdHK80w/+yeN/G28eXqlmHvRapGbsAshXzle8R5uwjcXDm+p57xZ8BxDeths9gGEq3Tz8uxE1RbU3o7ilWWsdnn+M2Tp2ywWCH/6Gnu58lazKFglLM43WQGwiqB4j/Nsr+BgR+mPRGWzKP5MmPxL1wVc4881/3OY76W5Si0UA3sw1rs0tlcLlC7+Kna5UQWQf1LcVRfE1kOswKD/tilfhXH8tDLCtYT8VWFyMX+P4/gthTcP+PId1E+PtCm5irBlgPcDNaxnbBam5zy7hP+6RKG3EvFzik/NvXf88xGC/Dvhv+5/DS1/iP/3XCXh8xLSPTMOpbf0NoKEQOKglK8c5H/gycpS6gPxXyL+2Ca2sVqlee5FEGaMLRH/5NMKtx5eSvgKUc7fQFCgXGYIrDppEP5MvcbGi7NJny1YbaAo8MpK2a/0lBtvN/hmk/YTeDBS/w31xJ9MfnjCslA+GEqB88Ljd4l14AMo2spCKLC3UIWw/ATDWllgIf/vPgQKJp/k/6HQMa9mGQfEXyL/o8SiTd5g5UmK/6ywSim0zbagHRq8d1Q5t/FipWBO+C8gy7AQK+GvPAAhk/cl/iFN+HvIf9TP3RKpSvKC5VVVLUBUVQ5pVZUBoLlUXwtj2FRgJAehVLaAwzqrKg/YOgcrxJQezG0Gm7Vi7k4Ym5eqehK8ioBtdsDSfUGbA1jhrlqLqESVK/Nk+JLZpQs737DxNYrqE/NZC1iU+Ff1WNVsrEmw6/S0vk9Syxt+Rt7SdrvWOpE0fq1lXuGvpI4KQMHdsLSC9qugEG1AjE87vuA12m0E6shutBcMHu6XeEnHc5P0EF1CnZX2jqFNGAAspQPf0uYv+IwiOCm0BNnaoOPQGFwwMsa0VktaFikCQjGpH0bhxi7NClo6bwyF0UVNVsq+G2pkfR8Wt/+h8/p9gOtrXP2Kenzd/yodZ5JC51FoSdpsROv0nDbS0bEjJV3XQDIdexJLVeSggzmQUUy7k1DwJi51+AcpJVnFVJtSVwDUIYjpEqdLIHVASqnfI/U2P3iR0KANWakc2i1xZdWR66JvAX6zsP5q5b0mOWJQ06eP5NhkexEe2IBf81Fd278iWpgLJJN+TaIF/daHzXlz24yaY8/VYRw0Q+pMmN50R2/ZQ36EpH7omE2dV0RXIp2Tjyf1ZcrR3OBxZCJSmh/JYcSu4hIz32yXqUuYp997Q8qR+B5SRUMZ1uT3vdH/vfIH5kG+rCmP8d8yb0713zif7+jysv5PX8c7aQh6yyNW77qj43qSK6iOuSGhTOvnjw8sY/3/MedwfXxbfE6z3lAMb6X3XDpFoDsRF1Vdhn6K88q+vppXFrt027bg51GWXz/UynSXXt3Pl+UNzWA8oMWN+LfXwbhF2NMshTPCVthkQ9Xz0Jk2y56LuTcmV7l6GpcUtt9z0bHGygmLdDRLOeu7uh6Hn+WK+iOp+v1iN+J/6i3sznkZ3fiTp1TWDfxn4pSJ7mAN3i4MePHl4/jM8hb+7ZJp718rDB0n/K8e0vgPFlTj3zpXFz53euV1nmwcf84K6nNQq1G992/FH+Ztx8tF/LfzS8bwZ138dYQBHdvyXIZfx5+Up9+LP0n1btp/hb/BZ7IeVOrXfG/gT4pkq0y/Af/aPwrtAZ3fgD/m2XaI/wb8G9/t5Suvn7rF/0+k0wkHJVCfABrBn2kdz8+VxrC50ol/eGzyd8gfrrDXjJcmb33KGX925Lm78MfSuV7SCQPYwf+0y/0X5P85f8+2F1evhIscx/HXI7dPqIxwQbarFiWsO8Y+En9VB8i2Pt8TMgtl/aFd/qcYYrpkX+d/rmKk93nboUb4N2l5w8X34I9ZpfvV8iIObBt/1qhPiD8fGdFs4w+bwMs/lzrSWvuVx3KeDIkx/PWwxxPxr7ARIDc2tOSlTTKPEA7jr61edxt/WNqWNYwr/ueqGUu/p/8lTcjbAmsPQp7xZ0213IE/VwotvEMMrYHPLv+jhVp/wB3462Efe0e8237l8T4xZFPSYfyhwkKoNariGn/uh9piZe3pDKPxh6U6bDZbV6KN3Rf/2ThuDXCP/FdMildvAH/SYuqWdgf/M9pa8pC3zaAL+cMbcXEP/rQN1C6gcp6b7ln+wMkTNII/V5v12pwxpgzCH9wQbX2PLBp5KsaI/FeclUug+M9HLriMP+82cvse/KWCWQWqPXx/xh+NtkjUmz1/GX89gq+I/1s6Vgd/MJvO/j784elATN7H/2BKMG7LH2R2P1zl5Ooi+ZM4qHjMLO3AOTLLWPxhMHe7l/3ni9nscX2l//t2rcbcI38kmCsFHXu2Lf+pizS+hP+6xf9S7ZfGhfw3z/iHQh7l/1h40RP+nGx2axfqaGgt+b8+cW2hjurueP+Lok+lVZooG/VIzf+OwKwXpz54GH/qCbGtRD98moPV5f/mWf9f8D8TP/ILFjzpP+RhnH2V/9ctTubqNe5qlh3814qd8f+C/omJebRdu0nSnueErzzOLoPsFKfupv4pQXlFFtDeNyGK9FAYnIKgdsvZ1//qLdSw0sghOoi/LvBd8icJLyE44U8d+kz9G/xlEHUj93XwL6C++WX8UfkLZmGRhQi4avH/Cf/1SX+7ZX/VO6otwpKGRlCSI/7gz7+AP4HNadxKzwKE46UW/txP/wX/Y4sc4n/yZa//Df5kLclh/i+aLTq+iH/tyNXOHeyEjT78i1MQ5i/gTwMnINLKRvyNUPAb+Pc5rs7U9r+Jo0NqzP/Guv63vqC5bf+bfdy/6m7/W9dX2Pa/Bcc8v+x/I7P/ajCAnf1vmTwdrsfnSKLCr7RXGMSyCi2U/6P4G5DO0nlN+q8971DqHM4n9kes06RByAaj9pEQK+10Tj/N7wWlRXnKMa3CtE5b3sB/dy7j/PIQT3Zhej525qmtD9yR4JoMNpUuJJbCpvQpHrQBsF/tJs90H5wuZmowRzJ5actLPYcWa5NH2bpCVkT8j93KJf5ciuFhDdM3/fq3HuXws00zKGFdTUc8EyjAJxb4nN8/LOKb5umy75XJwtfJRqd+cpnUeSUD5TxnafrLWRLVp6BGojsySWM6OqHfP3xzLGnipMcEfjJcSKmlFFNKb2uJZyi+gyxViY2Noh//gXG7cxuEswjhsLHrVk/jg0No6VFt1MOYiFV/3vwsOzDrUugxT+PGsBKNtDFA27c3S6OzrZ6o6rFUgNHxXxpCpV/VM+xxQWZ4hOF6ZO5MWoXRI+KELFmWiICIs8I2YID/5dgQtHbz0ga0p/HoF4pPT9q8HCyFHgpHGZ+tPt3BvPnpDRCnetD41mQEpTj2advZ9Yg401VjGK3MZ34dMh/LKQdblQ78C3K5t2Fgg1zQ43l0IEuLNy8Y/nIy3rCUav4caWuNdCaSxuAVhTlg/xp8JASt3viCxsnrN+LHRCEHXccjrRr7X8OvZrO1R3uP6DjPF0lo/sOxxIaqyF3T8nsNfBuY2e5nWTZ6YDdXbnT6WS6qxq134X3s5ohVkzztP6vsFP/6Ks3R5IOoUQOpLgZrVBrKWISvq4q0/yY5sRhwK3Tq3u3+9Uf8lIiGZp2Y5upKY7j/xTIoQ7jxjAu0WvpHgU5OFipHNGvKOdyiyFDgQZSGcr7p7aU7T6Pws2O9a814eF1UEmdesIbQvFxucsqp0Trx/U8b+jQwRspJ9/xwE86hQP0buzP9NC1TYXBUwn9l/ZeeZkJqihqbHouQK8ZCG98ZXqn+fekhCMj1Nywp6paP2iTq00l4e/YNxwpYe8aYpCDSc26wnHwTy8vh/gvChGLnSuNGjjTzBgpUapFL2IXiNeR/u/k1Z9Lbh8A6VXoS1mCB8eutLIe6w/hC/hKBlRLG5CoJU5WRy1kOtKhOOWllTukxYzwpiepiiaUUFsjxtPTdVrVgN5bnIFeKykNpZgk+UKO/hD8qDCj+55kLI1HTsagmNhJyut6GShcF++CdxYxBjUq/2C8j3Q6+sC6AUwOVa1uNTwWRzM3yun+VapxRaGEUalXxjebMwK8Wen9YMcROv8b/hp7n45azpD1M3CG8nlZCC1TspYdtlXa2mGXlKBiCi+Y9plWiX35zyqZR9y6o+C3LHEaW0gBEuwS06sXkwGh5q4i0d+Ic0R2pU4C4pC+XqjbBetP8yvrfui/C95jFU+7q3Xr0XJdGLmrF04iq9Cz2v5o98EXlLMhikVrp1SsrycaTepZpUszvnHXJaXZnUMYWGSu1b0tPEyWPvtZMwQqf4GIz6fFvp8WCYZELbbbUIzKkMhEeWvuFpAzgFsP9lvXXKIaTNFunCa1rqY04vVcVqjtRZls07fPOHNFmVqZTzn0aBCU9Wm+WzXTbYMJZL8b7xx5ievBiWc08pecNaItRNjNL0ZSIUUaqu6YS0jRhcO3MjhTXzYBGVbTlovdwsYLK7G4u3fuhvwN/mhUNYHnzolgHqbewLCyQ62/SsJq75Py7G3+uJ/nKzbzIMEO/ZY/682Idsft3qSIJoDfgS9flLN5YjeGtLViRF5lWUO8qJ9eTXAEW86wMl5FoG/TWMis8qM3IUfot+PN6vi1H0125m9h2wqIoHDtdCL2Ye9Q86yepTWqa+q6EFwdZtqZtqsIZZhsJPen+7hwNvVO6bkJiM8cShs48RXKcglQ4LSu/0j2dc6RVgdRT43Nubj9l61lAOcahk82W9OlkUf8J/Omj9IpsfFvXs6NFx/1g1fseNj4EykgqN3GTxBXa4WKwq4AINwka/wYxJIloUFaip2T7Sd3T1+LtnjKSSs+16aOFLVeur2eO+y6527W7hv0R/P974vxYob8vyxaXPC7H/yf4/7U04f9YmvB/LE34P5Ym/B9LE/6PpQn/x9KE/2Npwv+xNOH/WJrwfyxN+D+WJvwfS8d52hRwbHE7eupEv5UYO/K/BLAXFE3lPPeRt2Zm8s4szdPx6M0beQzf7M2P/0cvG8jjrhe0jr/8NfUxcn3N/xzljycsMdEfJUs4Nf8j/nkxm+jP0tPTrHCJ/YHmZcNED6DjTMR6bmpn5Gx4GG10gG189O3mo78wHPgvH/3FrxmeeXnz8XMciYkeSP8HHJF2DJxtw1EAAAAASUVORK5CYII=)

![Alt text](image-2.png)
[plus d'infos](http://nsivaugelas.free.fr/terminale/listes.php)


## implémentation récursive avec une seule classe

```py
class ListeChaineeRecursive:
    def __init__(self, valeur=None, suivant=None):
        """
        Initialise une liste chaînée avec une valeur et l'élément suivant.
        
        Args:
            valeur: La valeur à stocker dans cet élément (par défaut None pour une liste vide).
            suivant: L'élément suivant dans la liste (par défaut None).
        """
        self.valeur = valeur
        self.suivant = suivant

    def ajouter(self, valeur):
        """
        Ajoute un élément à la liste chaînée.
        
        Args:
            valeur: La valeur à ajouter.
        """
        if self.valeur is None:
            self.valeur = valeur
        elif self.suivant is None:
            self.suivant = ListeChaineeRecursive(valeur)
        else:
            self.suivant.ajouter(valeur)

    def retirer_a_index(self, index, precedent=None):
        """
        Retire l'élément à l'index spécifié de la liste chaînée.
        
        Args:
            index: L'index de l'élément à retirer.
            precedent: L'élément précédent (par défaut None).
        """
        if self.valeur is None:
            return
        
        if index == 0:
            if precedent is not None:
                precedent.suivant = self.suivant
            else:
                if self.suivant is None:
                    self.valeur = None
                else:
                    self.valeur = self.suivant.valeur
                    self.suivant = self.suivant.suivant
        elif self.suivant is not None:
            self.suivant.retirer_a_index(index - 1, self)

    def longueur(self):
        """
        Calcule la longueur de la liste chaînée.
        
        Returns:
            int: La longueur de la liste.
        """
        if self.valeur is None:
            return 0
        elif self.suivant is None:
            return 1
        else:
            return 1 + self.suivant.longueur()

    def afficher(self):
        """
        Affiche les éléments de la liste chaînée.
        """
        courant = self
        while courant is not None:
            if courant.valeur is not None:
                print(courant.valeur, end=" -> ")
            courant = courant.suivant
        print("None")

# Exemple d'utilisation
liste = ListeChaineeRecursive()
liste.ajouter(10)
liste.ajouter(20)
liste.ajouter(30)

liste.afficher()
liste.retirer_a_index(1)
liste.afficher()

```



## code de la liste chainé implémentation avec les noeuds

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
        pass

    def retirer_a_index(self, index):
        """
        Retire l'élément à l'index spécifié de la liste chaînée.
        
        Args:
            index: L'index de l'élément à retirer.
        """
        pass

    def longueur(self):
        """
        Calcule la longueur de la liste chaînée.
        
        Returns:
            int: La longueur de la liste.
        """
        pass

    def afficher(self):
        """
        Affiche les éléments de la liste chaînée.
        """
        pass

        
```
[correction](liste_cor.md)