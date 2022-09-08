---
title: Idées principales
tags: [ R&D, ideas ]
created: 17/07/2022
author: Julien Paris
---

Datami est conçu comme un "micro-service" léger, qui vous laisse choisir parmi une collection réduite de widgets réutilisables pour **afficher les données que vous voulez**, **où vous voulez**, le tout **gratuitement**.

Pour rendre cela possible techniquement nous avons conçu Datami comme un projet _pure frontend_..

Pas de backend dans la _stack_ de Datami : cela aurait occasionné trop de maintenance, trop cher, trop chronophage, trop de soucis quoi...

Cela dit, si on souhaite afficher des données dans un widget _front_ _**les données doivent bien venir de quelque part, non ?**_

### Des services Git en guise de bases de données

En tant que développeurs nous-mêmes nous avons un usage à la quotidien et assez extensif de plateformes comme Github ou Gitlab. En général nous - les développeurs - sommes assez d'accord sur le fait que ce sont des infrastructures **extrêmement** utiles !

Tous les jours nous (enfin nous, développeurs) profitons de ces services pour :

- La gestion des versions et des modifications ;
- L'authentification et l'identification de "qui modifie quoi" ;
- Utiliser les APIs de ces services ;
- Communiquer et échanger avec nos pairs ;
- Le tout sur des services aux infrastuctures stables et robustes ;
- etc...

Du coup si nous - développeurs - hébergeons nos données et notre code sur ces services tout le temps, pourquoi ne pas tenter de vous faire bénéficier vous aussi (pas développeur) de tout cela ?

**La base de données préférée de Datami est "pas de base de donnée du tout"**, du moins au sens habituel du terme. En lieu et place de base de donnée dédiée pour Datami (qui aurait pu être un serveur de _backend_ + BDD en SQL, PostGreSQL, MongoDB...) **Datami s'appuie sur Github ou Gitlab (qu'on appellera ici des "services git") pour le stockage des données**, et donc sur la possibilité que les données soient sur un _repo_ qui vous appartient.

Il existe un documentation extrêmement fournie sur les APIs de ces services (Gitlab est un logiciel libre par ailleurs), APIs qui permettent de modifier ces données à distance.

L'autre fonctionnalité importante dans Datami que permet le fait de s'adosser à ces "services Git" comme Github ou Gitlab réside dans la possibilité de créer des `branches` et des `pull requests`. Imaginez ces actions comme des "propositions de contribution" envoyées au propriétaire d'un fichier : **celui-ci peut accepter, rejeter, modifier, amender, votre proposition avant de l'intégrer (ou "merger") dans son fichier**.

Nous considérons que le processus de `pull request` et la modération qu'il induit, reste la manière la plus "polie et élégante" de collaborer : proposer quelque chose à quelqu'un, lui laisser la liberté d'accepter ou pas... bref, engager la conversation.

