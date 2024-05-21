# Les fonctions mathématiques sont-elles des outils de chiffrement efficaces ?

Non, les fonctions mathématiques simples comme les transformations linéaires ou les applications bijectives non linéaires ne sont généralement pas considérées comme des outils de chiffrement efficaces par elles-mêmes. Voici pourquoi:

## Transformations linéaires

Les transformations linéaires comme la multiplication par une matrice inversible ne sont pas sûres pour le chiffrement car si un attaquant obtient suffisamment de paires de textes clairs et chiffrés, il peut retrouver facilement la clé (la matrice) en résolvant un système d'équations linéaires[1](https://www.math.u-bordeaux.fr/~cbachocb/Enseignements/CodesCryptoL1/CC-cours.pdf).

## Applications bijectives non linéaires

Bien que plus difficiles à casser que les transformations linéaires, les applications bijectives non linéaires ne sont pas non plus recommandées pour le chiffrement. La raison est qu'il faudrait mémoriser une énorme quantité de données (environ n*2^n bits pour une application de {0,1}^n dans {0,1}^n) pour spécifier complètement une telle application[1](https://www.math.u-bordeaux.fr/~cbachocb/Enseignements/CodesCryptoL1/CC-cours.pdf).

Les algorithmes de chiffrement modernes comme AES, DES, RSA etc. utilisent des constructions mathématiques plus complexes impliquant des opérations non linéaires, des substitutions et des permutations répétées sur les données. Cela les rend beaucoup plus robustes face aux attaques par rapport aux simples fonctions mathématiques[2](https://www.ionos.fr/digitalguide/serveur/securite/apercu-des-diverses-procedures-de-chiffrement/)[5](https://www.kaspersky.fr/resource-center/definitions/encryption).

Citations:
[1](https://www.math.u-bordeaux.fr/~cbachocb/Enseignements/CodesCryptoL1/CC-cours.pdf)
[2](https://www.ionos.fr/digitalguide/serveur/securite/apercu-des-diverses-procedures-de-chiffrement/)
[3](https://fr.wikipedia.org/wiki/Chiffrement_RSA)
[4](https://www.sealpath.com/fr/blog/types-de-chiffrement-guide/)
[5](https://www.kaspersky.fr/resource-center/definitions/encryption)
