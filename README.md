# GLOSSAIRE

- [Général](#général)
- [Front-end](#front-end)
- [UX / UI](#ux-ui)
- [Architecture](#architecture)
- [Modélisation / Base de données](#modélisation---base-de-données)
- [Symfony](#symfony)
- [Sécurité](#sécurité)
- [RGPD](#rgpd)
- [SEO](#seo)
- [Gestion de projets / DevOps](#gestion-de-projets---devops)
- [English](#english)

## Général

1. Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte

   Laragon (Windows) et MAMP (MAC)

2. Qu’est-ce qu’un algorithme ?

   Un algorithme est une suite d’étapes/instructions permettant de retourner un résultat.

3. Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?

   Une variable est un élément qui associe un nom avec une valeur, une variable est préfixée avec « $ » sur PHP.

4. Qu’est-ce que la portée d’une variable ?

   La portée d’une variable est son espace de fonctionnement. La portée est de base étendue sur tout le programme mais peut être limitée à une fonction ou une classe.

5. Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?

   Une constante est une variable qui ne peut pas être modifiée au cours d’un programme.

6. Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation

   Une superglobale est une variable prédéfinie, elle est disponible quel que soit le contexte du script. Il en existe 9.\
   $\_COOKIE est utilisée comme un tableau associatif, il peut chercher et données des cookies http et les introduire dans le code.

7. Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)

   Les différents types sont :

   -char (caractère) : $name = 'maxime'

   -int (entier) : $age = 23

   -float (chiffre à virgule) : $bankAccount = 15,42€

   -double (chiffre à virgule dépassant les 15 chiffres) : π

   -boolean (booléen) : $isGood = true

   -byte (octet)

   -void : null

8. Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?

   Oui, il y a les tableaux indexés, les tableaux associatifs et les tableaux multidimensionnels.

9. Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles

   Il existe 3 différentes structures de contrôle :\
   -La séquence : Consiste à exécuter les actions les unes à la suite des autres.\
   exemple : un bloc de code\
   -La répetition : La répétition consiste à évaluer une condition et d'effectuer une ou des actions tant que la condition est VRAI.\
   exemple : une boucle (for, while, foreach)\
   -La sélection : La séquence consiste à exécuter les actions les unes à la suite des autres.\
   exemple : if/else, switch statement\

10. Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?  

    strlen()

12. Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP

   Une session est un moyen de stocker des données pour chaque utilisateur en utilisant un identifiant unique.\
   Elle se démarre en utilisant session_start(). \
   Exemple : système de compte pour utilisateur

12. Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP

    Un cookie est un mécanisme d'enregistrement et de lecture d'informations sur le client.\
    Exemple : enregistrer le nom d'utilisateur

13. Quelle est la différence entre les instructions « require » et « include » en PHP

    require est utilisé quand le fichier 'requis' est indispensable au bon fonctionnement de l'app, include est utilisé dans le cas contraire

14. Comment effectuer une redirection en PHP ?

    Avec la fonction header()

15. Définir la partie « front-end » et « back-end » d’une application

    La partie front-end d’une application est la partie gérée du côté client, elle est principalement chargée de l’affichage (partie boutique     d’un magasin) contrairement à la partie back-end qui est gérée du côté serveur et est principalement chargée du fonctionnement (partie        arrière/entrepôt d’un magasin).

16. Définir le contrôle de version ? Qu’est-ce que Git ?

    Le contrôle de version est le fait de suivre et gérer les changements apportés au code d’un logiciel. Git est le système de contrôle de       version le plus utilisé.

17. Qu’est-ce qu’un CMS ? Citer au moins 2 exemples

    Un CMS (Content Management System) est un outil pour créer un site web sans directement utiliser la programmation, Webflow et Wordpress       sont de bon choix.

## Front-end

18. Définir HTML  

    HTML (HyperText Markup Language) est un langage de balisage, il est utilisé afin de créer le contenu et la structure d’un site web.

20. Définir CSS  

    CSS (Cascasing Style Sheets) est un langage de style, il sert à donner la forme et à manier les éléments d’un site web ?

22. Définir Javascript  

    JavaScript est un langage de script orienté objet, il sert à manipuler des éléments HTML et CSS afin de rendre un site web plus animé et      intuitif.

24. Définir JSON. Dans quel contexte ce format est-il utilisé ?  

    JSON (JavaScript Object Notation) est un moyen de représenter des objets, tableaux et données JS.

26. Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?  

    Oui il est possible d’interpreter du JavaScript côté serveur avec Node.js, il s’suffit d’écrire une ligne de commande “node example.js”.

28. Qu’est-ce qu’un sélecteur CSS ?  

    Un sélecteur CSS définie les éléments sur lesquels les propriétés CSS s’appliquent.

30. Quelle balise HTML permet de créer un lien hypertexte ?  

    La balise anchor ( <a>…</a>) permet de créer un lien hypertexte.

32. Qu’est-ce qu’une requête AJAX ?  

    Une requête AJAX est une technique qui permet d’actualiser une page web sans la recharger totalement.

34. Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?  

    Le sélecteur « . » permet de sélectionner tous les éléments d’une classe et le sélecteur « # » permet de sélectionner tous les éléments       d’un identifiant.

36. Définir le responsive design  

    Le responsive design est le fait de créer une application qui s’adapte à différentes tailles d’écran (mobile, tablette et desktop).

38. Qu’est-ce que le templating ?  

    Le templating est le fait de regrouper plusieurs fichiers et leurs appliquer du HTML/CSS afin d’éviter les répétitions.

40. Qu’est-ce qu’une fonction anonyme en Javascript ?  

    Une fonction anonyme est une fonction qui n’a pas de nom. On peut exécuter en l’affectant à une variable, en l’auto-invoquant ou en           l’utilisant dans un évènement.

42. Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?  

    La méthode push().

44. Qu’est-ce qu’un « media query » ?  

    Un media query est une requête CSS qui permet de modifier le visuel en fonction de la taille de l’écran utilisé.

46. Qu’est-ce qu’un pseudo élément en CSS ?  

    Un pseudo-élément est un mot-clé ajouté en utilisant « :: » (ne pas confondre avec : des pseudo-classes) qui permet de mettre en forme        certaines parties de l’élément ciblé par la règle.

48. Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent  

    Bootstrap est un framework front-end, il permet de créer le HTML et CSS bien plus rapidement en utilisant des templates.

    Tailwind, Bulma ou Materialize sont des équivalents.

34. Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes  
    La méthode GET récupère une page et affiche son contenu alors que la méthode POST récupère le contenu et l’envoie au serveur.

## UX UI

35. Quelle est la différence entre UX Design et UI Design ?  

    UX design (User Experience) se focalise sur la facilité de prise en main et l'accessibilité de l'interface alors que l'UI design (User Interface) se focalise sur les visuels et la visibilité de l'interface.

37. Qu’est-ce qu’un wireframe ?  

    Un wireframe est un schéma d'une page web, il est souvent fait de forme basiques et en nuances de gris. Un wireframe permet de pré-visualiser la structure d'un site.

39. Qu’est-ce qu’un prototype ?

    Un prototype est une version détaillée du produit fini avec animations et transitions incluses

40. Qu’est-ce que la hiérarchie visuelle en UI Design ?

    La hiérarchie visuelle est le fait d'appliquer des propriétés à certains éléments afin de les faires ressortirs, exemple : COntraste de couleur, texte gras, taille de la police, emplacement

42. Qu’est-ce que l’accessibilité en UX Design ?

43. Qu’est-ce qu’une grille de mise en page ?

44. Qu’est-ce que la notion d’affordance en UX Design ?

45. Qu’est-ce qu’un « mobile first design » ?  

    Le mobile first design est le fait de créer un site avec une structure et un style adapté aux petits écrans, puis de l'ajuster pour les       écrans plus larges.

## Programmation orientée objet (POO)

43. Donner une définition de la programmation orientée objet  

    La POO consiste à définir et faire interagir entre eux des objets, compris ici comme tous types de structures issues d’un langage donné.      Par convenance, les objets en POO désignent le plus souvent des variables complexes, elles-mêmes composées de variables ou       de fonctions.

45. Qu’est-ce qu’une classe ? Comment la déclare-t-on ?  

    Une classe est un élément qui créé contient des objets, on la déclare avec des attributs et des méthodes.

47. Qu’est-ce qu’un objet ?  

    Un objet représente un concept, une idée ou toute entité du monde physique. Il possède une structure interne et un comportement et peut       interagir avec ses pairs.

49. Définir la notion de propriété / attribut / méthode  

    Les attributs (propriétés) représentent les caractéristiques de l’objet et les méthodes correspondent aux actions possibles avec l’objet.

51. Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité  

    La visibilité d’une propriété/méthode correspond à son rayon d’action.

-Publique : permet aux propriétés/méthodes d’être accessible depuis n’importe où dans le programme principal.

-Privée : permet aux propriétés/méthodes de n’être accessible que depuis l’intérieur de la classe.

-Protégée : l’intermédiaire entre les deux autres, elle permet d’utiliser les propriétés/méthodes communs dans une classe parente et ses classes dérivées.

48. Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?  

    Le constructor est la méthode (magique) la plus utilisée pour créer un nouvel objet, elle permet de définir tous les attributs de l’objet     en le créant.

50. Qu’est-ce que l’encapsulation ?

51. Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple

    Étendre une classe consiste à créer une classe mère qui regroupe des classes enfants. Cela permet aux classe enfant d’hériter des             attributs de la classe mère.

   Exemple : On crée une classe mère “Personne” et deux classes enfant “Acteur” et “Réalisateur”, on a plus qu’à déclarer les attributs (nom,    prenom, sexe, age) une seule fois dans la classe “Personne” et les deux classes enfant hériteront de ses attributs.

51. Définir l’opérateur de résolution de portée

52. Définir une méthode / propriété statique

53. Définir le polymorphisme en POO

54. Définir une méthode / classe abstraite ?
   Une méthode abstraite peut seulement être déclaré par son nom ou ses paramêtres (signature), une classe abstraite est une classe qui ne peut être instanciée.
   Si une classe contient une méthode abstraite, elle doit elle aussi devenir une classe abstraite

55. Définir le chaînage de méthodes

56. Qu’est-ce que la méthode **toString() ? Existe-t-il d’autres méthodes « magiques »  

    La méthode magique **toString permet de passer en chaîne de caractères différents attributs de la classe, elle peut être appelée en           utilisant $this.
    Il existe d’autres méthodes magiques (**construct, **destruct, \_\_call et plein d’autres).

58. Qu’est-ce qu’un « autoload » ?  

    Un autoload est un auto-chargement de classe, il permet de charger plusieurs classes d’un programme au sein d’un seul et même fichier.

59. Comment appelle-t-on en français les « getters » et les « setters » ?  

    Les getters sont des accesseurs et les setters sont des mutateurs.

61. Qu’est-ce que la sérialisation en PHP ?

   La sérialisation est une technique qui à pour but de transferer des valeurs entre scripts sans qu'elles perdent leurs structure ou type. 
   

## Architecture

60. Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence
61. Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern
   Un design pattern (patron de conception) est une infrastructure, une suite d'étapes permettant de créer un logiciel/app avec une structure controlée

   Factory, Observer, Decorator

62. Qu’est-ce que l’architecture MVC ?
63. Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?
64. Quels sont les avantages de l’architecture MVC ?
65. Existe-t-il des variantes à l’architecture MVC ?
66. Qu’est-ce qu’une API ? Définir l’architecture REST

## Modélisation - Base de données

67. Qu’est-ce que la modélisation de données ? Définir la méthode Merise
68. Quelles sont les 3 étapes principales de la méthode Merise ?  
    a. Analyse, conception et réalisation  
    b. Planification, exécution et contrôle  
    c. Création, modification et suppression
69. Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?
70. Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?
71. Donner la définition des mots suivants :
    a. Entité
    b. Relation
    c. Cardinalité
    d. Clé primaire / clé étrangère
72. Que devient une relation de type « Many To Many » dans le modèle logique de données ?
73. Qu’est-ce qu’une base de données ?
74. Définir les notions suivantes :
    a. SQL
    b. MySQL
    c. SGBD (donner 2 exemples de SGBD)
75. Dans une base de données, les données sont stockées dans des **_. Celles-ci sont constituées de lignes appelées _** et de colonnes appelées \_\_\_
76. Quelle est la différence entre une base de données relationnelle et non relationnelle ?
77. Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?
78. A quoi sert une vue dans une base de données ?
79. Qu’est-ce que l’intégrité référentielle dans une base de données ?
80. Quelles sont les fonctions d’agrégation en SQL ?
81. Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?
82. Quelles sont les clauses qui permettent de :  
    a. Insérer un nouvel enregistrement dans une table  
    b. Modifier un enregistrement dans une table  
    c. Supprimer un enregistrement dans une table  
    d. Supprimer la base de données  
    e. Filtrer les résultats d’une requête SQL  
    f. Trier les résultats d’une requête SELECT  
    g. Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique  
    h. Concaténer 2 chaînes de caractères
83. Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?

## Symfony

84. Qu’est-ce que Symfony ?
   Symfony est un framework de PHP permettant d'utiliser des composants PHP plus simplement et plus rapidement

85. Sur quel langage de programmation et design pattern repose Symfony ?
   Symfony se repose sur PHP et sur le design pattern MVC

86. Quelle est la dernière version en date de Symfony ?
    La dernière version en date est la 7.1

87. Qu’est-ce qu’un bundle ?
   Un bundle est un ensemble, une collection de code / fichiers / ressources facile à installer

88. Quel est le moteur de template utilisé par défaut dans Symfony ?
   Le moteur de template utilisé par défaut est twig

89. Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?
   Un ORM (Object-Relational Mapping) est un programme qui créer une relation entre une app et une base de donnée. L'ORM Doctrine est utilisé au sein de Symfony.

90. Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?
91. Que permet le bundle Maker au sein de Symfony ?
   Le bundle Maker de Sylfony permet de facilement créer des éléments tels que des entités, des controlleurs ou des commandes.

92. Quel est le langage de requêtage exploité au sein d’un projet Symfony ?
   DQL (Doctrine Query Language) est le language de requêtage utilisé avec Symfony, il permet de directement inclure les entités dans les requetes.

93. Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?

## Sécurité

94. Qu’est-ce que l’injection SQL ? Comment s’en prémunir ?

   L'injection SQL est le fait d'attacher des lignes de codes SQL dans les inputs d'un site afin de modifier la base de donnée. On peut s'en     prémunir en préparant ses requêtes SQL.

95. Qu’est-ce que la faille XSS ? Comment s’en prémunir ?
 
   Une faille XSS est le fait d'introduire du code malveillant dans un site. On peut s'en prémunir en utilisant par exemple des filter_input     ou filter_var en PHP, cela permettra aux formulaires de détecter et annuler du code malveillant ou des caractères non voulus.

96. Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?
97. Définir l’attaque par force brute et l’attaque par dictionnaire
98. Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement
99. A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?
100.  Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage
101.  Qu’est-ce qu’une politique de mots de passe forts ?
102.  Qu’est-ce que l’hameçonnage ?
103.  Définir la « validation des entrées »

## RGPD

104. Qu’est-ce que le RGPD ?
105. Quel est son objectif principal ?
106. Quelle est la date d’entrée en vigueur du RGPD ?
107. Quelles sont les sanctions possibles en cas de non-respect du RGPD ?
108. En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?
109. Quel est le consentement valide selon le RPGD ?
110. Qu’est-ce qu’une politique de confidentialité ?
111. Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?
112. Quels sont les droits des utilisateurs selon le RGPD ?
113. Qu’est-ce que le principe de minimisation des données selon le RGPD ?

## SEO

114. Qu’est-ce que le SEO ?
115. Quel est l’objectif principal du SEO ?
116. Existe-t-il plusieurs types de référencement ? Lesquels ?
117. Qu’est-ce que la densité de mots-clés en SEO ?
118. Qu’est-ce qu’une balise « alt » ?
119. Qu’est-ce que la balise « meta description » ?
120. Qu’est-ce que le « nofollow » en SEO ?
121. Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?
122. Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?
123. Quelle est la recommandation pour les URL d'un site web bien référencé ?
124. Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?
125. Qu'est-ce que l'optimisation des images pour le référencement ?
126. Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

## Gestion de projets - DevOps

127. Qu’est-ce que la gestion de projet ?
128. Qu’est-ce qu’une méthode Agile de gestion de projet ?
129. Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages
130. A quoi sert la méthodologie MVP ? Citer les caractéristiques clés
131. Qu’est-ce que la planification itérative ?
132. Citer 3 méthodes Agiles dans le cadre d’un projet informatique
133. Qu’est-ce qu’une réunion de revue de projet ?
134. Qu’est-ce qu’un livrable dans un projet ?
135. Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux
136. Qu’est-ce que le DevOps et quel est son objectif principal ?
137. Qu’est-ce que l’intégration continue ?
138. Qu’est-ce que Docker ? Et en quoi est-il utile dans le cadre du DevOps ?
139. Qu’est-ce qu’un test unitaire ?
140. Quelle est l'unité de code testée lors d'un test unitaire ?
141. Quelles sont les caractéristiques d'un bon test unitaire ?
142. Qu'est-ce qu'une assertion dans un test unitaire ?

## English

1. What does JavaScript enable you to do on a website ?

   a. Add interactive behavior and dynamic content <-

   b. Define the layout and design of web pages

   c. Handle server-side operations

2. Which programming language is primarily used for server-side web development ?

   a. PHP <-

   b. JavaScript

   c. HTML

3. What is the purpose of a web browser ?

   a. To render and display web pages <-

   b. To execute serve-side code

   c. To manage databases

4. What is the difference between GET and POST methods in HTTP ?

   a. GET retrieves data from a server, while POST submits data to a server <-

   b. GET submits data to a server, while POST retrieves data from a server

   c. GET and POST methods are interchangeable

5. What is the purpose of version control systems (e.g., Git) in web development ?

   a. To track changes and manage collaborative development <-

   b. To optimize website loading speed

   c. To handle server-side scripting

6. What is the purpose of a framework in web development ?

   a. To provide a structured environment for building web applications <-

   b. To handle network protocols and data transfer
   
   c. To create visual designs and layouts for websites

7. What does NoSQL stand for ?

   a. Not Only SQL <-

   b. Non-Structured Query Language
   
   c. New Object-Oriented Language

8. Which of the following is a characteristic of NoSQL databases ?

   a. Strict schema enforcement

   b. Support for complex transactions
   
   c. Scalability and flexible data models <-
