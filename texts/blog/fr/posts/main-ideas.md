---
title: Idées principales
tags: [ R&D, ideas ]
created: 17/07/2022
author: Julien Paris
---

Gitribute est conçu comme un "micro-service" léger, qui vous laisse choisir parmi une collection réduite de widgets réutilisables pour **afficher les données que vous voulez**, **où vous voulez**, le tour **gratuitement**.

Pour rendre cela possible techniquement nous avons conçu Gitribute comme un projet _pure frontend_..

Pas de backend dans la _stack_ de Gitribute : cela aurait occasionné trop de maintenance, trop cher, trop de soucis quoi...

Cela dit, si on souhaite afficher des données dans un widget _front_ _**les données doivent bien venir de quelque part, non ?**_

### Des services Git en guise de bases de données

En tant que développeurs nous-mêmes nous avons un usage à la quotidien et assez extensif de plateformes comme Github ou Gitlab. En général nous - les développeurs - sommes assez d'accord sur le fait de ce sont des infrastructures **extrêmement** utiles !

Tous les jours nous (enfin nous, développeurs) nous profitons de ces services pour :

- La gestion de versions et de modifications ;
- L'authentification et l'identification de qui modifie quoi ;
- Des APIs ;
- Communiquer et échanger avec nos pairs ;
- Le tout sur des services aux infrastuctures stables et robustes ;
- etc...

Du coup si nous - développeurs - hébergeons nos données et notre code sur ces services tout le temps, faisons ainsi mais tentons de vous faire bénéficier vous aussi de tout cela.

**La base de données préférée de Gitribute est "pas de base de donnée du tout"**, du moins au sens habituel du terme. En lieu et place de base de donnée dédiée pour Gitribute (qui aurait pu être un serveur de _backend_ + BDD en SQL, PostGreSQL, MongoDB...) **Gitribute s'appuie sur Github ou Gitlab pour stocker les données**.

Il existe un documentation extrêmement fournie sur les APIs de ces services (Gitlab est un logiciel libre par ailleurs), APIs qui permettent de modifier ces données à distance.

L'autre fonctionnalité importante dans Gitribute que permet le fait de s'adosser à ces "services Git" que sont Github ou Gitlab réside dans la possibilité de créer des `branches` et des `pull requests`. Imaginez ces concepts comme des "propositions de contribution" envoyées au propriétaire d'un fichier : **celui-ci peut accepter, rejeter, modifier, amender, votre proposition avant de l'intégrer (ou "merger") dans son fichier**.

Nous considérons que le processus de `pull request` et la modération qu'il induit, sont la manière la plus "polie et élégante" de collaborer : proposer quelque chose à quelqu'un, lui laisser la liberté d'accepter ou pas, bref engager la conversation.

Cette manière de contribuer a des _[manières](https://idiomorigins.org/origin/manners-maketh-man)_.

### Basic interoperabilty

🚧  &nbsp; `Translation in progress...`

In the "tech" world - and especially in the open source movement - "full interoperability" is the Graal we all crave for. Http protocol, RSS, XML, Semantic web, activityPub, were or still are great inventions reaching for this goal.

Digital world is full of standards, tools, frameworks, languages, uses, etc... Some standards are adopted and widely accepted, other are struggling to become so.

Many actors (corporations or else) fight to defend their own standard(s), which is always better than the competitor's standard, and it goes on and on...

_A little though here for the mini-disc standard, the blu-ray, and many other standards who died fiercly... And a less tender though for Apple and their habit to change plugs shape every ten minutes._

But this tech world could seem... you know... kinda very technical, at least for "normal" people.

Try to explain the pros and cons of semantic web to your grandpa' or grandma', I dare you.

So instead of "extensive interoperability" we prefer to imagine Gitribute posture about this topic as reaching for the **"best interoperability between noobs & machines"**, as the combination of :

- **"What people commonly use"** : excel spreadsheets, gsheet, airtable... for instance.
- **"What could be read by any machine today"** : `json`, `csv`, `markdown` ...

We won't say Gitribute is interoperable, it's just it tries to use standards having the best chance to be commonly used by human and machines **altogether**...

### Data and schema agnostic

🚧  &nbsp; `Translation in progress...`

Data comes in every shapes and forms. 

Usually - if you did not produce this data - they come in forms you don't expected... at all...

A key idea in Gitribute is it should display **any data in a common format**, disregarding what's inside : **Gitribute tries to stay "data agnostic"**.

Taking this as the ground step for displaying data, we also wanted to append - if and only if necessary - more options so your data could be shown as beautiful you imagined it.

Knowing the more common way to write data were the "table" format, we included very early in our developments a keystone feature allowing **to apply a [table schema](https://specs.frictionlessdata.io/table-schema/)** and other custom properties **to your `csv` or `tsv` files**.

### A widgets collection...

🚧  &nbsp; `Translation in progress...`

Gitribute is constituted by of a collection of widgets you can use separatly or compose with.

We didn't want to centralize a service and/or your data.

After all _you_ sweat to produce it, _you_ own it, therefore _you_ are responsible for it.

But if you want to **valorize** and **refine your data** the best chance to do so is to **let other people reuse and contribute to YOUR data**.

Sharing. [This is the way](https://www.youtube.com/watch?v=uelA7KRLINA&ab_channel=Gabriel)...

"Sharing data" means letting people reuse YOUR data where THEY want.

Widgets are the solution we though of to allow this, without the risk to lose entirely the control over your data :

- The data source stays in _your_ repository ;
- But _anybody_ can make a proposal...

Let's dare say again that **"[Manners maketh commoner](https://www.youtube.com/watch?v=hUtNQAdhIR4&ab_channel=RodStickler)...** _you know what that means ?_"

### ... For noobs

🚧  &nbsp; `Translation in progress...`

We believe you don't have to be an engineer to have or share your knowledge.

Knowledge _is_ data, and likewise it comes in all shapes and forms.

But in a digital world **interfaces** are the key to make possible the expression and sharing of people's knowledge.

The last - and perhaps more important - principle we follow is the **major importance of UX and UI design**.

We won't emphasize this enough : **a good design is a design you don't have to ask or care about**.

Now let's do our best to fulfill this promise...
