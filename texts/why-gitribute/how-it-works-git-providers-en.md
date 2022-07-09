
## Gitribute relies on Git providers

The very difference with proprietary solutions (like GoogleSheet or Airtable) or with equivalent open sourced solutions (like [nocoDB](https://www.nocodb.com/) or [Baserow](https://baserow.io/)) is that the data you edit with Gitribute is not stored on our servers. Your data is where you want it to be, on your own Gitlab or Github organization.

So **Gitribute does not have its own backend server**, but relies only on [Gitlab](https://gitlab.com/), [Github](https://github.com/), or [Mediawiki](https://www.mediawiki.org/wiki/MediaWiki) APIs. It means if you already have your own Gitlab account (or better, your own Gitlab instance), you won't have to rent a server for your database, let it on Gitlab, it already does a lot : versionning, authentication, pull requests...

This way your data stays protected, and you can manage the incoming contributions as you'd manage many pull requests.

