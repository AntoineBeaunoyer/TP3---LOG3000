# Tests Unitaires - Calculatrice

## Description

Ce projet contient une suite de tests unitaires pour une fonction `calculate()` qui effectue des opérations mathématiques simples. Les tests couvrent les cas nominaux ainsi que les gestion des erreurs.

## Structure du projet

```
.
├── back-end/
│   ├── app.py              # Contient la fonction calculate()
│   ├── operators.py
│   └── README.md
├── README.md
├── front-end/
│    ├── templates/
│    │   └── index.html
│    ├── static/
│    │   └── style.css
│    └── README.md
└── tests/
     ├── tests_app.py         # Tests unitaires
     └── README.md            # Ce fichier
```

## Prérequis

- Python 3.6 ou supérieur
- Aucune dépendance externe requise (utilise le module `unittest` de la stdlib)

## Comment exécuter les tests

### Exécution de tous les tests

```bash
python tests/tests_app.py
```

### Exécution avec verbose (affichage détaillé)

```bash
python tests/tests_app.py -v
```

### Exécution d'un test spécifique

```bash
python tests/tests_app.py MyTestCase.test_addition
```

### Exécution avec unittest depuis la ligne de commande

```bash
python -m unittest tests.tests_app -v
```

## Couverture des tests

La suite de tests couvre les fonctionnalités et cas d'erreur suivants :

### ✅ Opérations arithmétiques valides

| Test | Description | Exemple | Résultat attendu |
|------|-------------|---------|------------------|
| `test_addition` | Addition de deux nombres | `"2+3"` | `5` |
| `test_substraction` | Soustraction de deux nombres | `"5-3"` | `2` |
| `test_multiplication` | Multiplication de deux nombres | `"5*3"` | `15` |
| `test_dicision` | Division de deux nombres | `"9/3"` | `3` |

## Résultat attendu

Lors de l'exécution réussie des tests, vous devriez voir :

```
........
----------------------------------------------------------------------
Ran 8 tests in X.XXXs

OK
```
 les permissions d'exécution sont correctes sur le fichier test
