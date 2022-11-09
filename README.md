# Données relatives aux résultats des tests virologiques COVID-19 SI-DEP (Base de données de Santé Publique France)

## 0) Description de la base de données
### a. Carte d'identité

* __Nom__ : Données relatives aux résultats des tests virologiques COVID-19 SI-DEP puis Données de laboratoires pour le dépistage (à compter du 18/05/2022)  
* __Où trouver le jeu de données__ : data.gouv.fr - [Données relatives aux résultats des tests virologiques COVID-19 (SI-DEP)](https://www.data.gouv.fr/fr/datasets/donnees-relatives-aux-resultats-des-tests-virologiques-covid-19/) et [Données de laboratoires pour le dépistage (A COMPTER DU 18/05/2022) - SI-DEP](https://www.data.gouv.fr/fr/datasets/donnees-de-laboratoires-pour-le-depistage-a-compter-du-18-05-2022-si-dep/)  
* __Producteur du jeu de données__ : Santé Publique France  
* __Licence__ : Licence Ouverte / Open Licence version 2.0  
* __Temporalité__ : quotidienne  
* __Date de création__ : 29 mai 2020  
* __Dernière mise à jour__ : 8 novembre 2022  
* __Granularité de la couverture territoriale__ : Iris (quartiers INSEE)  
* __Couverture __territoriale : France  
* __Conservation de la data__ : 10 ans (CNIL + https://www.tf1info.fr/societe/video-coronavirus-si-vaccin-covid-comment-fonctionne-ce-fichier-regroupant-les-donnees-des-personnes-vaccinees-2174533.html)  

### b. Description qualitative générale (c'est que du copié/collé de data.gouv.fr ; faudra affiner/compléter)

* Durant la crise sanitaire liée à l'épidémie du COVID-19, Santé publique France se charge de surveiller et comprendre la dynamique de l'épidémie, d'anticiper les différents scénarii et de mettre en place des actions pour prévenir et limiter la transmission de ce virus sur le territoire national.
* Le nouveau système d’information de dépistage (SI-DEP), en déploiement depuis le 13 mai 2020, est une plateforme sécurisée où sont systématiquement enregistrés les résultats des laboratoires des testsréalisés par l’ensemble des laboratoires de ville et établissements hospitaliers concernant le SARS-COV2.
* La création de ce système d'information est autorisée pour une durée de 6 mois à compter de la fin de l'état d'urgence sanitaire par application du décret n° 2020-551 du 12 mai 2020 relatif aux systèmes d’information mentionnés à l’article 11 de la loi n° 2020-546 du 11 mai 2020 prorogeant l’état d’urgence sanitaire et complétant ses dispositions.
* Le système d’information Dépistage est alimenté par les professionnels de santé réalisant les dépistage.  
* Sur la base de l’exploitation de ces données, Santé Publique France publie en open data les indicateurs de progression de l'épidémie sur data.gouv, sur Geodes ainsi que sur un dashboard disponible sur le site de santé Publique France : InfoCovidFrance  

### c. Description du jeu de données

Le présent jeu de données renseigne à l'échelle __départementale et régionale__ :  
* le nombre de personnes testées et le nombre de personnes déclarées positives par classe d'âge (quotidien et hebdomadaire) ;  
* le nombre de personnes positives sur 7 jours glissants.  

Le présent jeu de données renseigne à l'échelle __nationale__ :  
* le nombre de personnes testées et le nombre de personnes déclarées positives par sexe et classe d'âge (quotidien et hebdomadaire).  
* Le taux de positivité correspond au nombre de tests positifs rapportés au nombre de tests réalisés. Il est calculé de la manière suivante : 100*nombre de test positif/ nombre de tests réalisés  

Précisions : Si plusieurs prélèvements sont rapportés pour un même patient:

* A compter du 29/08, les indicateurs issus des données de laboratoires (SI-DEP) présentent des taux d’incidence, de positivité et de dépistage corrigés en fonction des dépistages réalisés dans les aéroports à l’arrivée des vols internationaux.  

La correction s’applique sur l’ensemble des données postérieures à la date du 12 août.  

## 1) Qui a créé ce jeu de données ? A quelles fins ?

### a. Producteur du jeu de données : Santé Publique France
	
* Santé publique France est l’agence nationale de santé publique.  
   * Créée en mai 2016 par ordonnance et décret, c’est un établissement public administratif sous tutelle du ministère chargé de la Santé.  
   * Sa mission : améliorer et protéger la santé des populations. Cette mission s'articule autour de trois axes majeurs :  
      * Anticiper  
      * Comprendre  
      * Agir.  
* En tant qu'agence scientifique et d’expertise du champ sanitaire, Santé publique France a en charge :  
   * l'observation épidémiologique et la surveillance de l'état de santé des populations ;  
   * la veille sur les risques sanitaires menaçant les populations ;  
   * le lancement de l'alerte sanitaire ;  
   * la promotion de la santé et la réduction des risques pour la santé ;  
   * le développement de la prévention et de l'éducation pour la santé ;  
   * la préparation et la réponse aux menaces, alertes et crises sanitaires.  
	
	À partir de l’adresse <https://www.data.gouv.fr/fr/organizations/sante-publique-france/> 
	
### b. A quelles fins le jeu de données est-il créé ?

* Dans le but d'assurer un suivi quotidien de la progression de l'épidémie de Covid-19 sur le territoire afin de :  
   * Piloter la campagne (l'exploitation des données conduit à de nombreuses analyses à usage des acteurs de la gestion de crise)  
   * Informer le grand public (l'exploitation des données conduit à de nombreuses analyses publiées)  
   
### c. Chaîne de valeur du jeu de données

![Chaîne de valeur du jeu de données](https://www.santepubliquefrance.fr/var/site/storage/images/2/8/0/7/3107082-1-fre-FR/miniature_infog_covid_sidep_220721.JPG)
[Cliquer ici pour télécharger l'image en meilleure qualité](https://www.santepubliquefrance.fr/content/download/362234/3107084?version=1)


## 2) Quelles catégories sont utilisées pour le représenter ?

* Xxx  

## 3) Quels sont les usages de ce jeu de données ?

* https://www.ameli.fr/sites/default/files/vaccin-covid-mention-complete-information-personnes-concernees.pd_.pdf  
* https://www.lexpress.fr/actualite/societe/sante/cinq-questions-sur-le-fichier-de-donnees-si-vaccin-covid_2141805.html  
* Agence National du Médicament  
   * Pour surveiller et prévenir en cas de problème  
* Assurance Maladie pour organiser la suite de la campagne de vaccination  
   * Bons de vaccination selon l'âge, aux personnes à risque  
* Autres, en vrac  
   * DREES - https://drees.solidarites-sante.gouv.fr/sources-outils-et-enquetes/les-appariements-si-vic-si-dep-et-vac-si  
      * DREES-INFOS@sante.gouv.fr  
      * Presse, journalistes  


## 4) Quelles sont les limites ou les critiques rencontrées par ce jeu de données ?

* Enormément de critiques pendant la crise sur la façon de compter les cas de Covid  
* Actualité : pour dénoncer la coupe budgétaire dans le budget de la Sécurité Sociale, les biologistes __ne déclareront plus les résultats des tests Covid dans la base SI-DEP__ et ce à compter du __jeudi 27 octobre__. "Devant la surdité des pouvoirs publics, nous avons décidé de suspendre la transmission des données de dépistage sur la plateforme SI-DEP à partir du 27 octobre", a annoncé Alain Le Meur à l'AFP.  
	

## 5) Quelle réalités ces données/indicateurs sont-ils censés représenter ?

* xx  

