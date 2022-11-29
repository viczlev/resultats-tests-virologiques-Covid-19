


# Données relatives aux résultats des tests virologiques COVID-19 SI-DEP

Nous présentons les résultats de notre enquête collective menée en novembre 2022 sur la base de données de Santé publique France relative aux résultats des tests virologiques Covid-19 en France.   

L'enquête est réalisée par Aliette de Cacqueray, Anaïs des Rosiers et Victoire Leveilley.


![image](https://user-images.githubusercontent.com/115630281/203543220-41b1f794-6566-4efb-b087-697f2ab655e9.png)



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


6) [Entretien avec un data scientist travaillant chez Santé publique France](#6)


7) [Sources](#sources)   

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

Durant la crise sanitaire liée à l'épidémie du COVID-19, Santé publique France se charge de surveiller et comprendre la dynamique de l'épidémie, d'anticiper les différents scénarii et de mettre en place des actions pour prévenir et limiter la transmission de ce virus sur le territoire national.

Le __système d’information de dépistage (SI-DEP)__, en déploiement depuis le 13 mai 2020, est une plateforme sécurisée où sont systématiquement enregistrés les résultats des laboratoires des tests réalisés par l’ensemble des laboratoires de ville et établissements hospitaliers concernant le SARS-COV2. Le fichier SI-DEP est une base nominative qui contient les résultats des tests sérologiques et des tests RT-PCR. Elargi depuis aux tests antigéniques ainsi qu’aux autotests supervisés, son remplissage conditionne le remboursement des soignants, pharmacies et laboratoires qui réalisent les tests du Covid-19. Le système d’information Dépistage est alimenté par les professionnels de santé réalisant les dépistages (voir en partie 2 la chaîne de valeur).

Ce système d'information est encadré par l'arrêté du 16 octobre 2020 modifiant l'arrêté du 10 juillet 2020 prescrivant les mesures générales nécessaires pour faire face à l'épidémie de covid-19 dans les territoires sortis de l'état d'urgence sanitaire et dans ceux où il a été prorogé

__Sur la base de l’exploitation des données de SI-DEP et après pseudonymisation de celles-ci, Santé Publique France publie en open data les indicateurs de progression de l'épidémie sur data.gouv, sur Geodes ainsi que sur un dashboard disponible sur le site de santé Publique France : InfoCovidFrance__  

### C. Description du jeu de données <a name="0.C"></a>

Le jeu de données "Données de laboratoires pour le dépistage (à compter du 18/05/2022)" exploité par Santé Publique France renseigne __à différentes échelles géographiques__, à __différents échelons temporels__ et selon le sexe et la classe d'âge (voir partie 2 pour le détail) :  
* le nombre de personnes testées
* le nombre de personnes déclarées positives   
* des indicateurs clés de suivis de l'épidémie que sont le taux d'incidence, le taux de positivité et le taux de dépistage

Comme expliqué précedemment, les données ont été pseudonymisées par le système d'information avant d'être exploitées par Santé publique France.

## 1) Qui a créé ce jeu de données ? A quelles fins ? <a name="1"></a>

### A. Producteur du jeu de données : Santé Publique France <a name="1.A"></a>
	
Santé publique France est l’agence nationale de santé publique. Créée en mai 2016 par ordonnance et décret, c’est un établissement public administratif sous tutelle du ministère chargé de la Santé. Sa mission est d'améliorer et protéger la santé des populations. Cette mission s'articule autour de trois axes majeurs :  
* Anticiper  
* Comprendre  
* Agir   

En tant qu'agence scientifique et d’expertise du champ sanitaire, Santé publique France a en charge :  
* l'observation épidémiologique et la surveillance de l'état de santé des populations ;  
* la veille sur les risques sanitaires menaçant les populations ;  
* le lancement de l'alerte sanitaire ;  
* la promotion de la santé et la réduction des risques pour la santé ;  
* le développement de la prévention et de l'éducation pour la santé ;  
* la préparation et la réponse aux menaces, alertes et crises sanitaires.  
   
	
### B. A quelles fins le jeu de données est-il créé ? Mise en contexte (crise sanitaire) <a name="1.B"></a>

Depuis le début de l'année 2020, la France est touchée par le virus de la Covid-19 qualifié de pandémie par l'OMS le 11 mars 2020. Aux débuts de l'épidémie, le gouvernement est dans l'incapacité de décompter exhaustivement le nombre de tests réalisés chaque semaine et par conséquent le nombre de cas de Covid identifiés. 

Le __Système d'Information national de dépistage populationnel (SI-DEP)__ est un outil numérique mis en oeuvre dans ce contexte afin d'accompagner le déploiement des tests virologiques de dépistage du Covid 19 et répondre agilement et rapidement aux besoins de :
   * Contact-tracing
   * De surveillance de la dynamique de l’épidémie
   * D’anticipation de l’évolution de l'épidémie
   * De prévention afin de limiter la transmission du virus sur le territoire

La plateforme SI-DEP traite et exploite les résultats des tests virologiques effectués dans toute la France, ce qui permet ensuite à __Santé Publique France__ de publier ces données qui ont servi / servent à  
   * Piloter la campagne pour les acteurs de la gestion de crise (les indicateurs de surveillance de l'évolution de la pandémie aident significativement à la détection de cluster) 
   * Informer le grand public 

SI-DEP repose sur un partenariat entre le ministère des Solidarités et de la Santé (responsable du traitement), l’Assistance publique – Hôpitaux de Paris (AP-HP, maître d’œuvre), Santé publique France, les laboratoires de biologie médicale et leurs éditeurs de système d’information.
   
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

C.f. Partie 3

## 2) Quelles catégories sont utilisées pour le représenter ? <a name="2"></a>

Dans un souci de simplification, nous ne détaillerons de façon précise que la composition de la base de données utilisée depuis le 18 mai 2022 "Données de laboratoires pour le dépistage (à compter du 18/05/2022)" étant donné qu'elle est une amélioration de la base de données initiale.

Tous les jours, les données brutes collectées auprès des professionnels de santé sont retraitées après pseudonymisation afin de calculer des indicateurs complexes qui sont ensuite découpés sous forme de nombreuses agrégations géographiques et temporelles. La production des indicateurs est complexe et il est donc nécessaire que le modèle de données soit efficient pour que les objectifs de publication quotidienne de Santé publique France soient remplis. __Afin de minimiser le temps de production des indicateurs, les bases de données sont pré-agrégées selon la "définition patient" ainsi que selon différentes échelles géographiques : ce sont les tables agrégées__

Au cours des collectes de données auprès des professionnels de santé (ie des tests de dépistage), sont collectées des données concernant 
   1. Les personnes dépistées (nom, prénom, âge, sexe, date de naissance, e-mail, téléphone...) 
   
   2. Le prélèvement et son origine (n° RPPS du médecin prescripteur et du médecin traitant, n° de dossier, date et heure du dépistage...)
   
   3. Le résultat du test (positif, négatif, ininterprétable, non-conforme)


__En revanche, les données sont anonymisées préalablement par SI-DEP avant d'être exploitées par Santé Publique France qui publie les indicateurs.__

Les fichiers de tables agrégées contiennent chacun :
* Une colonne pour l'échelon géographique (France, région, département, code INSEE de la commmune, code IRIS du quartier, code de l'EPCI)
* Une colonne pour le pas de temps (semaine glissante, semaine calendaire, date du jour)
* Une colonne pour les variables d'agrégation (catégorie d'âge, catégories scolaires, sexe)
* Une colonne pour les effectifs (population, patients testés positifs, nombre de patients testés)
* Une colonne pour les indicateurs calculés 
   * Taux d'incidence : nombre de personne positifs ramené à la population française (pour 100 000 habitants), cela peut être calculé au niveau nationale, régionale ou départemental notamment pour pouvoir voir les différences entre les parties du territoire
   
   * Taux de positivité : le nombre de personnes positives parmis le nombre de personnes testées - cela nous permet de pouvoir tirer des conclusions sur les tendances sur le dépistage et la fréquence d'un résultat positif
   
   * Taux de dépistage :le nombre de tests dont le résultat est exploitable, le positif ou le négatif, rapporté à la population française pour 100 000 habitants. Encore une fois, cela peut être calculé au niveau nationale, régionale ou départementale pour pouvoir faire des comparaisons sur l'ensemble du territoire

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


