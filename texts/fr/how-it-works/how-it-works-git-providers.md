
## Gitribute relies on Git providers

🚧  &nbsp; `Translation in progress...`

The very difference with proprietary solutions (like GoogleSheet or Airtable) or with equivalent open sourced solutions (like [nocoDB](https://www.nocodb.com/) or [Baserow](https://baserow.io/)) is that the data you edit with Gitribute is not stored on our servers. 

Your data is where you want it to be, for instance on your own Gitlab server or on your Github organization.

So **Gitribute does not have its own backend server**, but relies only on [Gitlab](https://gitlab.com/), [Github](https://github.com/), or [Mediawiki](https://www.mediawiki.org/wiki/MediaWiki) servers and APIs to store your data where you put it originally. 

It means if you already have your own Gitlab account (or better, your own Gitlab instance), you won't have to rent a server for your database. Let your data be on Gitlab / Github / Mediawiki, those already do a lot : versionning, authentication, pull requests...

This way your data stays where it was, protected, and you can manage the incoming contributions as you would manage any "pull request".

> **Note** : More about our "no-code" solutions benchmark in the **["Why Gitribute ? > Benchmark"](/benchmark)** section
