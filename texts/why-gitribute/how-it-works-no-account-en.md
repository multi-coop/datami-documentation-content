
## Contribute anonymously (if you're shy)

Gitribute uses the [tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) system provided by Github or Gitlab to "commit" and contribute to some data stored on one of those git providers.

To avoid asking to your grandpa' or your grandma' creating an account on those providers and create their own personal tokens, **Gitribute uses a "ghost user token" (or an individual one)**.

The other thing necessary is to set your repo and its branches on Github or Gitlab to authorize this "ghost user token". Basically you don't want this token to be allowed to push on your main branch for instance...

To sum up when you set up your Gitribute widget you have to :

- 1/ create a default token
- 2/ set up the target repo to allow this token to create contributions (to create branches, but not to the main one)
- 3/ you can inject this default token in the widget (either from an `.env` variable or directly from the frontend).

That way an **user can push commits anonymously, without having to create its own account**, they also can use their own token, your data stays protected, and you - the dataset's owner - keep the control of who or what can write on it.

It's a bit of a hack, but the "ghost user" trick is not that much complicated.
