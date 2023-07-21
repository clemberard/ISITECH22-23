# Merise Hotel

## 1. Dictionnaire des données

- Clients(id_client, nom, prenom, adresse, mail, telephone)
- Chambres(numero_chambre, etat, disponibilite, tarif, entretien)
- Services(id_service, nom)
- Personnels(id_personnel, poste, nom, prenom, adresse, mail, telephone, horaire)
- Conges(id_personnel, date_debut, date_retour, nb_jours)
- Foramtions(id_personnel, nom, nb_jours)
- Article(id_article, nom, utilise)
- Stock(id_article, capacite)
- Facturation(num_facture, date, montant)
- Credits(num_credits, date, montant)
- Hotel(id_hotel, nom, cp, ville, adresse)

## 2. Modèle conceptuel de données

Le fichier .asi est disponible dans le même dossier que ce fichier.
![MCD](capture_mcd_hotel.png)

## 3. Modèle logique de données

Le fichier .asi est disponible dans le même dossier que ce fichier.
![MLD](capture_mld_hotel.png)

## 4. Modèle physique de données

```sql
CREATE TABLE `clients` (
  `id_client` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `nom` varchar(50) NOT NULL,
  `prenom` varchar(50) NOT NULL,
  `adresse` varchar(100) NOT NULL,
  `mail` varchar(100) NOT NULL,
  `telephone` varchar(20) NOT NULL
)

CREATE TABLE `chambres` (
  `numero_chambre` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `etat` varchar(50) NOT NULL,
  `disponibilite` boolean NOT NULL,
  `tarif` float(11) NOT NULL,
  `entretien` varchar(50) NOT NULL
)

CREATE TABLE `services` (
  `id_service` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `nom` varchar(50) NOT NULL
)

CREATE TABLE `personnels` (
  `id_personnel` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `poste` varchar(50) NOT NULL,
  `nom` varchar(50) NOT NULL,
  `prenom` varchar(50) NOT NULL,
  `adresse` varchar(100) NOT NULL,
  `mail` varchar(100) NOT NULL,
  `telephone` varchar(20) NOT NULL,
  `horaire` varchar(50) NOT NULL
)

CREATE TABLE `conges` (
  `id_personnel` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `date_debut` date NOT NULL,
  `date_retour` date NOT NULL,
  `nb_jours` int(11) NOT NULL
)

CREATE TABLE `formations` (
  `id_personnel` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `nom` varchar(50) NOT NULL,
  `nb_jours` int(11) NOT NULL
)

CREATE TABLE `article` (
  `id_article` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `nom` varchar(50) NOT NULL,
  `utilise` boolean NOT NULL
)

CREATE TABLE `stock` (
  `id_article` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `capacite` int(11) NOT NULL
)

CREATE TABLE `facturation` (
  `num_facture` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `date` date NOT NULL,
  `montant` float(11) NOT NULL
)

CREATE TABLE `credits` (
  `num_credits` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `date` date NOT NULL,
  `montant` float(11) NOT NULL
)

CREATE TABLE `hotel` (
  `id_hotel` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `nom` varchar(50) NOT NULL,
  `cp` int(11) NOT NULL,
  `ville` varchar(50) NOT NULL,
  `adresse` varchar(100) NOT NULL
)
```