Cette manière de contribuer a de bonnes _[manières](https://idiomorigins.org/origin/manners-maketh-man)_.

### Intéropérabilité "basique"

Dans le petit monde de la "tech" - et particuièrement dans le milieu de l'_open source_ - l'"intéropérabilité" est un Graal après lequel tout le monde court : **faire en sorte qu'une donnée produite ici soit lisible ailleurs** (sur un autre ordinateur, dans un autre logiciel). Le protocole HTTP, le RSS, le XML, le "web sémantique", le standard _activityPub_, ... sont autant d'inventions géniales allant dans ce sens.

L'univers des technologies numériques regorge de ces normes, outils, _frameworks_, langages, etc... Certains sont réellement devenus des standards et ont été à la fois largement adoptés et acceptés comme tels. D'autres par contre luttent pour le devenir ou périssent en le tentant.

Depuis le début de l'informatique de nombreux acteurs de la _tech_ (des corporations par exemples) défendent et promeuvent leur(s) propre(s) standard(s), toujours meilleur(s) que celui de la concurrence.

_Une petite pensée en passant pour le mini-disc, le bluray, et tous ces autres standards qui firent long feu avant leur chant du cygne..._ _Et une autre pensée moins tendre pour Apple et leur fâcheuse habitude de changer leurs connecteurs tous les dix minutes_.

Effectivement ce petit monde de la _tech_ est... comment dire... un peu "technique", du moins pour des personnes "normales" (oui, il y a encore des gens qui ne sont pas des développeurs en ce bas monde).

Tentez d'expliquer en cinq minutes les avantages et inconvénient du _web sémantique_ à votre papi ou à votre mamie. Vous voulez vraiment essayer ? ... vraiment ?

Au lieu de viser une "intéropérabilité tous azimuts", nous avons préféré penser Datami comme un outil visant à **l'intéropérabilité "la meilleure possible à la fois pour les ordinateurs et les débutants"**, consistant en la combinaison de :

- **"Qu'est-ce que les personnes non techniciennes utilisent habituellement ?"** : excel spreadsheets, gsheet, airtable... par exemple.
- **"Qu'est-ce que n'importe quelle machine peut lire aujourd'hui ?"** : les formats `json`, `csv`, `markdown` ...

Nous ne dirions pas que Datami est "intéropérable", mais juste que Datami tente d'utiliser au mieux les standards **à la fois les plus communs** et **pour les humains**, et **pour les machines**.

### Agnostique envers les données et leurs modèles

Les données, il y en a pour tous les goûts et toutes les couleurs...

En général si vous ne produisez pas vous-même un jeu de données, les données que vous recevez le sont dans un format et dans un état que vous n'attendiez pas forcément... Et des fois, souvent, plutôt l'inverse.

Une idée centrale dans le projet Datami est que Datami devrait **pouvoir afficher tout type de donnée arrivant dans un fichier de type commun** (`csv`, `json`, `md`), quel que soit leur contenu : **Datami tente de rester "data-agnostique"**.

Cette intention est fondatrice dans la manière dont nous avons conçu Datami et dans sa capacité à afficher des données. Pour aller au bout de cette idée nous avons permis - si l'utilisateur le souhaite - d'adjoindre différentes options de visualisations à un jeu de données afin qu'il soit rendu aussi agréablement que voulu.

En partant du principe que la manière la plus commune de produire des jeux de données était de le faire sous le format "tableur", nous avons inclus très rapidement dans nos développement l'option consistant à pouvoir **appliquer un [modèle de données (ou _table schema_)](https://specs.frictionlessdata.io/table-schema/)** ainsi que d'autres propriétés **à vos tableurs `csv` or `tsv`**.

### Une collection de widgets...

Datami est constitué d'une petite collection de widgets que vous pouvez utiliser séparément ou conjointement.

Nous ne souhaitions pas centraliser et stocker vos données sur un même service. Nous ne souhaitions pas non plus obliger vos utilisateurs à se rendre sur un domaine en particulier pour consulter _vos_ données. **Nous voulions que vous puissiez valoriser vos données sur votre propre site**.

Après tout, _vous_ avez transpiré pour les produire, _vous_ en êtes le.la propriétaire, et donc au final _vous_ en êtes responsable.

Par contre si vous souhaitez à la fois **valoriser** vos données et les faire **gagner en qualité**, la meilleure des stratégies est que **vos données puissent être réutilisées et améliorées par d'autres personnes que vous.**

Partager... [This is the way](https://www.youtube.com/watch?v=uelA7KRLINA&ab_channel=Gabriel)...

Dans cette optique "partager ses données" ne peut pas se faire à moitié, cela suppose de laisser les tiers réutiliser VOS données là où ILS le souhaitent.

Les widgets et le fait de s'adosser à des "services Git" pour le stockage est une solution technique qui nous semblait résoudre ce double problème : permettre un large partage, tout en vous laissant garder le contrôle sur vos propres données :

- Les données source sont hébergées dans _votre_ service Git ;
- Un widget affichant ces données peut _être intégré_ dans n'importe quel site web ;
- Tout le monde peut _proposer_ des contributions si vous le souhaitez ;
- Mais uniquement _vous_ pouvez accepter ou non une contribution, et la merger aux données source.

Paraphrasons nos élégants amis les Anglais et disons que **"[_Manners maketh commoner_](https://www.youtube.com/watch?v=hUtNQAdhIR4&ab_channel=RodStickler)...** _you know what that means ?_"

### ... Pour les débutants

Nous pensons que personne n'a besoin d'un diplôme d'ingénieur pour posséder ou partager son savoir.

La connaissance _c'est_ de la donnée et, tout comme les données, la connaissance de chacun ou de tout groupe est aussi affaire de goûts et de couleurs.

Afin de partager cette connaissances aux formes multiples dans un monde numérisé, l'expression et la transmission du savoir ne peut se faire qu'avec une médiation technique, en l'occurrence des **interfaces**.

Le dernier principe - et sans doute le plus important dans notre approche - est donc celui de **donner une importance majeure à l'expérience utilisateur (_UX_) et aux interfaces (_UI_)**.

Nous ne soulignerons jamais assez ce principe : **un bon _design_ est un _design_ qui ne se remarque pas**.

> Personnellement j'aime aussi cette variante : "Une interface c'est comme une blague. S'il faut l'expliquer c'est qu'elle n'est pas si bonne."

Maintenant reste à tenir cette promesse le mieux possible...