Comme expliqué précedemment, ce jeu de donné est fondamental dans la politique de lutte contre la COVID-19 de la France. Les données présentes permettent au Ministère de la Santé de calculer des indicateurs et des statistiques sur la situation de la pandémie en France, et la santé des français. Utilisés par les médias pour relayer les informations de manière plus synthétique et compréhensible pour le grand public - vous avez certainement entendu parler de certains de ces indicateurs tel que le taux de positivité ou encore le taux de dépistage.

En plus d'être décliné pour des personnes précises et décliné dans une délimitation géographique, ces indicateurs pevent être déclinés pour une période de temps précise. Cela permet de pouvoir analyser en profondeur et de manière pointue les statistiques liées au COVID-19 en France. Bien evidemment, il faut se rappeler que ces indicateurs sont utilisés par le gouvernement et les services de santé dans un but de savoir, mais aussi potentiellement dans un but politique. Pouvoir relayer un certain message politique, quel qu'il soit, est grandement facilité par la création de ce jeu de données - il est évident que nous avons tous entendus parler des ces indicateurs dans les médias, détournés par tous les bords politiques ! La data peut sembler objectif, par sa nature mathématique et factuelle, hors, en réalité, différents acteurs peuvent s'emparer de la data afin de relayer un message ou mettre en évidence une tendance. 

