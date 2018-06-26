# Si-AC + Site AC évolutions

## 1. possibilité de générer automatiquement des pages terminales
possibilité d'associer des ressources informationnelles à des pages générées automatiquement

## 2. possibilité de créer des liens, tuiles, ... sur des pages générées à la volée
possibilité de créer des liens, tuiles, ... sur le moteur de recherche dûment paramétré (Ex.1: recherche de toutes les oeuvres musicales au répertoire: oEuvre: ∃ une oeuvre liée à une prestation taguée "événement" et "musique"; Ex.2: recherche de toutes les prestations actuelles sur le campus Valais, triées chronologiquement)

## 3. site web mixant des pages avec contenu en dur, avec contenu généré, et pages générées

## 4. nouvelle structure de site:
	culture
		catalogue
			-cours
			-cycles et colloques (tout ce qui est architecturé)
			-événements
			-billets offerts
			-oeuvres au répertoire
		cinéclub
		choeur
		orchestre
		moteur de recherche/requêtes sur les archives
		pages diverses (en dur)
			- projets
			- partenaires
			- contacts
			- informations pratiques
			- faq
			- règlements divers
			- galeries
			- informations culturelles

## 5. catalogue des prestations: expressions paramétrées par défaut du moteur de recherche
		catalogue des cours: expression d'un recherche sur le SIAC
			- structure: cours
			- matière: -
			- disponibilité: actuelle
			- inscription: -
			- calendrier: -
			- tri: alphabétique du titre
			- navigation au sein des prestations par filtre / facettes
				- matière 1: danse, écriture, image, musique, nature, théâtre
				- matière 2: déclinées selon matière 1
				- date calendaire (=,>,<)
				- lieu
				- personne
			- tris alternatifs (alphabétique du titre, chronologique, par personne, ...)
			- recherche libre
			- réinitialisation des paramètres par défaut du catalogue des cours
		
		catalogue des cycles et colloques
			- structure: cycle
			- matière: -
			- disponibilité: actuelle
			- inscription: -
			- caldendrier: à partir d'aujourdhui
			- tri: chronologique
			
			- navigation au sein des prestations par filtre / facettes
				- matière 1: danse, écriture, image, musique, nature, théâtre
				- matière 2: déclinées selon matière 1
				- date calendaire (=,>,<)
				- lieu
				- personne
			- tris alternatifs (alphabétique du titre, chronologique, par personne, ...)
			- recherche libre
			- réinitialisation des paramètres par défaut du catalogue des cycles et colloques

		catalogue des événements (y compris séances ccu, cf plus bas)
			- structure: événement
			- matière 1: -
			- disponibilité: actuelle
			- inscription: -
			- caldendrier: à partir d'aujourdhui
			- tri: chronologique
			
			- navigation au sein des prestations par filtre / facettes
				- matière 1: danse, écriture, image, musique, nature, théâtre
				- matière 2: déclinées selon matière 1
				- date calendaire (=,>,<)
				- lieu
				- personne
			- tris alternatifs (alphabétique du titre, chronologique, par personne, ...)
			- recherche libre
			- réinitialisation des paramètres par défaut du catalogue des événements

		catalogue des billets offerts
			- structure: billet offert
			- matière: -
			- disponibilité: actuelle
			- inscription: -
			- calendrier: -
			- tri: par personne (partenaire)
			
			- navigation au sein des prestations par filtre / facettes
				- matière 1: danse, écriture, image, musique, nature, théâtre
				- matière 2: déclinées selon matière 1
				- date calendaire (=,>,<)
				- lieu
				- personne
			- tris alternatifs (alphabétique du titre, chronologique, par personne, ...)
			- recherche libre
			- réinitialisation des paramètres par défaut

		catalogue des oeuvres au répertoire AC
			- structure: -
			- matière: -
			- disponibilité: actuelle
			- inscription: -
			- calendrier: -
			- tri: par oeuvre
			- les prestations pour lesquelles ∃ au moins 1 oeuvre qui leur soit associée
			
			- navigation au sein des prestations par filtre / facettes
				- matière 1: danse, écriture, image, musique, nature, théâtre
				- matière 2: déclinées selon matière 1
				- date calendaire (=,>,<)
				- lieu
				- personne
			- tris alternatifs (alphabétique du titre, chronologique, par auteur, par oeuvre)
			- recherche libre
			- réinitialisation des paramètres par défaut du répertoire des oeuvres

Remarque:
	filtres et facettes constituent le moyen de navigation au sein du catalogue > à présenter tel quel

Remarque:
	format de sortie des résultats générés par la recherche au sein du catalogue
		- liste / grille
		- habillage
		- informations de base: titre, statut inscription, calendrier, lieu, personne, matière, oeuvre

Remarque:
	- nouveau tag structure: cycle (s:cycle); cinéclub devient un tag matière: m:cinéclub
	- toutes les prestations au top d'une architecture sont taguées "cycle", par exemple, les cycles CCU, les cycles de conférences, les cycles cinéma (Histoire et cité, ...), les festivals (Commedia, FUIT);

## 6. CCU
* les prestations cycle sont taguées s:cycle, m:cinéclub, m:cinéma
* les séances CCU sont taguées: s:événement, m:cinéclub, m:cinéma
* la page CCU est créée en dur, le sommaire des cycles actuels est cependant généré: s:cycle, m:cinéclub, m:cinéma, date:actuel, tri:chronologique
* la page du cycle est générée, le sommaire des séances est généré, la prochaine séance est générée, les ressources informationnelles (image) et documentaires (revue, trailer, cahier des fiches filmiques), les crédits (personnes associées à la prestation en tant que groupe de travail) sont générés à la volée

