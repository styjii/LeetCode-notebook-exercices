# LeetCode en notebooks Jupyter

Recueil d'exercices issus de [LeetCode](https://leetcode.com/problemset/), présentés sous forme de **notebooks Jupyter** autonomes, à résoudre **hors ligne** :

- des exercices d'**algorithmique** à résoudre en **Python** ;
- des exercices de **bases de données** à résoudre en **SQL**, exécutés sur une base **SQLite** en mémoire.

Chaque notebook contient l'énoncé complet en français, des exemples illustrés, les contraintes, une cellule à compléter, une batterie de tests automatiques, une grille d'analyse et des pistes de réflexion progressives. Aucune solution n'est fournie : l'objectif est de s'entraîner.

---

## Sommaire

- [Structure du dépôt](#structure-du-dépôt)
- [Exercices d'algorithmique](#exercices-dalgorithmique)
- [Exercices SQL](#exercices-sql)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Structure d'un notebook](#structure-dun-notebook)
- [Fonctionnement des tests](#fonctionnement-des-tests)
- [Suivi de progression](#suivi-de-progression)
- [Conseils](#conseils)
- [Licence](#licence)

---

## Structure du dépôt

```
.
├── LeetCode-Algo
│   ├── 01-two_sum.ipynb
│   ├── 02-add_two_numbers.ipynb
│   ├── 03-longest_substring.ipynb
│   ├── 04-median_two_sorted_arrays.ipynb
│   ├── 05-longest_palindromic_substring.ipynb
│   ├── 06-zigzag_conversion.ipynb
│   ├── 07-reverse_integer.ipynb
│   ├── 08-string_to_integer_atoi.ipynb
│   ├── 09-palindrome_number.ipynb
│   └── 10-regular_expression_matching.ipynb
├── LeetCode-SQLite
│   ├── 175-combine_two_tables.ipynb
│   ├── 176-second_highest_salary.ipynb
│   ├── 177-nth_highest_salary.ipynb
│   ├── 178-rank_scores.ipynb
│   ├── 180-consecutive_numbers.ipynb
│   ├── 181-employees_earning_more_than_managers.ipynb
│   ├── 182-duplicate_emails.ipynb
│   ├── 183-customers_who_never_order.ipynb
│   ├── 184-department_highest_salary.ipynb
│   ├── 185-department_top_three_salaries.ipynb
│   ├── 196-delete_duplicate_emails.ipynb
│   ├── 197-rising_temperature.ipynb
│   ├── 262-trips_and_users.ipynb
│   └── 511-game_play_analysis_i.ipynb
├── LICENSE
└── README.md
```

| Dossier | Contenu |
|---------|---------|
| `LeetCode-Algo` | Exercices d'algorithmique, à résoudre en Python |
| `LeetCode-SQLite` | Exercices SQL, à résoudre avec des requêtes exécutées par SQLite |

Les notebooks sont préfixés par le **numéro du problème sur LeetCode** (sur deux chiffres pour les premiers). Ce préfixe garantit un tri correct dans l'explorateur de fichiers et dans `git`.

---

## Exercices d'algorithmique

Dossier : [`LeetCode-Algo`](LeetCode-Algo)

| N° | Exercice | Difficulté | Thèmes | Notebook |
|----|----------|------------|--------|----------|
| 1 | [Two Sum](https://leetcode.com/problems/two-sum/) | Facile | Tableaux, table de hachage | [01-two_sum.ipynb](LeetCode-Algo/01-two_sum.ipynb) |
| 2 | [Add Two Numbers](https://leetcode.com/problems/add-two-numbers/) | Moyen | Listes chaînées, mathématiques, récursivité | [02-add_two_numbers.ipynb](LeetCode-Algo/02-add_two_numbers.ipynb) |
| 3 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/) | Moyen | Chaînes, table de hachage, fenêtre glissante | [03-longest_substring.ipynb](LeetCode-Algo/03-longest_substring.ipynb) |
| 4 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/) | Difficile | Tableaux, recherche binaire, diviser pour régner | [04-median_two_sorted_arrays.ipynb](LeetCode-Algo/04-median_two_sorted_arrays.ipynb) |
| 5 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/) | Moyen | Chaînes, programmation dynamique, deux pointeurs | [05-longest_palindromic_substring.ipynb](LeetCode-Algo/05-longest_palindromic_substring.ipynb) |
| 6 | [Zigzag Conversion](https://leetcode.com/problems/zigzag-conversion/) | Moyen | Chaînes | [06-zigzag_conversion.ipynb](LeetCode-Algo/06-zigzag_conversion.ipynb) |
| 7 | [Reverse Integer](https://leetcode.com/problems/reverse-integer/) | Moyen | Mathématiques | [07-reverse_integer.ipynb](LeetCode-Algo/07-reverse_integer.ipynb) |
| 8 | [String to Integer (atoi)](https://leetcode.com/problems/string-to-integer-atoi/) | Moyen | Chaînes | [08-string_to_integer_atoi.ipynb](LeetCode-Algo/08-string_to_integer_atoi.ipynb) |
| 9 | [Palindrome Number](https://leetcode.com/problems/palindrome-number/) | Facile | Mathématiques | [09-palindrome_number.ipynb](LeetCode-Algo/09-palindrome_number.ipynb) |
| 10 | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/) | Difficile | Chaînes, programmation dynamique, récursivité | [10-regular_expression_matching.ipynb](LeetCode-Algo/10-regular_expression_matching.ipynb) |

---

## Exercices SQL

Dossier : [`LeetCode-SQLite`](LeetCode-SQLite)

| N° | Exercice | Difficulté | Thèmes | Notebook |
|----|----------|------------|--------|----------|
| 175 | [Combine Two Tables](https://leetcode.com/problems/combine-two-tables/) | Facile | Jointures | [175-combine_two_tables.ipynb](LeetCode-SQLite/175-combine_two_tables.ipynb) |
| 176 | [Second Highest Salary](https://leetcode.com/problems/second-highest-salary/) | Moyen | Sous-requêtes, valeurs `NULL` | [176-second_highest_salary.ipynb](LeetCode-SQLite/176-second_highest_salary.ipynb) |
| 177 | [Nth Highest Salary](https://leetcode.com/problems/nth-highest-salary/) | Moyen | Requête paramétrée, classements | [177-nth_highest_salary.ipynb](LeetCode-SQLite/177-nth_highest_salary.ipynb) |
| 178 | [Rank Scores](https://leetcode.com/problems/rank-scores/) | Moyen | Fonctions de fenêtrage, classements | [178-rank_scores.ipynb](LeetCode-SQLite/178-rank_scores.ipynb) |
| 180 | [Consecutive Numbers](https://leetcode.com/problems/consecutive-numbers/) | Moyen | Auto-jointures, fonctions de fenêtrage | [180-consecutive_numbers.ipynb](LeetCode-SQLite/180-consecutive_numbers.ipynb) |
| 181 | [Employees Earning More Than Their Managers](https://leetcode.com/problems/employees-earning-more-than-their-managers/) | Facile | Auto-jointure | [181-employees_earning_more_than_managers.ipynb](LeetCode-SQLite/181-employees_earning_more_than_managers.ipynb) |
| 182 | [Duplicate Emails](https://leetcode.com/problems/duplicate-emails/) | Facile | Regroupements, `HAVING` | [182-duplicate_emails.ipynb](LeetCode-SQLite/182-duplicate_emails.ipynb) |
| 183 | [Customers Who Never Order](https://leetcode.com/problems/customers-who-never-order/) | Facile | Jointures externes, `NOT IN`, `NOT EXISTS` | [183-customers_who_never_order.ipynb](LeetCode-SQLite/183-customers_who_never_order.ipynb) |
| 184 | [Department Highest Salary](https://leetcode.com/problems/department-highest-salary/) | Moyen | Jointures, regroupements, sous-requêtes | [184-department_highest_salary.ipynb](LeetCode-SQLite/184-department_highest_salary.ipynb) |
| 185 | [Department Top Three Salaries](https://leetcode.com/problems/department-top-three-salaries/) | Difficile | Jointures, fonctions de fenêtrage | [185-department_top_three_salaries.ipynb](LeetCode-SQLite/185-department_top_three_salaries.ipynb) |
| 196 | [Delete Duplicate Emails](https://leetcode.com/problems/delete-duplicate-emails/) | Facile | Instruction `DELETE`, sous-requêtes | [196-delete_duplicate_emails.ipynb](LeetCode-SQLite/196-delete_duplicate_emails.ipynb) |
| 197 | [Rising Temperature](https://leetcode.com/problems/rising-temperature/) | Facile | Dates, auto-jointure | [197-rising_temperature.ipynb](LeetCode-SQLite/197-rising_temperature.ipynb) |
| 262 | [Trips and Users](https://leetcode.com/problems/trips-and-users/) | Difficile | Jointures multiples, agrégation conditionnelle | [262-trips_and_users.ipynb](LeetCode-SQLite/262-trips_and_users.ipynb) |
| 511 | [Game Play Analysis I](https://leetcode.com/problems/game-play-analysis-i/) | Facile | Regroupements, `MIN` | [511-game_play_analysis_i.ipynb](LeetCode-SQLite/511-game_play_analysis_i.ipynb) |

### Particularités des notebooks SQL

- **Exécution :** vous écrivez votre requête SQL dans la variable Python `requete`. Elle est exécutée sur une base **SQLite en mémoire**, créée par le notebook avec le module `sqlite3` de la bibliothèque standard de Python : aucune installation supplémentaire n'est nécessaire.
- **Sécurité :** pour les requêtes de lecture, la base est ouverte en lecture seule (`PRAGMA query_only`) et une seule instruction SQL est acceptée.
- **Exercice 177 :** LeetCode demande de compléter une fonction MySQL. SQLite ne gérant pas les fonctions stockées, ce notebook demande une requête `SELECT` utilisant le **paramètre nommé `:N`** pour le rang demandé.
- **Exercice 196 :** il faut écrire une instruction **`DELETE`** (et non un `SELECT`). Le notebook exécute votre instruction sur une base modifiable, puis compare le **contenu final de la table** `Person` au contenu attendu.
- **Exercice 197 :** SQLite stocke les dates en texte `AAAA-MM-JJ` et utilise des fonctions comme `date()` ou `julianday()`, alors que MySQL utilise `DATEDIFF`, `DATE_SUB` ou `INTERVAL`.
- **Exercice 262 :** les types `ENUM` n'existent pas en SQLite ; ils sont remplacés par du texte avec une contrainte de valeurs. La division de deux entiers est entière en SQLite, il faut donc forcer un calcul décimal, puis arrondir à deux décimales.
- **Exercice 511 :** la clé primaire `(player_id, event_date)` de l'énoncé n'est volontairement pas déclarée dans la table de test (l'unicité du couple est respectée par les données). Avec cette clé, SQLite crée un index qui ferait lire les lignes dans l'ordre des dates, et une requête incorrecte (colonne sans agrégation dans un `GROUP BY`) passerait les tests par hasard.
- **Différences avec LeetCode :** LeetCode utilise MySQL pour ces exercices. Les constructions usuelles (jointures, `GROUP BY`, sous-requêtes, fonctions de fenêtrage) sont identiques, mais certains détails de syntaxe diffèrent. Par exemple :
  - MySQL n'accepte pas d'expression dans `LIMIT` / `OFFSET`, alors que SQLite l'accepte ;
  - MySQL permet `DELETE p1 FROM ...` (suppression avec jointure), que SQLite ne comprend pas ;
  - MySQL refuse une sous-requête sur la table en cours de suppression (erreur 1093), alors que SQLite l'accepte ;
  - les noms de colonnes comme `rank` ou `Cancellation Rate` demandent des accents graves en MySQL.

  Les notebooks le signalent lorsque c'est pertinent.

---

## Prérequis

- Python 3.8 ou supérieur
- `pip` (gestionnaire de paquets Python)
- Jupyter Notebook, JupyterLab, ou VS Code avec l'extension Jupyter
- Pour les exercices SQL utilisant des fonctions de fenêtrage (`DENSE_RANK`, `LAG`, `ROW_NUMBER`, etc.) : **SQLite 3.25 ou supérieur**

Pour connaître la version de SQLite utilisée par votre Python :

```bash
python3 -c "import sqlite3; print(sqlite3.sqlite_version)"
```

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

Puis ouvrir un notebook dans l'un des deux dossiers. Il est aussi possible de l'ouvrir directement :

```bash
jupyter notebook LeetCode-Algo/01-two_sum.ipynb
jupyter notebook LeetCode-SQLite/175-combine_two_tables.ipynb
```

> **Remarque :** si la mise en forme (encadrés, tableaux colorés) ne s'affiche pas, cliquez sur **Trust** (Faire confiance) dans la barre de menu de Jupyter, puis exécutez les cellules avec `Maj + Entrée`.

---

## Structure d'un notebook

### Notebooks d'algorithmique

| Section | Contenu |
|---------|---------|
| Bannière | Numéro, titre, difficulté et thèmes de l'exercice |
| 1. Énoncé | Description du problème, en français |
| 2. Exemples | Exemples illustrés avec entrées, sorties et explications |
| 3. Contraintes | Limites sur les entrées, remarques importantes |
| 4. Consignes de travail | Marche à suivre pour réaliser l'exercice |
| 5. Votre solution | Cellule de code avec le squelette à compléter |
| 6. Tests | Cellule de code qui valide votre solution |
| 7. Analyse | Tableau à remplir : complexités en temps et en espace, approche, remarques |
| 8. Pistes de réflexion | Indices progressifs, repliables, à consulter en dernier recours |

Certains notebooks contiennent des cellules supplémentaires (par exemple la définition de `ListNode` et des fonctions utilitaires pour l'exercice 2).

### Notebooks SQL

| Section | Contenu |
|---------|---------|
| Bannière | Numéro, titre, difficulté et thèmes de l'exercice |
| 1. Énoncé | Schéma des tables et description du problème, en français |
| 2. Exemples | Tables d'entrée et de sortie, avec explications |
| 3. Remarques | Points d'attention et précisions sur l'environnement |
| 4. Consignes de travail | Marche à suivre pour réaliser l'exercice |
| 5. Environnement SQL | Création de la base de l'exemple et fonctions `executer` et `afficher` |
| 6. Votre solution | Variable `requete` dans laquelle écrire votre requête SQL |
| 7. Essai sur l'exemple | Exécution de votre requête sur les données de l'exemple |
| 8. Tests | Exécution de votre requête sur plusieurs jeux de données |
| 9. Analyse | Tableau à remplir : approche, cas particuliers, remarques |
| 10. Pistes de réflexion | Indices progressifs, repliables, à consulter en dernier recours |

**Ordre d'exécution :** exécutez les cellules de haut en bas. Complétez d'abord la cellule *Votre solution*, exécutez-la, puis lancez la cellule *Tests*. Pour les notebooks SQL, la cellule *Environnement SQL* doit être exécutée en premier.

---

## Fonctionnement des tests

La cellule *Tests* affiche un tableau récapitulatif avec, pour chaque cas, l'entrée, le résultat attendu, le résultat obtenu et un statut :

| Statut | Signification |
|--------|---------------|
| `REUSSI` | Le résultat est correct |
| `ECHEC` | Le résultat est incorrect, ou une erreur a été levée |
| `LENT` | Le résultat est correct mais obtenu en plus d'une seconde (selon les exercices) |

Un bilan final indique le nombre de tests réussis. Les résultats attendus sont écrits explicitement dans les cellules de tests ou construits de manière simple : aucune solution n'y est incluse.

### Exercices d'algorithmique

Selon l'exercice, la cellule affiche également des **indications complémentaires**, qui ne font jamais échouer les tests :

- **Exercice 4** : un test bonus sur de très grands tableaux vérifie si la complexité logarithmique est atteinte.
- **Exercice 8** : détection d'un éventuel appel à `int()`, `float()` ou `eval()`, interdits par l'énoncé.
- **Exercice 9** : détection d'une conversion en chaîne de caractères, à éviter pour répondre à la question de suivi.
- **Exercice 10** : détection de l'utilisation du module `re`.

Ces détections reposent sur l'analyse du code source de votre méthode ; elles peuvent être indisponibles dans certains environnements, auquel cas un message l'indique.

### Exercices SQL

Votre requête est exécutée sur **plusieurs jeux de données** (cas courants, cas limites, tables vides, grands jeux de 1000 lignes ou plus). Les vérifications portent selon l'exercice sur :

- le **nom et l'ordre des colonnes** du résultat (la casse compte : `Email` n'est pas `email`) ;
- les **lignes** retournées (manquantes ou en trop, doublons) ;
- l'**ordre des lignes**, lorsque l'énoncé l'impose (exercice 178) ;
- la présence d'une **ligne contenant `NULL`** lorsqu'aucune valeur n'existe (exercices 176 et 177) ;
- les **valeurs arrondies**, lorsque l'énoncé l'impose (exercices 178 et 262) ;
- le **contenu final de la table** après exécution, pour l'exercice 196, qui demande un `DELETE`.

En cas d'échec, la colonne *Détail* explique ce qui ne va pas (par exemple, lignes manquantes, lignes en trop, colonnes incorrectes ou message d'erreur SQL).

Les jeux de tests incluent des pièges classiques : doublons, égalités, valeurs `NULL`, jours manquants, utilisateurs bannis, bornes incluses ou exclues, homonymes, lignes insérées dans le désordre. Une requête qui passe quelques exemples peut donc échouer sur un cas limite.

---

## Suivi de progression

### Algorithmique

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

### SQL

- [ ] 175 - Combine Two Tables
- [ ] 176 - Second Highest Salary
- [ ] 177 - Nth Highest Salary
- [ ] 178 - Rank Scores
- [ ] 180 - Consecutive Numbers
- [ ] 181 - Employees Earning More Than Their Managers
- [ ] 182 - Duplicate Emails
- [ ] 183 - Customers Who Never Order
- [ ] 184 - Department Highest Salary
- [ ] 185 - Department Top Three Salaries
- [ ] 196 - Delete Duplicate Emails
- [ ] 197 - Rising Temperature
- [ ] 262 - Trips and Users
- [ ] 511 - Game Play Analysis I

---

## Conseils

- **Commencez simple.** Une solution par force brute correcte vaut mieux qu'une solution optimisée incorrecte. Optimisez ensuite.
- **Dessinez** le problème sur papier avant de coder, en particulier pour les exercices 2, 5, 6 et 10, ainsi que pour les exercices SQL de classement (177, 178 et 185).
- **Testez vos requêtes SQL sur l'exemple** avant de lancer les tests complets : la cellule *Essai sur l'exemple* est là pour cela.
- **Pensez aux cas limites en SQL** : table vide, valeurs `NULL`, doublons, égalités, bornes d'une période. Les tests les vérifient.
- **Renseignez la section Analyse** à chaque exercice : calculer la complexité de sa propre solution est l'un des meilleurs entraînements.
- **Interrompez le noyau** (bouton d'arrêt) si l'exécution des tests dure trop longtemps : votre solution est probablement trop coûteuse pour les grandes entrées.
- **Consultez les pistes une à une**, dans l'ordre, et seulement si nécessaire.
- **Essayez plusieurs approches** pour un même exercice, notamment en SQL (jointure, sous-requête, fonction de fenêtrage) : chacune a ses avantages.
- **Gardez en tête les différences avec MySQL** avant de soumettre une requête sur LeetCode : une requête valide ici peut devoir être adaptée.

---

## Licence

Ce projet est distribué selon les termes du fichier [LICENSE](LICENSE).

Les énoncés des exercices sont la propriété de [LeetCode](https://leetcode.com/). Ce dépôt n'a pas de lien officiel avec LeetCode ; il sert uniquement à l'entraînement personnel.