Les acteurs principaux qui ont usage de ce jeu de données sont:

1. Santé Publique France - l'agence nationale de santé publique qui a pour mission d'améliorer et de protéger la santé des populations, elle est sous la tutelle du Minsitère chargé de la Santé. Santé Publique France publie et actualise les indicateurs clées liés au COVID-19 en France depuis le début de la pandémie (taux de dépistage, taux de positivité, quantité de cas confirmés, pourcentage d'évolution depuis la dernière semaine, mois..). Ils se chargent d'actualiser ces indicateurs quotidiennement, à l'exception des weekend et des jours feriés. Ces indicateurs sont très importants pour le grand public et pour d'autres organismes européens et internationaux qui voudraient suivre l'évolution de la pandémie dans d'autres pays pour pouvoir potentiellement réagir. Ces indicateurs sont également traduits par des cartes sur le site Geodes pour pouvoir montrer la data de manière plus visuelle est pédagogique. 

2. Organismes politiques divers - alimenté par la data et les indicateurs publiés par Santé Publique France, d'autres organismes politiques, tel le gouvernement français, le ministère des affaires étrangères ou encore le ministère de la santé utilisent la data de ce jeu de données pour pouvoir créer des politiques publiques cohérentes avec les statistiques. Il est primordial de pouvoir expliquer ces actions politiques, et qu'ils soient ancrés dans de la data concrète.

3. La presse - voici on nous avons certaines divergences. La presse n'est bien évidemment pas neutre, elle est de tout bord politique. La gestion de la crise de la COVID-19 a été extrêmement crtiquée par des populations diverses, d'opinions divergentes. Voilà le rôle joué par la presse. S'emparant de cette base de données et des statistiques et indicateurs qui en découlent, la presse peut les présenter dans ses publications sous de diverses lumières afin de souligner certains sujets qui leur tiennent à coeur et qui résonnent avec leurs lecteurs.



## 4) Quelles sont les limites ou les critiques rencontrées par ce jeu de données ? <a name="4"></a>


### A. Incohérence statistique <a name="4.A"></a>

Les données de laboratoires relatives au dépistage des résultats des tests virologiques COVID-19 SI-DEP (le service intégré de dépistage et de prévention) font face à de nombreuses limites: Actuellemnt en France, la somme des tests indiqués pour chaque départements ou régions françaises est inférieure au nombre de tests indiqué pour la France représentant ainsi une incohérence majeure.En effet, les fiches médicales de chaque patient ayant reçu un test virologique/dépistage étaient parfois incomplètes; le lieu de résidence de chaque personne n’a pas toujours été enregistré par le système SIDEP.

De ce fait, certains individus dont le département de résidence n’avait pas pu être localisé, avaient été comptabilisés au niveau de la France entière. Pour les personnes dont le département de résidence était connu, ceux-ci ont été fidèlement représentés sur les cartes. 

Il est difficile de suivre l’évolution de la pandémie avec des données incohérents et contradictoires. Le manque de précision épidémiologique dû aux fiches de tests incomplètes doit être suivis de prêt. Advenant une flambée de cas de dépistage positif dans l’Ouest de la France, les personnes dont la résidence est inconnue pourraient faire basculer la France entière dans un pallier d’alerte plus élevé. 

### B. Le temps d’attente <a name="4.B"></a>

Lors d’une très forte hausse du nombre de cas, la plateforme SI-DEP fait face à une grande pression. Depuis novembre 2022, les dépistages de COVID sont en forte hausse. Sous la montée fulgurante des tests l’infrastructure technique subit des ralentissements importants. Lors de certaines « heures de pointe » l’interface surcharge dû aux nombres trop importants de saisie sur une courte période. La direction générale de la santé (DGS) stipule que les incidents sont souvent provoqués par des tentatives d’attaque en déni de service (DDOS) qui envoient des connexions simultanées vers le système provoquant un arrêt de service.
Il est important de noter que c’est n’est pas la première fois que des incidents surviennent. En août 2022, à deux reprises pendant plusieurs heures les professionnels de la santé ne pouvaient pas rentrer les résultats de test antigénique sur la plateforme Si-Dep. Ce problème a empêché à plusieurs patients vaccinés de récupérer leur passe sanitaire, provoquant ainsi leur accès à des lieux nécessitant une passe sanitaire. 


### C. La question des données personnelles <a name="4.C"></a>

Le recueillement des données transmit à la SIDEP débute très souvent chez le médecin généraliste.  Un professionnel de la santé par l’intermédiaire de sa plateforme numérique médicale Amelipro, peut ordonner si jugé nécessaire, la prescription d’un dépistage de covid-19. Bien que cette action ne soit pas malveillante, elle peut déclencher une série de répercussions qui nous pousse à réfléchir sur l’importance du consentement du patient. 

En effet, un médecin peut prescrire un dépistage de COVID-19 sans le consentement d’un patient. Sur sa plateforme médicale, le professionnel est aussi invité à renseigner les coordonnées des cas-contacts de son patient. 

Sous le contexte de la pandémie mondiale, un médecin est autorisé à violer le secret professionnel (C. pén., art. 226-13) par un nouveau cas de dérogation prévu par l’article 11 de la loi n° 2020-546 du 11 mai 2020 prorogeant l’état d’urgence sanitaire. Lorsque celui-ci dévoile le « statut covid-19 » de son patient à un tiers il divulgue non seulement des données à caractère personnel de celui-ci mais également ceux de son entourage. Il faut également noter que les patients n’ont pas le droit de refuser la transmission de leurs données de santés.

De plus, la prescription du test de COVID par le médecin, engendre l’obligation de la saisie des données personnelles des personnes dépistés dans la base de données SIDEP. Dans le cas où un patient est positif, le contact-tracing sera enclenché et une alerte passe sur le fichier contact COVID pour initier une enquête auprès des cas-contacts.

Les fichiers SIDEP est nécessaire pour surveiller la propagation du virus. Néanmoins, son déploiement convoque de nombreuses parties, en dépit du consentement du patient. Les utilisateurs multiples de cette base de données ont à confronter de nombreux dilemmes dont la cyber-sécurité et la divulgation de données personnelles.

De plus, les données collectées lors des tests peuvent avoir à affronter quelques problèmes de sécurité. L’élargissement du dépistage et la forte hausse de l’utilisation de plateforme vulnérabilisent les données de plusieurs Français. En effet, en octobre 2021 une fuite massive de résultats de tests antigéniques a eu lieu : plus de 700 000 résultats de tests et de données personnelles étaient accessibles dus à une faille sur le site de Francetest.

### D. Des "bugs" de l'outil numérique SI-DEP ont pu affecter la collecte des données brutes de dépistage <a name="4.D"></a>

On peut observer sur le graphique ci-dessous issu du dernier rapport hebdomadaire de Santé publique France sur l'évolution du Covid-19 en France datant du 16 novembre 2022 que le taux de tests de dépistage (courbes bleues) a pu être très important à certains moments de l'épidémie.

<img width="547" alt="image" src="https://user-images.githubusercontent.com/115630281/202933247-e39fa3b5-0481-43d9-8d1e-8d73719937b3.png">

Des ralentissements voire même des bugs ont pu être observés par des professionnels de santé au moment de saisir les données des tests virulogiques, notamment en fin de journée. Par exemple à la fin 2021 et au début 2022, le nombre de tests réalisés était très important (plus de 7 millions lors de la semaine de Noël 2021) et les pharmaciens ont pu constater de nombreux bugs à ce moment-là, liés à la saturation des serveurs. D'après la DGS (direction générale de la santé), "ce n'est pas le "nombre de tests réalisé par jour" qui pose problème mais la "concentration sur une plage donnée" qui provoque la saturation du système.

> « Le système sature car il n'est pas calibré pour recevoir autant de résultats tests »   
*Propos déclarés par Gilles Bonnefond, porte-parole de l'Union des syndicats des pharmaciens d'officine et rapportés par Le Figaro dans un article du 5 janvier 2022*

Ces dysfonctionnements de la plateforme SI-DEP sont agaçants pour le personnel qui réalise ces tests et cela affecte donc leur opinion vis-à-vis du système SI-DEP et rend pénible leur travail de saisie de données des tests. En effet, une solution pour éviter les saturations du système serait de déconcentrer la saisie des données brutes dans le systèmes et de l'étaler tout au long de la journée plutôt que de saisir une masse de données importantes en fin de journée et ainsi saturer le système à ses "heures de pointes". On comprend alors que ces personnes ne soient pas enjouées à l'idée de transmettre les données via SI-DEP car non seulement cela représente un travail en plus mais cela peut également être pénible lorsque des bugs sont rencontrés.

> « Nous pouvons concevoir qu'il soit impossible d'éviter des bugs, mais cela arrive trop fréquemment»   
*Propos déclarés par Philippe Besset, président de la Fédération des syndicats pharmaceutiques de France (FSPF) et rapportés par Le Figaro dans un article du 5 janvier 2022*

### E. Dépendance à la coopération des laboratoires <a name="4.E"></a>

Les fichiers de la base de données SI-DEP sont alimentés en premier lieu par les professionnels de santé qui réalisent les tests virulogiques, et notamment par les laboratoires. De fait, le fichier SI-DEP nécessite la bonne volonté et la coopération des laboratoires pour que les données soient remontées et publiées et donc que le suivi de l'épidémie puisse se faire dans les meilleures conditions.

Cependant, depuis le 26 octobre 2022, __certains laboratoires de biologie libéraux ont décidé de cesser d'alimenter la base de données SI-DEP__ en protestation à une baisse de leurs tarifs prévue dans le projet de loi de financement de la Sécurité Sociale. 

> « Devant la surdité des pouvoirs publics, nous avons décidé de suspendre la transmission des données de dépistage sur la plate-forme SI-Dep à partir du 27 octobre »   
*Propos déclarés par Alain Le Meur, le président de l’Alliance pour la biologie médicale, à l'AFP et rapportés par le Monde dans un article du 26 octobre 2022*

Les mouvements de pression des laboratoires qui plaident leur cause auprès du gouvernement contribue à __gêner l'alimentation de la base de données SI-DEP__ et cela __entrave donc le bon suivi de l'épidémie par Santé publique France__. Les chiffres proposés au grand public ne refètent donc pas la vérité depuis le 26 octobre. La DREES a en effet expliqué dans un communiqué de presse datant du 3 novembre 2022 que "le vendredi 28 octobre, le nombre de tests RT-PCR remontés dans SI-Dep par les laboratoires du secteur privé était 81 % inférieur au niveau observé le vendredi précédent".

Cette baisse du nombre de dépistage liée à la mobilisation des laboratoires privés __a pour conséquence de rendre non-interprétable le taux d'incidence calculé par Santé publique France__. Afin de conserver un regard sur l'évolution de l'épidémie, Santé publique France continue néanmoins de calculer les indicateurs à partir des tests antigéniques réalisés en  pharmacie et qui représentent plus de la moitié des tests réalisés en France. La base de données a donc été fortement affaiblie par l'arrêt d'alimention de la base de données par de nombreux laboratoires et cela limite la significativité des indicateurs calculés. Antoine Flahaut, directeur de l’Institut de santé globale et épidémiologiste va même plus loin en affirmant que les statistiques ont été rendu vaines à cause de la grève des biologistes.

<img width="415" alt="image" src="https://user-images.githubusercontent.com/115630281/202932338-b65815b7-5b90-4d42-9f97-96dedd2c80e0.png">


__En somme, on comprend donc que le bon fonctionnement de la base de données est dépendant de la bonne volonté des professionnels de santé et de leur capacité à fournir les données brutes qui servent à calculer des indicateurs pertinents et suffisamment significatifs.__

### Critique de la méthodologie

La méthodologie utilisée pour suivre l'épidémie de Covid-19 est également fortement critiquée et souvent comparée à la méthodologie adoptée par d'autres pays. En effet, avec des méthodologies plus ou moins différentes, les données recueillies dans la base de données ne seront pas les mêmes et certains spécialistes font l'hypothèse que certaines méthodologies permettent d'obtenir des données plus significatives qu'avec un recours à une méthodologie différente.

Par exemple, Antoine Flahaut (épidémiologiste et directeur de l'Institut de santé globale) déplore que la France n'ait pas suivi une méthodologie similaire à la méthodologie anglosaxonne qui consiste à effectuer un sondage hebdomadaire auprès d'un échantillon représentatif de la population afin de mieux se rendre compte de l'évolution de l'épidémie.

<img width="426" alt="image" src="https://user-images.githubusercontent.com/115630281/202932363-d474e21e-474e-4cb9-b74d-fd4b420f6fca.png">


## 5) Quelle réalités ces données/indicateurs sont-ils censés représenter ? <a name="5"></a>

Ces jeu de données est presenté de manière très brut, seulement de la data pure. Il faut la manipuler, la transformer en indicateurs et en statistiques afin de pouvoir la digérer et en tirer des conclusions précises et générales. Brut, çela est très difficile de tirer des conclusions. Ainsi, en manipulant et puis en analysant notre jeu de données SI-DEP, nous pouvons voir qu'elle représente une réalité sociale, économique et politique de la France actuelle. Nous pouvons dessiner des tendances qui se dégagent de ces données, représentant différentes réalités. 

1. L'évolution des décès toutes causes confondues en 2020 par rapport à la même période - +27% en France MAIS quand nous voyons de plus près, +91% en île-de-France et +55% dans le Grand Est. Ainsi, nous voyons l'utilité d'analyser ce jeu de données de manière filtrée afin de voir là où les tendances se dessinent. Dans ces décès, nous constatons également que les personnes âgées sont plus touchées que le reste de la population avec une augmentation de +31% des décèsde plus de 85 and, comparé à +13% des décès chez ceux entre 50 et 65 ans.

2. Taux de vaccination. Comme nous avons pu le constater durant ces deux dernières années, la vaccination et les politiques de vaccination menées par le gouvernement français sont extrêmement contestées. Çela se remarque plus dans certaines tranches d'âge par leur opinions politiques ou par leur rapport à la médecine considérée comme "intrusive" et leur probabilité de contracter le virus, et se reflète dans les données du SI-DEP. Nous avant chez ceux âgés de plus de 75 ans un taux de non-vaccination d'environ 8%, alors que chez les jeunes âgés entre 20 et 30 ans un taux de non-vaccination de presque 20%. Également, le taux de non-vaccination peut s'analyser d'un point de vue des sexes. Ainsi, nous avons un taux de non-vaccination de preque 10 points de pourcentage de plus que chez les femmes - je vous laisse en tirer des potentiels conclusions sociales. 

3. L'impact des mutations et variations du COVID-19. Quand nous pensions en avoir enfin terminé avec le COVID-19, nous avons entendu parler de différentes variantes à ne plus en finir, Omicron, beta étant les plus connus. Le jeu de données de SI-DEP nous permet également de voir l'éfficacité du vaccin fâce aux variantes. En effet, l'éfficacité vaccinale contre les variants bêta et gamma apparaît comme inférieure à celles estimées pour le variant alpha. 

4. L'éfficacité du vaccin dans la durée. Voici une grande contestation de la part du public. Personne ne s'était imaginé que nous devrions faire des piqûres de rappel du vaccin régulièrement. Selon les données les plus récentes du SI-DEP, il y aurait une très nette diminution de l'efficacité vaccinale (d'un parcours complet) contre les formes symptomatiques du COVID, qui descendrait de 90% à 57% après six mois de la complétude du parcours vaccinal chez les personnes de 50 ans ou plus, et descendrait jusqu'à 39% chez les 85 ans et plus. Après une dose de rappel, l'éfficacité vaccinale retrouve un niveau très élevé sans distinction selon la classe d'âge.


## 6) Entretien avec un data scientist travaillant chez Santé publique France <a name="6"></a>

Nous avions initialement choisi d'étudier une base de données liée à la vaccination : "Données relatives aux personnes vaccinées contre la Covid-19 VAC-SI" et nous avions donc contacté les créateurs et gestionnaires de cette base de données avant de changer de sujet pour choisir la base de données liée aux tests de dépistage qui nous semblait plus intéressante à analyser.

Nous avons notamment contacté GEODES et nous avons obtenu une réponse positive à notre demande d'entretien. GEODES nous a mis en contact avec un data scientist travaillant chez Santé publique France et contributeur à la base de données relative à la vaccination Covid-19 en France, qui a accepté de répondre à nos questions dans un entretien le 23/11/2022. Les questions/réponses porteront donc sur la base de données liée à la vaccination et non sur la base de données liée aux tests de dépistage mais nous pourrons réaliser certains parallèles entre les deux, avec l'hypothèse que la gestion de ces deux bases de données font face à des enjeux et des problématiques similaires.

La personne que nous avons interrogé travaille à la direction DATA de Santé publique France et son équipe a été en charge de produire les indicateurs de vaccination en France pendant la période Covid. L'équipe recevait les données de la part de la Direction Numérique de la Santé puis les consommait pour produire les indicateurs avec l'aide d'un prestataire pour la gestion technique de la base de données.

Les principales difficultés rencontrées dans la gestion de cette base de données ont été liées à :
* la volumétrie très importante de la base (la volumétrie a bien entendu évolué entre les débuts de la campagne de vaccination et aujourd'hui)   
* la qualité des données parfois compromise par des erreurs provenant des outils numériques utilisés lors de la saisie des données
* la communication avec le grand public
* des délais parfois longs d'accès à certaines données le temps d'obtenir des autorisations (enjeu de protection des données personnelles)

[Lien Google Doc de retranscription de l'entretien](https://docs.google.com/document/d/15-7KpxwxdH3VvAd5yGnnim50DVudQReQGXXs5-GM_fw/edit?usp=sharing)


## 7) Sources <a name="sources"></a>
* data.gouv.fr
* santepubliquefrance.fr - [Chiffres clés et évolution de la COVID-10 en France et dans le monde](https://www.santepubliquefrance.fr/dossiers/coronavirus-covid-19/coronavirus-chiffres-cles-et-evolution-de-la-covid-19-en-france-et-dans-le-monde)
* solidarites-sante.gouv.fr - [Contact-COVID et SI-DEP, les outils numériques du dépistage Covid-19](https://solidarites-sante.gouv.fr/soins-et-maladies/maladies/maladies-infectieuses/coronavirus/tout-savoir-sur-le-covid-19/article/contact-covid-et-si-dep-les-outils-numeriques-du-depistage-covid-19)

* SANCHEZ, "Budget de la « Sécu » : les laboratoires d’analyse menacent de cesser la transmission des données des tests de dépistage du Covid-19", *Le Monde*, 26 octobre 2022 ; [lien](https://www.lemonde.fr/societe/article/2022/10/26/budget-de-la-secu-les-laboratoires-d-analyse-menacent-de-cesser-la-transmission-des-donnees-des-tests-de-depistage-du-covid-19_6147347_3224.html)
* SANCHEZ, "Covid-19 : le bras de fer entre les laboratoires d’analyse et le gouvernement perturbe le suivi de l’épidémie", *Le Monde*, 14 novembre 2022 ; [lien](https://www.lemonde.fr/les-decodeurs/article/2022/11/14/covid-19-le-bras-de-fer-entre-les-laboratoires-d-analyse-et-le-gouvernement-perturbe-le-suivi-de-l-epidemie_6149857_4355770.html)
* ZORN, "État d’urgence pour les données de santé (II) : sidep et contact covid", Dalloz, 26 mai 2020, [lien](https://www.dalloz-actualite.fr/flash/etat-d-urgence-pour-donnees-de-sante-ii-sidep-et-contact-covid#.Y3p04OzMKgQ!%5)
* SANCHEZ, "Covid-19 : la plate-forme SI-Dep, qui contient les résultats des tests de dépistage, rencontre des pannes", *Le Monde*, 5 avril 2022, [lien](https://www.lemonde.fr/les-decodeurs/article/2022/04/05/covid-19-la-plate-forme-si-dep-qui-contient-les-resultats-des-tests-de-depistage-rencontre-des-pannes_6120743_4355770.html)
* VAZQUEZ, "Tests Covid : les ralentissements de la plateforme SIDEP agacent les pharmaciens", *Le Figaro*, 5 janvier 2022, [lien](https://www.lefigaro.fr/economie/tests-covid-les-ralentissements-de-la-plateforme-sidep-agacent-les-pharmaciens-20220105)




