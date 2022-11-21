


# Données relatives aux résultats des tests virologiques COVID-19 SI-DEP

# Table des matières   
0) [Introduction - Description de la base de données](#0)   
    A. [Carte d'identité](#0.A)   
    B. [Description qualitative générale](#0.B)   
    C. [Description du jeu de données](#0.C)   
1) [Qui a créé ce jeu de données ? A quelles fins ?](#1)   
    A. [Producteur du jeu de données : Santé Publique France](#1.A)   
    B. [A quelles fins le jeu de données est-il créé ? Mise en contexte (crise sanitaire)](#1.B)   
    C. [Chaîne de valeur du jeu de données : depuis la collecte de la data jusqu'à la publication des indicateurs](#1.C)   
    	i) [Collecte de données auprès des professionnels de santé](#1.C.i)   
	ii) [Centralisation par SI-DEP](#1.C.ii)   
	iii) [Traitement des données anonymisées par Santé publique France](#1.C.iii)  
	iv) [Publications](#1.C.iv)   
2) [Quelles catégories sont utilisées pour le représenter ?](#2)   
3) [Quels sont les usages de ce jeu de données ?](#3)  
4) [Quelles sont les limites ou les critiques rencontrées par ce jeu de données ?](#4)   
    A. [Incohérence statistique](#4.A)   
    B. [Le temps d’attente](#4.B)   
    C. [Une question de consentement](#4.C)   
    D. [Des "bugs" de l'outil numérique SI-DEP ont pu affecter la collecte des données brutes de dépistage](#4.D)   
    E. [Dépendance à la coopération des laboratoires](#4.E)   
5) [Quelle réalités ces données/indicateurs sont-ils censés représenter ?](#5)   
6) [Sources](#sources)   

## 0) Introduction - Description de la base de données <a name="0"></a>
### A. Carte d'identité <a name="0.A"></a>

* __Nom__ : Données relatives aux résultats des tests virologiques COVID-19 SI-DEP puis Données de laboratoires pour le dépistage (à compter du 18/05/2022)  
* __Où trouver le jeu de données__ : data.gouv.fr - [Données relatives aux résultats des tests virologiques COVID-19 (SI-DEP)](https://www.data.gouv.fr/fr/datasets/donnees-relatives-aux-resultats-des-tests-virologiques-covid-19/) et [Données de laboratoires pour le dépistage (A COMPTER DU 18/05/2022) - SI-DEP](https://www.data.gouv.fr/fr/datasets/donnees-de-laboratoires-pour-le-depistage-a-compter-du-18-05-2022-si-dep/)  
* __Producteur du jeu de données__ : Santé Publique France  
* __Licence__ : Licence Ouverte / Open Licence version 2.0  
* __Temporalité__ : quotidienne  
* __Date de création__ : 29 mai 2020 (la deuxième base de données améliorée est utilisée depuis le 18 mai 2022)      
* __Dernière mise à jour__ : 16 novembre 2022  
* __Granularité de la couverture territoriale__ : de la maille nationale à la maille infracommunale (quartiers IRIS de l'INSEE)  
* __Couverture territoriale__ : France  

### B. Description qualitative générale <a name="0.B"></a>

* Durant la crise sanitaire liée à l'épidémie du COVID-19, Santé publique France se charge de surveiller et comprendre la dynamique de l'épidémie, d'anticiper les différents scénarii et de mettre en place des actions pour prévenir et limiter la transmission de ce virus sur le territoire national.
* Le __système d’information de dépistage (SI-DEP)__, en déploiement depuis le 13 mai 2020, est une plateforme sécurisée où sont systématiquement enregistrés les résultats des laboratoires des tests réalisés par l’ensemble des laboratoires de ville et établissements hospitaliers concernant le SARS-COV2.
* Le fichier SI-DEP est une base nominative qui contient les résultats des tests sérologiques et des tests RT-PCR. Elargi depuis aux tests antigéniques ainsi qu’aux autotests supervisés, son remplissage conditionne le remboursement des soignants, pharmacies et laboratoires qui réalisent les tests du Covid-19.
* Ce système d'information est encadré par l'arrêté du 16 octobre 2020 modifiant l'arrêté du 10 juillet 2020 prescrivant les mesures générales nécessaires pour faire face à l'épidémie de covid-19 dans les territoires sortis de l'état d'urgence sanitaire et dans ceux où il a été prorogé
* Le système d’information Dépistage est alimenté par les professionnels de santé réalisant les dépistages (voir en partie 2 la chaîne de valeur) 
* __Sur la base de l’exploitation des données de SI-DEP et après pseudonymisation de celles-ci, Santé Publique France publie en open data les indicateurs de progression de l'épidémie sur data.gouv, sur Geodes ainsi que sur un dashboard disponible sur le site de santé Publique France : InfoCovidFrance__  

### C. Description du jeu de données <a name="0.C"></a>

Le jeu de données "Données de laboratoires pour le dépistage (à compter du 18/05/2022)" exploité par Santé Publique France renseigne __à différentes échelles géographiques__, à __différents échelons temporels__ et selon le sexe et la classe d'âge (voir partie 2 pour le détail) :  
* le nombre de personnes testées
* le nombre de personnes déclarées positives   
* des indicateurs clés de suivis de l'épidémie que sont le taux d'incidence, le taux de positivité et le taux de dépistage

Comme expliqué précedemment, les données ont été pseudonymisées par le système d'information avant d'être exploitées par Santé publique France.

## 1) Qui a créé ce jeu de données ? A quelles fins ? <a name="1"></a>

### A. Producteur du jeu de données : Santé Publique France <a name="1.A"></a>
	
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
   
	
### B. A quelles fins le jeu de données est-il créé ? Mise en contexte (crise sanitaire) <a name="1.B"></a>

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
   
### C. Chaîne de valeur du jeu de données : depuis la collecte de la data jusqu'à la publication des indicateurs <a name="1.C"></a>

![image](https://user-images.githubusercontent.com/115630281/202484627-4cb0487e-7b54-4d53-95eb-bd3d242d2309.png)

***Comment Santé publique France produit-elle ses indicateurs virologiques ?***


#### i) Collecte de données auprès des professionnels de santé <a name="1.C.i"></a>

* Les professionnels de santé (pharmacies, hopitaux, laboratoires, campagnes de dépistage et autres professionnels) effectuent les tests de dépistage Covid-19 auprès des patients
* Les informations du patient ainsi que les résultats des tests (RT-PCR, antigéniques et salivaires) sont ensuite saisies sur le portail SI-DEP par les professionnels de santé

#### ii) Centralisation par SI-DEP <a name="1.C.ii"></a>

* Le système d'information numérique SI-DEP centralise, compile et anonymise les résultats des tests 
* Ce processus est sous le conntrôle du Ministère des solidarités et de la santé ainsi que du groupe Assistance publique - Hopitaux de Paris
* Les données sont transmises entre les serveur via des flux en continu

#### iii) Traitement des données anonymisées par Santé publique France <a name="1.C.iii"></a>

* Collecte des données anonymisées de la veille dans la nuit
* Vérification et traitement de la base anonymisée
* Extraction et calculs
* Production d'une trentaine d'indicateurs

#### iv) Publications <a name="1.C.iv"></a>

* Quotidiennement :
   * Actualisation des indicateurs clés COVID-19 produits par Santé publique France sur Geodes et data.gouv.fr (à l’exception des week-end et des jours fériés depuis juin 2022)
   * Cartes d'indicateurs actualisées sur Geodes
* Chaque semaine :
   * La data recueillie par Santé publique France alimente les points épidémiologiques au niveau national et au niveau régional 
* Autres :
   * Publications scientifiques et rapports


## 2) Quelles catégories sont utilisées pour le représenter ? <a name="2"></a>

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
 

## 3) Quels sont les usages de ce jeu de données ? <a name="3"></a>

--> partie à revoir car trop de redites avec la partie précédente. pas besoin de donner les raisons de création de la base de données ni les catégories car ce sont des parties précédentes !! En revanche, il faut expliciter l'usage final des bases de données : quelles publications, dans quels buts, à quelle fréquence, utilisés par qui...


Comme expliqué précedemment, ce jeu de donné est fondamental dans la politique de lutte contre la COVID-19 de la France.

Ce jeu de données a été crée en priorité pour
* Répondre aux besoins de contact-tracing
* Surveiller la dynamique de l'épidémie
* Prévenir et limiter la transmission du virus sur le territoire français
* Transmettre les résultats au plus vite pour mettre en oeuvre les mesures de prévention adaptées

SI-DEP est très efficace et atteint ses objectifs en catégorisant clairement ses données dans les catégories suivantes
1. Données concernant la personne dépistée (nom, date de naissance, téléphone, adresse mail et postale...)

2. Données concernant le prévelement et son origine (numéro du dossier ou de prélèvement, date et heure du prélèvement, identifiant national, numéro RPPS du prescripteur et médecin traitant...)

3. Données concernant le résultat du test (code de l'analyse, résultat de l'analyse positif ou négatif...)

Ces données permettent au Ministère de la Santé de calculer des indicateurs et des statistiques sur la situation de la pandémie en France, et la santé des français. Utilisés par les médias pour relayer les informations de manière plus synthétique et compréhensible pour le grand public - vous avez certainement entendu parler de certains de ces indicateurs tel le
* Taux d'incidence : nombre de personne positifs ramené à la population française (pour 100 000 habitants), cela peut être calculé au niveau nationale, régionale ou départemental notamment pour pouvoir voir les différences entre les parties du territoire

* Taux de positivité : le nombre de personnes positives parmis le nombre de personnes testées - cela nous permet de pouvoir tirer des conclusions sur les tendances sur le dépistage et la fréquence d'un résultat positif

* Taux de dépistage : le nombre de tests dont le résultat est exploitable, le positif ou le négatif, rapporté à la population française pour 100 000 habitants. Encore une fois, cela peut être calculé au niveau nationale, régionale ou départementale pour pouvoir faire des comparaisons sur l'ensemble du territoire

De plus, ces indicateurs pevent être déclinés pour une période de temps précise. Cela permet de pouvoir analyser en profondeur et de manière pointue les statistiques liées au COVID-19 en France. Bien evidemment, il faut se rappeler que ces indicateurs sont utilisés par le gouvernement et les services de santé dans un but de savoir, mais aussi potentiellement dans un but politique. Pouvoir relayer un certain message politique, quel qu'il soit, est grandement facilité par la création de ce jeu de données - il est évident que nous avons tous entendus parler des ces indicateurs dans les médias, détournés par tous les bords politiques !


## 4) Quelles sont les limites ou les critiques rencontrées par ce jeu de données ? <a name="4"></a>

Les données de laboratoires relatives au dépistage des résultats des tests virologiques COVID-19 SI-DEP (le service intégré de dépistage et de prévention) font face à de nombreuses limites :

### A. Incohérence statistique <a name="4.A"></a>

* La somme des tests indiqués pour chaque départements ou régions françaises est inférieure au nombre de tests indiqué pour la France représentant ainsi une incohérence majeure.

* En effet, les fiches médicales de chaque patient ayant reçu un test virologique/dépistage étaient parfois incomplètes; le lieu de résidence de chaque personne n’a pas toujours été enregistré par le système SIDEP.

* De ce fait, certains individus dont le département de résidence n’avait pas pu être localisé, avaient été comptabilisés au niveau de la France entière. Pour les personnes dont le département de résidence était connu, ceux-ci ont été fidèlement représentés sur les cartes. 

* Il est difficile de suivre l’évolution de la pandémie avec des données incohérents et contradictoires. Le manque de précision épidémiologique dû aux fiches de tests incomplètes doit être suivis de prêt. Advenant une flambée de cas de dépistage positif dans l’Ouest de la France, les personnes dont la résidence est inconnue pourraient faire basculer la France entière dans un pallier d’alerte plus élevé. 

### B. Le temps d’attente <a name="4.B"></a>

Selon les études menés pas xx, la base de données n’est pas appréciée de ces utilisateurs dû à certains de ses fléaux. 
( à développer) 

### C. Une question de consentement <a name="4.C"></a>

* Le recueillement des données transmit à la SIDEP débute très souvent chez le médecin généraliste.  Un professionnel de la santé par l’intermédiaire de sa plateforme numérique médicale Amelipro, peut ordonner si jugé nécessaire, la prescription d’un dépistage de covid-19. Bien que cette action ne soit pas malveillante, elle peut déclencher une série de répercussions qui nous pousse à réfléchir sur l’importance du consentement du patient. 

* En effet, un médecin peut prescrire un dépistage de COVID-19 sans le consentement d’un patient. Sur sa plateforme médicale, le professionnel est aussi invité à renseigner les coordonnées des cas-contacts de son patient. 

* Sous le contexte de la pandémie mondiale, un médecin est autorisé à violer le secret professionnel (C. pén., art. 226-13) par un nouveau cas de dérogation prévu par l’article 11 de la loi n° 2020-546 du 11 mai 2020 prorogeant l’état d’urgence sanitaire. Lorsque celui-ci dévoile le « statut covid-19 » de son patient à un tiers il divulgue non seulement des données à caractère personnel de celui-ci mais également ceux de son entourage. Il faut également noter que les patients n’ont pas le droit de refuser la transmission de leurs données de santés.

* De plus, la prescription du test de COVID par le médecin, engendre l’obligation de la saisie des données personnelles des personnes dépistés dans la base de données SIDEP. Dans le cas où un patient est positif, le contact-tracing sera enclenché et une alerte passe sur le fichier contact COVID pour initier une enquête auprès des cas-contacts.

* Les fichiers SIDEP est nécessaire pour surveiller la propagation du virus. Néanmoins, son déploiement convoque de nombreuses parties, en dépit du consentement du patient. Les utilisateurs multiples de cette base de données ont à confronter de nombreux dilemmes dont la cyber-sécurité et la divulgation de données personnelles.

### D. Des "bugs" de l'outil numérique SI-DEP ont pu affecter la collecte des données brutes de dépistage <a name="4.D"></a>

* On peut observer sur le graphique ci-dessous issu du dernier rapport hebdomadaire de Santé publique France sur l'évolution du Covid-19 en France datant du 16 novembre 2022 que le taux de tests de dépistage (courbes bleues) a pu être très important à certains moments de l'épidémie.

<img width="547" alt="image" src="https://user-images.githubusercontent.com/115630281/202933247-e39fa3b5-0481-43d9-8d1e-8d73719937b3.png">

* Des ralentissements voire même des bugs ont pu être observés par des professionnels de santé au moment de saisir les données des tests virulogiques, notamment en fin de journée. Par exemple à la fin 2021 et au début 2022, le nombre de tests réalisés était très important (plus de 7 millions lors de la semaine de Noël 2021) et les pharmaciens ont pu constater de nombreux bugs à ce moment-là, liés à la saturation des serveurs. D'après la DGS (direction générale de la santé), "ce n'est pas le "nombre de tests réalisé par jour" qui pose problème mais la "concentration sur une plage donnée" qui provoque la saturation du système.

> « Le système sature car il n'est pas calibré pour recevoir autant de résultats tests »   
*Propos déclarés par Gilles Bonnefond, porte-parole de l'Union des syndicats des pharmaciens d'officine et rapportés par Le Figaro dans un article du 5 janvier 2022*

* Ces dysfonctionnements de la plateforme SI-DEP sont agaçants pour le personnel qui réalise ces tests et cela affecte donc leur opinion vis-à-vis du système SI-DEP et rend pénible leur travail de saisie de données des tests. En effet, une solution pour éviter les saturations du système serait de déconcentrer la saisie des données brutes dans le systèmes et de l'étaler tout au long de la journée plutôt que de saisir une masse de données importantes en fin de journée et ainsi saturer le système à ses "heures de pointes". On comprend alors que ces personnes ne soient pas enjouées à l'idée de transmettre les données via SI-DEP car non seulement cela représente un travail en plus mais cela peut également être pénible lorsque des bugs sont rencontrés.

> « Nous pouvons concevoir qu'il soit impossible d'éviter des bugs, mais cela arrive trop fréquemment»   
*Propos déclarés par Philippe Besset, président de la Fédération des syndicats pharmaceutiques de France (FSPF) et rapportés par Le Figaro dans un article du 5 janvier 2022*

### E. Dépendance à la coopération des laboratoires <a name="4.E"></a>

* Les fichiers de la base de données SI-DEP sont alimentés en premier lieu par les professionnels de santé qui réalisent les tests virulogiques, et notamment par les laboratoires. De fait, le fichier SI-DEP nécessite la bonne volonté et la coopération des laboratoires pour que les données soient remontées et publiées et donc que le suivi de l'épidémie puisse se faire dans les meilleures conditions.
* Cependant, depuis le 26 octobre 2022, __certains laboratoires de biologie libéraux ont décidé de cesser d'alimenter la base de données SI-DEP__ en protestation à une baisse de leurs tarifs prévue dans le projet de loi de financement de la Sécurité Sociale. 

> « Devant la surdité des pouvoirs publics, nous avons décidé de suspendre la transmission des données de dépistage sur la plate-forme SI-Dep à partir du 27 octobre »   
*Propos déclarés par Alain Le Meur, le président de l’Alliance pour la biologie médicale, à l'AFP et rapportés par le Monde dans un article du 26 octobre 2022*

* Les mouvements de pression des laboratoires qui plaident leur cause auprès du gouvernement contribue à __gêner l'alimentation de la base de données SI-DEP__ et cela __entrave donc le bon suivi de l'épidémie par Santé publique France__. Les chiffres proposés au grand public ne refètent donc pas la vérité depuis le 26 octobre. La DREES a en effet expliqué dans un communiqué de presse datant du 3 novembre 2022 que "le vendredi 28 octobre, le nombre de tests RT-PCR remontés dans SI-Dep par les laboratoires du secteur privé était 81 % inférieur au niveau observé le vendredi précédent".

* Cette baisse du nombre de dépistage liée à la mobilisation des laboratoires privés __a pour conséquence de rendre non-interprétable le taux d'incidence calculé par Santé publique France__. Afin de conserver un regard sur l'évolution de l'épidémie, Santé publique France continue néanmoins de calculer les indicateurs à partir des tests antigéniques réalisés en  pharmacie et qui représentent plus de la moitié des tests réalisés en France. La base de données a donc été fortement affaiblie par l'arrêt d'alimention de la base de données par de nombreux laboratoires et cela limite la significativité des indicateurs calculés. Antoine Flahaut, directeur de l’Institut de santé globale et épidémiologiste va même plus loin en affirmant que les statistiques ont été rendu vaines à cause de la grève des biologistes.

<img width="415" alt="image" src="https://user-images.githubusercontent.com/115630281/202932338-b65815b7-5b90-4d42-9f97-96dedd2c80e0.png">


* __En somme, on comprend donc que le bon fonctionnement de la base de données est dépendant de la bonne volonté des professionnels de santé et de leur capacité à fournir les données brutes qui servent à calculer des indicateurs pertinents et suffisamment significatifs.__

### Critique de la méthodologie

* La méthodologie utilisée pour suivre l'épidémie de Covid-19 est également fortement critiquée et souvent comparée à la méthodologie adoptée par d'autres pays. En effet, avec des méthodologies plus ou moins différentes, les données recueillies dans la base de données ne seront pas les mêmes et certains spécialistes font l'hypothèse que certaines méthodologies permettent d'obtenir des données plus significatives qu'avec un recours à une méthodologie différente.

* Par exemple, Antoine Flahaut (épidémiologiste et directeur de l'Institut de santé globale) déplore que la France n'ait pas suivi une méthodologie similaire à la méthodologie anglosaxonne qui consiste à effectuer un sondage hebdomadaire auprès d'un échantillon représentatif de la population afin de mieux se rendre compte de l'évolution de l'épidémie.

<img width="426" alt="image" src="https://user-images.githubusercontent.com/115630281/202932363-d474e21e-474e-4cb9-b74d-fd4b420f6fca.png">


## 5) Quelle réalités ces données/indicateurs sont-ils censés représenter ? <a name="5"></a>

* xx  

## Sources <a name="sources"></a>
* data.gouv.fr
* santepubliquefrance.fr - [Chiffres clés et évolution de la COVID-10 en France et dans le monde](https://www.santepubliquefrance.fr/dossiers/coronavirus-covid-19/coronavirus-chiffres-cles-et-evolution-de-la-covid-19-en-france-et-dans-le-monde)
* solidarites-sante.gouv.fr - [Contact-COVID et SI-DEP, les outils numériques du dépistage Covid-19](https://solidarites-sante.gouv.fr/soins-et-maladies/maladies/maladies-infectieuses/coronavirus/tout-savoir-sur-le-covid-19/article/contact-covid-et-si-dep-les-outils-numeriques-du-depistage-covid-19)

* SANCHEZ, "Budget de la « Sécu » : les laboratoires d’analyse menacent de cesser la transmission des données des tests de dépistage du Covid-19", *Le Monde*, 26 octobre 2022 ; [lien](https://www.lemonde.fr/societe/article/2022/10/26/budget-de-la-secu-les-laboratoires-d-analyse-menacent-de-cesser-la-transmission-des-donnees-des-tests-de-depistage-du-covid-19_6147347_3224.html)
* SANCHEZ, "Covid-19 : le bras de fer entre les laboratoires d’analyse et le gouvernement perturbe le suivi de l’épidémie", *Le Monde*, 14 novembre 2022 ; [lien](https://www.lemonde.fr/les-decodeurs/article/2022/11/14/covid-19-le-bras-de-fer-entre-les-laboratoires-d-analyse-et-le-gouvernement-perturbe-le-suivi-de-l-epidemie_6149857_4355770.html)
* ZORN, "État d’urgence pour les données de santé (II) : sidep et contact covid", Dalloz, 26 mai 2020, [lien](https://www.dalloz-actualite.fr/flash/etat-d-urgence-pour-donnees-de-sante-ii-sidep-et-contact-covid#.Y3p04OzMKgQ!%5Bimage%5D(https://user-images.githubusercontent.com/118362232/202925405-f6728590-7dc1-4e98-b5c2-8792597188ad.png)
* SANCHEZ, "Covid-19 : la plate-forme SI-Dep, qui contient les résultats des tests de dépistage, rencontre des pannes", *Le Monde*, 5 avril 2022, [lien](https://www.lemonde.fr/les-decodeurs/article/2022/04/05/covid-19-la-plate-forme-si-dep-qui-contient-les-resultats-des-tests-de-depistage-rencontre-des-pannes_6120743_4355770.html)
* VAZQUEZ, "Tests Covid : les ralentissements de la plateforme SIDEP agacent les pharmaciens", *Le Figaro*, 5 janvier 2022, [lien](https://www.lefigaro.fr/economie/tests-covid-les-ralentissements-de-la-plateforme-sidep-agacent-les-pharmaciens-20220105)


