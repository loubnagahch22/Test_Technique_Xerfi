# Pipotron Checker

Ce projet propose un script Python permettant de déterminer si une phrase donnée est générée par un pipotron. Un pipotron est un générateur automatique de phrases construit en assemblant aléatoirement des composants préalablement définis.

## Comment utiliser le script

### Prérequis

- Python 3.x installé sur votre machine.

### Installation

1. Clonez le repository sur votre machine :

```bash
git clone https://github.com/votre-utilisateur/pipotron-checker.git
```

2. Accédez au répertoire du projet :

```bash
cd pipotron-checker
```

### Exécution

Exécutez le script en utilisant la commande suivante :

```bash
python pipotron_checker.py p_size list_possibilities sentence
```

- `p_size` : un entier supérieur ou égal à 2 représentant la taille du pipotron.
- `list_possibilities` : un dictionnaire contenant l'ensemble des possibilités pour chaque composant du pipotron. Assurez-vous que le dernier composant est une ponctuation.
- `sentence` : une phrase au format string à tester.

### Exemple

```bash
python pipotron_checker.py 2 {"component1": ["mot1", "mot2"], "component2": ["phrase1", "phrase2"]} "mot1 phrase2."
```

## Exemple de structure du dictionnaire `list_possibilities`

```python
{
    "component1": ["mot1", "mot2", "mot3"],
    "component2": ["phrase1", "phrase2", "phrase3"],
    "component3": ["autre1", "autre2"],
    "punctuation": [".", "!", "?"]
}
```
