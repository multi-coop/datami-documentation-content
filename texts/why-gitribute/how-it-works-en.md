
# How does it work ?

## Gitribute is a widgets system

Gitribute is a web application providing a serie of "widgets". It means that **you could integrate it inside any website**, and you don't have to rely on a centralized website to use any of our widgets.

The term "widget" is equivalent to "web component", it's a way to display an independent dynamic component inside a website. The "widget" approach is similar to the old-fashion _iframe_, but is more flexible and adapted to modern web than the latter.

## Gitribute relies on Git providers

The very difference with proprietary solutions (like GoogleSheet or Airtable) or with equivalent open sourced solutions (like nocoDB or Baserow) is that the data you edit with Gitribute is not stored on our servers. Your data is where you want it to be, on your own Gitlab or Github organization.

So **Gitribute does not have its own backend server**, but relies only on Github / Gitlab, or Mediawiki APIs. It means if you already have your own Gitlab account (or better, your own Gitlab instance), you won't have to rent a server for your database, let it on Gitlab, it already does a lot : versionning, authentication, pull requests...

This way your data stays protected, and you can manage the incoming contributions as you'd manage many pull requests.

## No account to contribute

Gitribute uses the token system provided by Github or Gitlab to "commit" and contribute anonymously to the data. 

When you set up your Gitribute widget you have to 1/ create a default token, 2/ set up the target repo to allow this token to create contributions (to create branches, but not to the main one), 3/ you can inject this default token in the widget.

That way an **anonymous user can push commits without having to create its own account**, but your data stays protected and you keep the control of who can write on it.

It's a bit of a hack, but it's also that simple.
