# db-Modeling-Workshop

## Objectifs :  
1. Établir le dictionnaire de donnés,
2. Réaliser le MCD et le MLD.

## Énoncé 1: Gestion de stock (Entrée)
Dans l’entreprise "X", les produits (caractérisés par un code et une désignation et un prix unitaire) peuvent soit être fabriqués par l’entreprise ou provenir de différents fournisseurs (caractérisés par un numéro et un nom et une adresse).
Un même produit peut provenir de plusieurs fournisseurs à des prix d’achat différents.
Un fournisseur peut livrer plusieurs produits.

1. Établir le dictionnaire de données.
2. Identifier les règles de gestion.
3. Réaliser un MCD.
4. Déduire MLD.
5. Déduire le modèle relationnel.

 ## Énoncé 2 : Gestion de stock (Sortie)
- Le magasin vend des produits à des clients.
- Les produits possèdent une référence (un code), un libellé et un prix unitaire.
- Les clients ont une identité, nom, prénom, adresse.
- Les clients passent des commandes de produits. On mémorise la date de la commande.
- Pour chaque commande, le client précise une adresse de livraison.
- La commande concerne un certain nombre de produits, en une quantité spécifiée pour chaque produit.
 
1. Établir le dictionnaire de données.
2. Identifier les règles de gestion.
3. Réaliser un MCD.
4. Déduire MLD.
5. Déduire le modèle relationnel.

## Énoncé 3 : Gestion d’un institut de formation
On veut réaliser l’informatisation d’un institut de formation.

- Les cours sont organisés en modules, chaque module est caractérisé par un numéro de module, un intitulé, une durée en heures et un type.

- Les étudiants suivent des enseignements portant sur plusieurs modules. Chaque étudiant est caractérisé par un numéro d’inscription unique, un nom, un prénom et une adresse et une date de naissance, un étudiant est évalué trois fois pour chaque module et possède une note de fin de module.

- Chaque étudiant appartient à un groupe caractérisé par un code, une spécialité et le nombre d’étudiants qu’il comporte.

- Un enseignant intervient dans un module pour un groupe donné à une date donnée, chaque enseignant est caractérisé par un code, un nom, un prénom et une adresse.

- Un enseignant intervient habituellement dans plusieurs modules.

- On désire aussi mémoriser le nombre d’heures effectué par chaque enseignant dans un module donné pour un groupe donné.

1. Établir le dictionnaire de données.
2. Identifier les règles de gestion.
3. Réaliser un MCD.
4. Déduire MLD.
5. Déduire le modèle relationnel.

## Énoncé 4 

Installer le serveur local `XAMPP` ou un outil similaire. En utilisant l'outil MySQL `phpmyadmin` executez les tâches suivantes:
0. Créer la base de `HR` en se base sur le shéma relationnelle illustré sur l'image `HR-DB.jpeg`.
1. Dans la table `countries` insérer en une seule requête les enregistrements suivant : 
('AR', 'Argentina', '2'),
('AU', 'Australia', '3'),
('BE', 'Belgium', '1'),
('BR', 'Brazil', '2'),
('CA', 'Canada', '2'),
('CH', 'Switzerland', '1'),
('CN', 'China', '3'),
('DE', 'Germany', '1'),
('DK', 'Denmark', '1'),
('EG', 'Egypt', '4'),
('FR', 'France', '1'),
('HK', 'HongKong', '3'),
('IL', 'Israel', '4'),
('IN', 'India', '3'),
('IT', 'Italy', '1'),
('JP', 'Japan', '3'),
('KW', 'Kuwait', '4'),
('MX', 'Mexico', '2'),
('NG', 'Nigeria', '4'),
('NL', 'Netherlands', '1'),
('SG', 'Singapore', '3'),
('UK', 'United Kingdom', '1'),
('US', 'United States of America', '2'),
('ZM', 'Zambia', '4'),
('ZW', 'Zimbabwe', '4')

