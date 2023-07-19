# Cours modélisation de données

## 1. Commandes Git

Cette commande va initialiser un dépôt Git. Git va traquer les modifs effectuées au sein de ce dossier.

```sh
git init
```

Pour consulter l'etat du dépôt Git, il suffit de lancer cette commande:

```sh
git status
```

Cette commande va afficher les fichiers qui ont été modifiés depuis le dernier commit.

Pour ajouter un fichier au prochain commit, il faut utiliser la commande:

```sh
git add <nom du fichier>
```

Pour ajouter tous les fichiers modifiés au prochain commit, il faut utiliser la commande:

```sh
git add .
```

Pour enregistrer les modifications dans le dépôt Git, il faut utiliser la commande:

```sh
git commit -m "Message du commit"
```

## 2. Merise

Merise est une méthode de modélisation de données. Elle permet de représenter les données d'un système d'information.
Merise est un acronyme de : Méthode d'Etude et de Réalisation Informatique pour les Systemes d'Entreprise.

Présentation générale de Merise:
Cette méthode est composée de 3 points clés :

- Une approche dite systémique : on transforme les process de l'entreprise en système d'information.
- une séparation des données et des traitements : on sépare les données et les traitements pour faciliter la maintenance.
- une approche nivelée : on découpe le système d'information en plusieurs niveaux.

### 2.1 L'appoche systémique

Le système de pilotage :

- Il est composé de l'ensemble des acteurs qui vont **piloter** le système d'information.

Le système d'information :

- Il est composé de l'ensemble des acteurs qui vont **utiliser** le système d'information.

Le système opérant :

- Il est composé de l'ensemble des acteurs qui vont **produire** les données du système d'information.

### 2.2 La séparation des données et des traitements

La séparation des données et des traitements permet de séparer les données du système d'information et les traitements éffectués sur ces données.
Cette démarche se fait en 3 étapes :

- L'analyse des flux : on analyse les flux d'informations entre les acteurs du système d'information et les acteurs du système opérant.
- L'étude des documents internes (factures, bon de livraison, etc...).
- L'étude des documents externes (fournisseurs, clients, etc...).

Les différents types d'informations :

- les infos de bases ou élmentaires : ce sont les informations qui sont à l'origine du système d'information.
- les informations calculées : ce sont les informations qui sont calculées à partir des informations de bases.
- les traitements ou les fonctions : ce sont les traitements qui sont effectués sur les informations de bases pour obtenir les informations calculées.

En résumé : vous devrez identifiées les données et les traitements effectués sur ces données.

### 2.3 L'approche nivelée

Pour effectuer la conception d'un SI, on va utiliser une approche nivelée. Cette approche se compose de 4 niveaux :

- Le niveau conceptuel : on va représenter les données du système d'information.
- Le niveau organisationnel : on va représenter les traitements du système d'information.
- Le niveau logique : on va représenter les données et les traitements du système d'information.
- Le niveau physique : on va représenter les données et les traitements du système d'information.

#### 2.3.1 Le niveau conceptuel

Le niveau conceptuel permet de modéliser les données de l'entreprise. On va utiliser le modèle conceptuel de données (MCD) pour représenter les données de l'entreprise et le MCT pour représenter les traitements de l'entreprise.

#### 2.3.2 Le niveau organisationnel

Le niveau organisationnel va permettre d'intégrer à l'analyse précédente toutes les notions de temporalité, de chronologie des opérations, de contraintes géographiques. On va utiliser le modèle organisationnel des traitements (MOT) et le modèle organisationnel des données (MOD) pour modéliser les traitements de l'entreprise.

En résumé, on se pose les questions suivantes à partir des données recueillies au niveau conceptuel :

- **Quand** les traitements sont-ils effectués ?
- **Où** les traitements sont-ils effectués ?
- **Qui** effectue les traitements ?

#### 2.3.3 Le niveau logique
