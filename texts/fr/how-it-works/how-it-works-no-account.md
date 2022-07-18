
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