2. Dans la table `departments` insérer en une seule requête les enregistrements suivant : 
('10', 'Administration', '200', '1700'),
('20', 'Marketing', '201', '1800'),
('30', 'Purchasing', '114', '1700'),
('40', 'Human Resources', '203', '2400'),
('50', 'Shipping', '121', '1500'),
('60', 'IT', '103', '1400'),
('70', 'Public Relations', '204', '2700'),
('80', 'Sales', '145', '2500'),
('90', 'Executive', '100', '1700'),
('100', 'Finance', '108', '1700'),
('110', 'Accounting', '205', '1700'),
('120', 'Treasury', '0', '1700'),
('130', 'Corporate Tax', '0', '1700'),
('140', 'Control And Credit', '0', '1700'),
('150', 'Shareholder Services', '0', '1700'),
('160', 'Benefits', '0', '1700'),
('170', 'Manufacturing', '0', '1700'),
('180', 'Construction', '0', '1700'),
('190', 'Contracting', '0', '1700'),
('200', 'Operations', '0', '1700'),
('210', 'IT Support', '0', '1700'),
('220', 'NOC', '0', '1700'),
('230', 'IT Helpdesk', '0', '1700'),
('240', 'Government Sales', '0', '1700'),
('250', 'Retail Sales', '0', '1700'),
('260', 'Recruiting', '0', '1700'),
('270', 'Payroll', '0', '1700');

3. Dans la table `employees` insérer en une seule requête les enregistrements suivant : 
('100', 'Steven', 'King', 'SKING', '515.123.4567', '1987-06-17', 'AD_PRES', '24000.00', '0.00', '0', '90'),
('101', 'Neena', 'Kochhar', 'NKOCHHAR', '515.123.4568', '1987-06-18', 'AD_VP', '17000.00', '0.00', '100', '90'),
('102', 'Lex', 'De Haan', 'LDEHAAN', '515.123.4569', '1987-06-19', 'AD_VP', '17000.00', '0.00', '100', '90'),
('103', 'Alexander', 'Hunold', 'AHUNOLD', '590.423.4567', '1987-06-20', 'IT_PROG', '9000.00', '0.00', '102', '60'),
('104', 'Bruce', 'Ernst', 'BERNST', '590.423.4568', '1987-06-21', 'IT_PROG', '6000.00', '0.00', '103', '60'),
('105', 'David', 'Austin', 'DAUSTIN', '590.423.4569', '1987-06-22', 'IT_PROG', '4800.00', '0.00', '103', '60'),
('106', 'Valli', 'Pataballa', 'VPATABAL', '590.423.4560', '1987-06-23', 'IT_PROG', '4800.00', '0.00', '103', '60'),
('107', 'Diana', 'Lorentz', 'DLORENTZ', '590.423.5567', '1987-06-24', 'IT_PROG', '4200.00', '0.00', '103', '60'),
('108', 'Nancy', 'Greenberg', 'NGREENBE', '515.124.4569', '1987-06-25', 'FI_MGR', '12000.00', '0.00', '101', '100'),
('109', 'Daniel', 'Faviet', 'DFAVIET', '515.124.4169', '1987-06-26', 'FI_ACCOUNT', '9000.00', '0.00', '108', '100'),
('110', 'John', 'Chen', 'JCHEN', '515.124.4269', '1987-06-27', 'FI_ACCOUNT', '8200.00', '0.00', '108', '100'),
('111', 'Ismael', 'Sciarra', 'ISCIARRA', '515.124.4369', '1987-06-28', 'FI_ACCOUNT', '7700.00', '0.00', '108', '100'),
('112', 'Jose Manuel', 'Urman', 'JMURMAN', '515.124.4469', '1987-06-29', 'FI_ACCOUNT', '7800.00', '0.00', '108', '100'),
('113', 'Luis', 'Popp', 'LPOPP', '515.124.4567', '1987-06-30', 'FI_ACCOUNT', '6900.00', '0.00', '108', '100'),
('114', 'Den', 'Raphaely', 'DRAPHEAL', '515.127.4561', '1987-07-01', 'PU_MAN', '11000.00', '0.00', '100', '30'),
('115', 'Alexander', 'Khoo', 'AKHOO', '515.127.4562', '1987-07-02', 'PU_CLERK', '3100.00', '0.00', '114', '30'),
('116', 'Shelli', 'Baida', 'SBAIDA', '515.127.4563', '1987-07-03', 'PU_CLERK', '2900.00', '0.00', '114', '30'),
('117', 'Sigal', 'Tobias', 'STOBIAS', '515.127.4564', '1987-07-04', 'PU_CLERK', '2800.00', '0.00', '114', '30'),
('118', 'Guy', 'Himuro', 'GHIMURO', '515.127.4565', '1987-07-05', 'PU_CLERK', '2600.00', '0.00', '114', '30')



