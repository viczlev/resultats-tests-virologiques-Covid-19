


# Données relatives aux résultats des tests virologiques COVID-19 SI-DEP

## 0) Description de la base de données
### A. Carte d'identité

* __Nom__ : Données relatives aux résultats des tests virologiques COVID-19 SI-DEP puis Données de laboratoires pour le dépistage (à compter du 18/05/2022)  
* __Où trouver le jeu de données__ : data.gouv.fr - [Données relatives aux résultats des tests virologiques COVID-19 (SI-DEP)](https://www.data.gouv.fr/fr/datasets/donnees-relatives-aux-resultats-des-tests-virologiques-covid-19/) et [Données de laboratoires pour le dépistage (A COMPTER DU 18/05/2022) - SI-DEP](https://www.data.gouv.fr/fr/datasets/donnees-de-laboratoires-pour-le-depistage-a-compter-du-18-05-2022-si-dep/)  
* __Producteur du jeu de données__ : Santé Publique France  
* __Licence__ : Licence Ouverte / Open Licence version 2.0  
* __Temporalité__ : quotidienne  
* __Date de création__ : 29 mai 2020 (la deuxième base de données améliorée est utilisée depuis le 18 mai 2022)      
* __Dernière mise à jour__ : 16 novembre 2022  
* __Granularité de la couverture territoriale__ : de la maille nationale à la maille infracommunale (quartiers IRIS de l'INSEE)  
* __Couverture territoriale__ : France  

### B. Description qualitative générale

* Durant la crise sanitaire liée à l'épidémie du COVID-19, Santé publique France se charge de surveiller et comprendre la dynamique de l'épidémie, d'anticiper les différents scénarii et de mettre en place des actions pour prévenir et limiter la transmission de ce virus sur le territoire national.
* Le __système d’information de dépistage (SI-DEP)__, en déploiement depuis le 13 mai 2020, est une plateforme sécurisée où sont systématiquement enregistrés les résultats des laboratoires des tests réalisés par l’ensemble des laboratoires de ville et établissements hospitaliers concernant le SARS-COV2.
* Le fichier SI-DEP est une base nominative qui contient les résultats des tests sérologiques et des tests RT-PCR. Elargi depuis aux tests antigéniques ainsi qu’aux autotests supervisés, son remplissage conditionne le remboursement des soignants, pharmacies et laboratoires qui réalisent les tests du Covid-19.
* Ce système d'information est encadré par l'arrêté du 16 octobre 2020 modifiant l'arrêté du 10 juillet 2020 prescrivant les mesures générales nécessaires pour faire face à l'épidémie de covid-19 dans les territoires sortis de l'état d'urgence sanitaire et dans ceux où il a été prorogé
* Le système d’information Dépistage est alimenté par les professionnels de santé réalisant les dépistages (voir en partie 2 la chaîne de valeur) 
* __Sur la base de l’exploitation des données de SI-DEP et après pseudonymisation de celles-ci, Santé Publique France publie en open data les indicateurs de progression de l'épidémie sur data.gouv, sur Geodes ainsi que sur un dashboard disponible sur le site de santé Publique France : InfoCovidFrance__  

### C. Description du jeu de données

Le jeu de données "Données de laboratoires pour le dépistage (à compter du 18/05/2022)" exploité par Santé Publique France renseigne __à différentes échelles géographiques__, à __différents échelons temporels__ et selon le sexe et la classe d'âge (voir partie 2 pour le détail) :  
* le nombre de personnes testées
* le nombre de personnes déclarées positives   
* des indicateurs clés de suivis de l'épidémie que sont le taux d'incidence, le taux de positivité et le taux de dépistage

Comme expliqué précedemment, les données ont été pseudonymisées par le système d'information avant d'être exploitées par Santé publique France.

## 1) Qui a créé ce jeu de données ? A quelles fins ?

### A. Producteur du jeu de données : Santé Publique France
	
* Santé publique France est l’agence nationale de santé publique.  
   * Créée en mai 2016 par ordonnance et décret, c’est un établissement public administratif sous tutelle du ministère chargé de la Santé.  
   * Sa mission : améliorer et protéger la santé des populations. Cette mission s'articule autour de trois axes majeurs :  
      * Anticiper  
      * Comprendre  
      * Agir  
* En tant qu'agence scientifique et d’expertise du champ sanitaire, Santé publique France a en charge :  
   * l'observation épidémiologique et la surveillance de l'état de santé des populations ;  
   * la veille sur les risques sanitaires menaçant les populations ;  
   * le lancement de l'alerte sanitaire ;  
   * la promotion de la santé et la réduction des risques pour la santé ;  
   * le développement de la prévention et de l'éducation pour la santé ;  
   * la préparation et la réponse aux menaces, alertes et crises sanitaires.  
   
	
### B. A quelles fins le jeu de données est-il créé ? Mise en contexte (crise sanitaire)

* Depuis le début de l'année 2020, la France est touchée par le virus de la Covid-19 qualifié de pandémie par l'OMS le 11 mars 2020. Aux débuts de l'épidémie, le gouvernement est dans l'incapacité de décompter exhaustivement le nombre de tests réalisés chaque semaine et par conséquent le nombre de cas de Covid identifiés. 
* Le __Système d'Information national de dépistage populationnel (SI-DEP)__ est un outil numérique mis en oeuvre dans ce contexte afin d'accompagner le déploiement des tests virologiques de dépistage du Covid 19 et répondre agilement et rapidement aux besoins de :
   * Contact-tracing
   * De surveillance de la dynamique de l’épidémie
   * D’anticipation de l’évolution de l'épidémie
   * De prévention afin de limiter la transmission du virus sur le territoire

* La plateforme SI-DEP traite et exploite les résultats des tests virologiques effectués dans toute la France, ce qui permet ensuite à __Santé Publique France__ de publier ces données qui ont servi / servent à  
   * Piloter la campagne pour les acteurs de la gestion de crise (les indicateurs de surveillance de l'évolution de la pandémie aident significativement à la détection de cluster) 
   * Informer le grand public 

* SI-DEP repose sur un partenariat entre le ministère des Solidarités et de la Santé (responsable du traitement), l’Assistance publique – Hôpitaux de Paris (AP-HP, maître d’œuvre), Santé publique France, les laboratoires de biologie médicale et leurs éditeurs de système d’information.
   
### C. Chaîne de valeur du jeu de données : depuis la collecte de la data jusqu'à la publication des indicateurs

![image](https://user-images.githubusercontent.com/115630281/202484627-4cb0487e-7b54-4d53-95eb-bd3d242d2309.png)

***Comment Santé publique France produit-elle ses indicateurs virologiques ?***


#### 1) Collecte de données auprès des professionnels de santé

* Les professionnels de santé (pharmacies, hopitaux, laboratoires, campagnes de dépistage et autres professionnels) effectuent les tests de dépistage Covid-19 auprès des patients
* Les informations du patient ainsi que les résultats des tests (RT-PCR, antigéniques et salivaires) sont ensuite saisies sur le portail SI-DEP par les professionnels de santé

#### 2) Centralisation par SI-DEP

* Le système d'information numérique SI-DEP centralise, compile et anonymise les résultats des tests 
* Ce processus est sous le conntrôle du Ministère des solidarités et de la santé ainsi que du groupe Assistance publique - Hopitaux de Paris
* Les données sont transmises entre les serveur via des flux en continu

#### 3) Traitement des données anonymisées par Santé publique France

* Collecte des données anonymisées de la veille dans la nuit
* Vérification et traitement de la base anonymisée
* Extraction et calculs
* Production d'une trentaine d'indicateurs

#### 4) Publications

* Quotidiennement :
   * Actualisation des indicateurs clés COVID-19 produits par Santé publique France sur Geodes et data.gouv.fr (à l’exception des week-end et des jours fériés depuis juin 2022)
   * Cartes d'indicateurs actualisées sur Geodes
* Chaque semaine :
   * La data recueillie par Santé publique France alimente les points épidémiologiques au niveau national et au niveau régional 
* Autres :
   * Publications scientifiques et rapports


## 2) Quelles catégories sont utilisées pour le représenter ?

* Dans un souci de simplification, nous ne détaillerons de façon précise que la composition de la base de données utilisée depuis le 18 mai 2022 "Données de laboratoires pour le dépistage (à compter du 18/05/2022)" étant donné qu'elle est une amélioration de la base de données initiale.

* Tous les jours, les données brutes collectées auprès des professionnels de santé sont retraitées après pseudonymisation afin de calculer des indicateurs complexes qui sont ensuite découpés sous forme de nombreuses agrégations géographiques et temporelles. La production des indicateurs est complexe et il est donc nécessaire que le modèle de données soit efficient pour que les objectifs de publication quotidienne de Santé publique France soient remplis. __Afin de minimiser le temps de production des indicateurs, les bases de données sont pré-agrégées selon la "définition patient" ainsi que selon différentes échelles géographiques : ce sont les tables agrégées__

* Au cours des collectes de données auprès des professionnels de santé (ie des tests de dépistage), sont collectées des données concernant 
   * les personnes dépistées (nom, prénom, âge, sexe, date de naissance, e-mail, téléphone...) 
   * le prélèvement et son origine (n° RPPS du médecin prescripteur et du médecin traitant, n° de dossier, date et heure du dépistage...)
   * le résultat du test (positif, négatif, ininterprétable, non-conforme)

__En revanche, les données sont anonymisées préalablement par SI-DEP avant d'être exploitées par Santé Publique France qui publie les indicateurs.__

Les fichiers de tables agrégées contiennent chacun :
* Une colonne pour l'échelon géographique (France, région, département, code INSEE de la commmune, code IRIS du quartier, code de l'EPCI)
* Une colonne pour le pas de temps (semaine glissante, semaine calendaire, date du jour)
* Une colonne pour les variables d'agrégation (catégorie d'âge, catégories scolaires, sexe)
* Une colonne pour les effectifs (population, patients testés positifs, nombre de patients testés)
* Une colonne pour les indicateurs calculés 
   * Taux d'incidence
   * Taux de positivité
   * Taux de dépistage
   * La classe du taux d'incidence (si applicable ie pour les fichiers IRIS, commune et EPCI)
   * La classe du taux de dépistage (si applicable ie pour les fichiers IRIS, commune et EPCI)
   * La classe du taux de positivité (si applicable ie pour les fichiers IRIS, commune et EPCI)

Par exemple :
* la table agrégée __sp_reg_7j_cage10__ contient les données SI DEP (sp) au niveau régional (reg) pour les semaines glissantes (7j) et les classes d'âge de 10 ans (cage10)
* la table agrégée __sp_fra_heb_cage_scol__ contient les données SI DEP (sp) au niveau nationale (reg) pour les semaines calendaires (heb) et les classes d'âge scolaires (cage_scol)

Remarques :
* Les valeurs manquantes sont notées < NA >
* Les données "tous âges confondus" sont identifiés par une valeur 0 dans la colonne "cl_age90"
 

## 3) Quels sont les usages de ce jeu de données ?

* https://www.lemonde.fr/les-decodeurs/article/2022/01/10/comment-fonctionne-sidep-la-base-de-donnees-qui-contient-les-resultats-des-tests-covid-19_6108907_4355770.html
* Télécharger le ppt suivant y'a plein d'infos dessus : https://www.cite-sciences.fr/fileadmin/fileadmin_CSI/fichiers/au-programme/lieux-ressources/cite-de-la-sante/_documents/JIS/Laurent_Treluyer_Journees_de_l_innovation_en_sante_3103_01042021_Universcience_sollicitation_pour_interview_ou_reportage_sur_SI-DEP.pptx

Comme nous avons vu au dessus, ce jeu de donné est fondamental dans la politique de lutte contre la COVID-19 de la France.
Ce jeu de données a été crée pour

_


## 4) Quelles sont les limites ou les critiques rencontrées par ce jeu de données ?

* https://www.lemonde.fr/les-decodeurs/article/2022/01/10/comment-fonctionne-sidep-la-base-de-donnees-qui-contient-les-resultats-des-tests-covid-19_6108907_4355770.html
* Enormément de critiques pendant la crise sur la façon de compter les cas de Covid  
* Actualisation de la base de données parfois longue --> problèmes de logistique
* Actualité : pour dénoncer la coupe budgétaire dans le budget de la Sécurité Sociale, les biologistes __ne déclareront plus les résultats des tests Covid dans la base SI-DEP__ et ce à compter du __jeudi 27 octobre__. "Devant la surdité des pouvoirs publics, nous avons décidé de suspendre la transmission des données de dépistage sur la plateforme SI-DEP à partir du 27 octobre", a annoncé Alain Le Meur à l'AFP.  
	

## 5) Quelle réalités ces données/indicateurs sont-ils censés représenter ?

* xx  

