
## Contribute anonymously (if you feel a bit shy)

Gitribute uses the [tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) system provided by Github or Gitlab to "commit" and contribute to some data stored on one of those git providers.

To avoid asking to your grandpa' or your grandma' creating an account on those providers, and to avoid asking them to create their own personal tokens, **Gitribute uses a default "ghost user token" (or an individual one)**.

If you want anonymous contribution against your data with Gitribute, it is necessary to set your repo and its branches on Github or Gitlab as authorizing this "ghost user" token. Basically, you don't want this token to allow "pushes" on your `main` branch for instance...

To sum up, when you set up your Gitribute widget from scratch you have to :

- 1/ Create your own "ghost user" / default token
- 2/ Set up the target repo to allow this token to make contributions (create branches, but not pushes directly to your `main` branch)
- 3/ You can inject this default token in the widget (either from an `.env` variable or directly from the frontend).

That way, an **user can push commits anonymously, without having to create its own Github or Gitlab account**.

Users can also use their own token.

Your data stays protected on your Git provider, and you - the dataset's owner - keep the control of who can write on it and where.

It's a bit of a hack, but the "ghost user" trick is not that much complicated.

It's like letting your grandpa' or grandma' use your Netflix account...
