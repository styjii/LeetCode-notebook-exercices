# LeetCode en notebooks Jupyter

Recueil d'exercices d'algorithmique issus de [LeetCode](https://leetcode.com/problemset/), présentés sous forme de **notebooks Jupyter** autonomes, à résoudre **hors ligne** en Python.

Chaque notebook contient l'énoncé complet en français, des exemples illustrés, les contraintes, un squelette de code à compléter, une batterie de tests automatiques, une grille d'analyse et des pistes de réflexion progressives. Aucune solution n'est fournie : l'objectif est de s'entraîner.

---

## Sommaire

- [Exercices](#exercices)
- [Structure du dépôt](#structure-du-dépôt)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Structure d'un notebook](#structure-dun-notebook)
- [Fonctionnement des tests](#fonctionnement-des-tests)
- [Suivi de progression](#suivi-de-progression)
- [Conseils](#conseils)

---

## Exercices

| N°  | Exercice                                                                                                                        | Difficulté | Thèmes                                           | Notebook                                                                         |
| --- | ------------------------------------------------------------------------------------------------------------------------------- | ---------- | ------------------------------------------------ | -------------------------------------------------------------------------------- |
| 1   | [Two Sum](https://leetcode.com/problems/two-sum/)                                                                               | Facile     | Tableaux, table de hachage                       | [01-two_sum.ipynb](01-two_sum.ipynb)                                             |
| 2   | [Add Two Numbers](https://leetcode.com/problems/add-two-numbers/)                                                               | Moyen      | Listes chaînées, mathématiques, récursivité      | [02-add_two_numbers.ipynb](02-add_two_numbers.ipynb)                             |
| 3   | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/) | Moyen      | Chaînes, table de hachage, fenêtre glissante     | [03-longest_substring.ipynb](03-longest_substring.ipynb)                         |
| 4   | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/)                                       | Difficile  | Tableaux, recherche binaire, diviser pour régner | [04-median_two_sorted_arrays.ipynb](04-median_two_sorted_arrays.ipynb)           |
| 5   | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/)                                   | Moyen      | Chaînes, programmation dynamique, deux pointeurs | [05-longest_palindromic_substring.ipynb](05-longest_palindromic_substring.ipynb) |
| 6   | [Zigzag Conversion](https://leetcode.com/problems/zigzag-conversion/)                                                           | Moyen      | Chaînes                                          | [06-zigzag_conversion.ipynb](06-zigzag_conversion.ipynb)                         |
| 7   | [Reverse Integer](https://leetcode.com/problems/reverse-integer/)                                                               | Moyen      | Mathématiques                                    | [07-reverse_integer.ipynb](07-reverse_integer.ipynb)                             |
| 8   | [String to Integer (atoi)](https://leetcode.com/problems/string-to-integer-atoi/)                                               | Moyen      | Chaînes                                          | [08-string_to_integer_atoi.ipynb](08-string_to_integer_atoi.ipynb)               |
| 9   | [Palindrome Number](https://leetcode.com/problems/palindrome-number/)                                                           | Facile     | Mathématiques                                    | [09-palindrome_number.ipynb](09-palindrome_number.ipynb)                         |
| 10  | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/)                                       | Difficile  | Chaînes, programmation dynamique, récursivité    | [10-regular_expression_matching.ipynb](10-regular_expression_matching.ipynb)     |

---

## Structure du dépôt

```
.
├── .gitignore
├── README.md
├── 01-two_sum.ipynb
├── 02-add_two_numbers.ipynb
├── 03-longest_substring.ipynb
├── 04-median_two_sorted_arrays.ipynb
├── 05-longest_palindromic_substring.ipynb
├── 06-zigzag_conversion.ipynb
├── 07-reverse_integer.ipynb
├── 08-string_to_integer_atoi.ipynb
├── 09-palindrome_number.ipynb
└── 10-regular_expression_matching.ipynb
```

Les notebooks sont numérotés selon l'ordre des problèmes sur LeetCode. Le préfixe à deux chiffres garantit un tri correct dans l'explorateur de fichiers et dans `git`.

---

## Prérequis

- Python 3.8 ou supérieur
- `pip` (gestionnaire de paquets Python)
- Jupyter Notebook, JupyterLab, ou VS Code avec l'extension Jupyter

Aucune connexion Internet n'est nécessaire pour résoudre les exercices une fois l'environnement installé.

---

## Installation

```bash
# 1. Cloner le dépôt
git clone <url-du-depot>
cd <nom-du-depot>

# 2. Créer et activer un environnement virtuel
python3 -m venv .venv
source .venv/bin/activate        # Windows : .venv\Scripts\activate

# 3. Installer Jupyter
pip install notebook
```

Pour utiliser JupyterLab à la place : `pip install jupyterlab`.

---

## Utilisation

Lancer Jupyter depuis la racine du dépôt :

```bash
jupyter notebook
```

Puis ouvrir un notebook, par exemple `01-two_sum.ipynb`. Il est aussi possible de l'ouvrir directement :

```bash
jupyter notebook 01-two_sum.ipynb
```

> **Remarque :** si la mise en forme (encadrés, tableaux colorés) ne s'affiche pas, cliquez sur **Trust** (Faire confiance) dans la barre de menu de Jupyter, puis exécutez les cellules avec `Maj + Entrée`.

---

## Structure d'un notebook

Tous les notebooks suivent la même organisation :

| Section                 | Contenu                                                                    |
| ----------------------- | -------------------------------------------------------------------------- |
| Bannière                | Numéro, titre, difficulté et thèmes de l'exercice                          |
| 1. Énoncé               | Description du problème, en français                                       |
| 2. Exemples             | Exemples illustrés avec entrées, sorties et explications                   |
| 3. Contraintes          | Limites sur les entrées, remarques importantes                             |
| 4. Consignes de travail | Marche à suivre pour réaliser l'exercice                                   |
| 5. Votre solution       | Cellule de code avec le squelette à compléter                              |
| 6. Tests                | Cellule de code qui valide votre solution                                  |
| 7. Analyse              | Tableau à remplir : complexités en temps et en espace, approche, remarques |
| 8. Pistes de réflexion  | Indices progressifs, repliables, à consulter en dernier recours            |

Certains notebooks contiennent des cellules supplémentaires (par exemple la définition de `ListNode` et des fonctions utilitaires pour l'exercice 2).

**Ordre d'exécution :** exécutez les cellules de haut en bas. Complétez d'abord la cellule _Votre solution_, exécutez-la, puis lancez la cellule _Tests_.

---

## Fonctionnement des tests

La cellule _Tests_ affiche un tableau récapitulatif avec, pour chaque cas, l'entrée, le résultat attendu, le résultat obtenu et un statut :

| Statut   | Signification                                                                   |
| -------- | ------------------------------------------------------------------------------- |
| `REUSSI` | Le résultat est correct                                                         |
| `ECHEC`  | Le résultat est incorrect, ou une erreur a été levée                            |
| `LENT`   | Le résultat est correct mais obtenu en plus d'une seconde (selon les exercices) |

Un bilan final indique le nombre de tests réussis.

Selon l'exercice, la cellule affiche également des **indications complémentaires**, qui ne font jamais échouer les tests :

- **Exercice 4** : un test bonus sur de très grands tableaux vérifie si la complexité logarithmique est atteinte.
- **Exercice 8** : détection d'un éventuel appel à `int()`, `float()` ou `eval()`, interdits par l'énoncé.
- **Exercice 9** : détection d'une conversion en chaîne de caractères, à éviter pour répondre à la question de suivi.
- **Exercice 10** : détection de l'utilisation du module `re`.

Ces détections reposent sur l'analyse du code source de votre méthode ; elles peuvent être indisponibles dans certains environnements, auquel cas un message l'indique.

Les résultats attendus sont écrits explicitement dans les cellules de tests ou construits de manière simple : aucune solution n'y est incluse.

---

## Suivi de progression

- [ ] 01 - Two Sum
- [ ] 02 - Add Two Numbers
- [ ] 03 - Longest Substring Without Repeating Characters
- [ ] 04 - Median of Two Sorted Arrays
- [ ] 05 - Longest Palindromic Substring
- [ ] 06 - Zigzag Conversion
- [ ] 07 - Reverse Integer
- [ ] 08 - String to Integer (atoi)
- [ ] 09 - Palindrome Number
- [ ] 10 - Regular Expression Matching

---

## Conseils

- **Commencez simple.** Une solution par force brute correcte vaut mieux qu'une solution optimisée incorrecte. Optimisez ensuite.
- **Dessinez** le problème sur papier avant de coder, en particulier pour les exercices 2, 5, 6 et 10.
- **Renseignez la section Analyse** à chaque exercice : calculer la complexité de sa propre solution est l'un des meilleurs entraînements.
- **Interrompez le noyau** (bouton d'arrêt) si l'exécution des tests dure trop longtemps : votre solution est probablement trop coûteuse pour les grandes entrées.
- **Consultez les pistes une à une**, dans l'ordre, et seulement si nécessaire.
