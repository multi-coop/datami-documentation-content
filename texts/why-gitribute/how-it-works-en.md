
# How does it work ?

## Gitribute is a widgets system

Gitribute is a web application providing a serie of "[widgets](https://en.wikipedia.org/wiki/Web_widget)". It means that **you could integrate it inside any website**, and you don't have to rely on a centralized website to use any of our widgets.

The term "widget" is equivalent to "web component", it's a way to display an independent dynamic component inside a website. The "widget" approach is similar to the old-fashion _iframe_, but is more flexible and adapted to modern web than the latter.

## Gitribute relies on Git providers

The very difference with proprietary solutions (like GoogleSheet or Airtable) or with equivalent open sourced solutions (like [nocoDB](https://www.nocodb.com/) or [Baserow](https://baserow.io/)) is that the data you edit with Gitribute is not stored on our servers. Your data is where you want it to be, on your own Gitlab or Github organization.

So **Gitribute does not have its own backend server**, but relies only on [Gitlab](https://gitlab.com/), [Github](https://github.com/), or [Mediawiki](https://www.mediawiki.org/wiki/MediaWiki) APIs. It means if you already have your own Gitlab account (or better, your own Gitlab instance), you won't have to rent a server for your database, let it on Gitlab, it already does a lot : versionning, authentication, pull requests...

This way your data stays protected, and you can manage the incoming contributions as you'd manage many pull requests.

## No account to contribute

Gitribute uses the [tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) system provided by Github or Gitlab to "commit" and contribute to some data stored on one of those git providers.

To avoid asking to your grandpa or your grandma creating an account on those providers and create their own personal tokens, **Gitribute uses a "ghost user token" (or an individual one)**.

The other thing necessary is to set your repo and its branches on Github or Gitlab to authorize this "ghost user token". Basically you don't want this token to be allowed to push on your main branch for instance...

To sum up when you set up your Gitribute widget you have to :

- 1/ create a default token
- 2/ set up the target repo to allow this token to create contributions (to create branches, but not to the main one)
- 3/ you can inject this default token in the widget (either from an `.env` variable or directly from the frontend).

That way an **user can push commits anonymously, without having to create its own account**, they also can use their own token, your data stays protected, and you - the dataset's owner - keep the control of who or what can write on it.

It's a bit of a hack, but the "ghost user" trick is not that much complicated.