## 7. Archivage
* portfolio: l'historique des personnes doit permettre d'exprimer toutes les relations entre une personne et les Activités culturelles, soit i) à travers une inscription (cours, billets offerts), soit ii) à travers une relation qualifiée ("jeu" pour un événement, "groupe de travail" pour le ciné-club, etc., selon le point 10 ci-dessous)
* permettre l'archivage des productions (événements) à travers le moteur de recherche
* permettre l'archivage des ressources associées aux prestations en distinguant a) les ressources internes au CMS et b) les ressources documentaires externes au CMS (accessibles et récupérables en tout temps):
	* les ressources informationnelles - quel que soit leur support (images, pdf, trailers, etc) - qui servent à la promotion de la prestation à travers, probablement, l'ID de la prestation;
	* les ressources documentaires - quels que soient leur support et leur nature (images des spectacles, enregistrements audiovisuels, revues du CCU, fiches filmiques, critiques, revues de presse, etc) - qui servent à la documentation de la prestation, intégrées dans le système "développé" en parallèle à travers l'ID de la prestation

## 8. Transactions financières
* pas de crédits sur les comptes pour les remboursements et les paiements
* options ajoutées (partitions) considérées comme de nouvelles prestations associées (regroupement). Il n'y a par conséquent pas la possibilité d'enlever une option
* rabais concédés sur les inscriptions:
	* pendant une certaine durée (de type: semaine promotionnelle) pour les paiements synchrones uniquement. Possibilité de développer les méthodes de paiement synchrones de type maestro pre-paid?
	* en fonction d'une condition (de type: participation déjà validée à un autre atelier regroupé)
	* en fonction d'une personne (de type: Anne Zanelli pour une prestation donnée)
	* en fonction du rapport à la prestation (de type: "Animateur", "Comité X", "Groupe de travail" --> implique de modifier les types de relations et de ne pas limiter l'inscription à ce type de relations (exception faite pour les animateurs)
	règles: ° une relation à n'importe quelle prestation de type "Animateur" / un ensemble de prestations définies parmi les cours
		° une relation de type "Comité" / une prestation et ses regroupements			
	* pouvoir annoncer de manière automatique les rabais concédés pour a/b/d de manière i) non individuelle si la personne n'est pas connectée au moment de la navigation (de type: "les animateurs ont droit...") et ii) de manière individuelle si la personne se connecte (panier)
	* obtenir une vue comptable sur les formations:
		* inclure le coût du cours dans la vue "prestation" (insertion manuelle à partir de la feuille excel de gouvernance des cours)
		* inclure le différentiel entre le coût du cours et les paiements reçus dans la vue "prestation"
		* inclure dans la vue particulière de chaque inscription le montant avant rabais et le montant après rabais (soit le montant payé)
		* détailler le calcul dans la vue "paiement" en fonction des prestations (exemple: "danse classique" = 72.-; "danse contemporaine" = 72.-)
		* inclure la possibilité de gérer des paiements échelonnés à travers la vue "inscription" --> pour une inscription, validation partielle en précisant le montant, soit i) plusieurs lignes par date de paiement, soit ii) une case avec montant reçu et mise à jour manuelle --> c'est ce montant qui doit être calculé dans le montant des paiements reçus

## 9. Répertoire des oeuvres
* pour l'indexation des films, des oeuvres musicales, des pièces produits par les AC
* oeuvre: titre 1, titre 2, année de production, détails
* auteur: prénom, nom, date de naissance
* plusieurs auteurs pour une oeuvre, un auteur de plusieurs oeuvres
* les oeuvres sont à lier à une prestation dont elles constituent le programme (dont on renonce provisaoirement à ce qu'il soit exprimé automatiquement)
* doit servir à exprimer:
	* le répertoire des oeuvres exécutées par le choeur ou l'orchestre
	* le répertoire des films passés en séance de Cinéclub
	* la filmographie CCU de tel réalisateur
	* …
	
## 10. Divers:
- labeliser des unités de calendrier (ex: cours d'essai, nouvelle date, date modifiée, ...)
- assurer la synchronisation des calendriers
- communiquer avec les participant-e-s (inscrits, non-inscrits, ayant participé ou non à telle séance) à une prestation
- anonymisation
- gestion des listes d'attentes pour les inscriptions
	comment distinguer une inscription à une prestation d'une inscription à sa liste d'attente
	comment résoudre la question des paiements différés qui valident une inscription à un cours devenu complet entre temps
		> le cours est complet lorsqu'il atteint le nombre d'inscriptions validées par un paiement
		> les inscriptions avec paiement asynchrone passent en liste d'attente jusqu'à validation du paiement tant que la prestation n'est pas complète
		> les inscriptions en attente payées passent, par priorité de date de paiement, en inscription validée si la prestation est incomplète
		> les inscriptions en attente qui sont payées (par paiement synchrone ou asynchrone) restent en attente si la prestation est complète
- modification de la table des lieux (bâtiment universitaire, campus VS)
- labelliser le rapport d'une personne inscrite à une prestation:
	- soprano, alto, tenor, basse
	- violon 1, violon 2, alto, violoncelle, contrebasse
	- trompette, trombone, cor
	- flute, hautbois, clarinette, basson
	- "autre"
- enrichir la palette de rapports possibles entre une personne et une prestation:
	- animateur, partenaire, comité, groupe de travail
	- texte, adaptation, mise en scène, dramaturgie, scénographie, jeu
	- chorégraphie, danse, création
	- direction, soliste, orchestre, choeur
	- son, musique, lumières
- service de réservation/prêt (le matériel MU, les postes informatiques au Studio IX) en ligne
- régler le cas du paiement à double (Maradan Laetitia, ID 13799, paiement validé le 02.10.2017 et le 30.12.2017)
- identification des personnes: SIUS; infos sur les filières, info admin qui s'inscrivent à une prestation
