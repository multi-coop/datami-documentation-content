---
title: Comment ça marche Gitribute ?
tags: [ tech, R&D ]
created: 17/07/2022
author: Julien Paris
---

C'est parti pour un petit coup d'oeil sous le capot.

## Gitribute est une collection de widgets

Gitribute est une application web fournissant une série de "[widgets](https://en.wikipedia.org/wiki/Web_widget)". Cela signifie que **vous pouvez intégrer Gitribute dans n'importe quel site web**, et que vous n'avez pas besoin de votre propre serveur pour utiliser un widget de Gitribute.

Le terme "widget" est équivalent à celui de "composant web", c'est une façon d'afficher au sein d'un site un composant indépendant fourni par un serveur tiers. L'approche "widget" est similaire à celle de la bonne vieille _iframe_, à ceci près que les widgets sont plus flexibles et plus adaptés au web d'aujourd'hui que les _iframes_.

## Gitribute relies on Git providers

🚧  &nbsp; `Translation in progress...`

The very difference with proprietary solutions (like GoogleSheet or Airtable) or with equivalent open sourced solutions (like [nocoDB](https://www.nocodb.com/) or [Baserow](https://baserow.io/)) is that the data you edit with Gitribute is not stored on our servers. 

Your data is where you want it to be, for instance on your own Gitlab server or on your Github organization.

So **Gitribute does not have its own backend server**, but relies only on [Gitlab](https://gitlab.com/), [Github](https://github.com/), or [Mediawiki](https://www.mediawiki.org/wiki/MediaWiki) servers and APIs to store your data where you put it originally. 

It means if you already have your own Gitlab account (or better, your own Gitlab instance), you won't have to rent a server for your database. Let your data be on Gitlab / Github / Mediawiki, those already do a lot : versionning, authentication, pull requests...

This way your data stays where it was, protected, and you can manage the incoming contributions as you would manage any "pull request".

> **Note** : More about our "no-code" solutions benchmark in the **["Why Gitribute ? > Benchmark"](/benchmark)** section

## Contribute anonymously (if you feel a bit shy)

🚧  &nbsp; `Translation in progress...`

Gitribute uses the [tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) system provided by Github or Gitlab to "commit" and contribute to some data stored on one of those git providers.

To avoid asking to your grandpa' or your grandma' to create an account on those providers, and even worse to avoid asking them to create their own personal tokens, **Gitribute uses a default "ghost user token" (or your own)**.

If you want anonymous contribution onto your data with Gitribute, it is necessary to set your repo and related branches on Github or Gitlab for this "ghost user"'s actions (GET, PUT, POST). 

> **Note** : Basically you don't want this user's token to make "pushes" on your `main` branch for instance...

To sum up, when you set up your Gitribute widget from scratch you have to :

- 1/ Create your own "ghost user" / default token
- 2/ Set up the target repo to allow this token to make contributions (create branches, but not pushes directly to your `main` branch)
- 3/ You can inject this default token in the widget (either from an `.env` variable or directly from the frontend).

That way, an **user can push commits anonymously, without having to create its own Github or Gitlab account**. That said you can add a little message to the data owner to your anonymous contribution.

Users can also use their own token.

Your data on the `main` branch stays protected on your Git provider, and you - the dataset's owner - keep the control of who can write on it and on which branch.

It could seem like a bit of a hack, but the "ghost user" trick is not that much complicated.

It's like letting your grandpa' or grandma' use your Netflix account...
