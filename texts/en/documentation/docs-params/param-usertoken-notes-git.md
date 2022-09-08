
#### Notes about the `usertoken` parameter

The `usertoken` parameter is one of the most important features of this project. You will need a private token to push to a repository and make all the operations we want to automatize for an open contribution :

- **Create a new branch** againt a reference branch ;
- **Push a commit** to the new branch ;
- **Create a merge request** from the new branch onto the reference branch.

Our strategy to simplify those operations for 'normal' people (who does not give a s*** about git) was to create one or several "ghost users", so we could set the repositories' permissions and tokens in advance.

In order to deploy a Datami demo on a domain we chose to store those tokens on an `.env` file, based on the `example.env` file at the project's root. So you can have several strategies to inject a default token :

- create an `.env` file, but you will have to deploy your own instance of Datami ;
- copy-paste the html block, filling the widget's `usertoken` parameter ;
- leave all blank and ask your users to create their own tokens on Gitub or Gitlab...

So you can read more on those topics here =>

- More about **Gitlab** :
  - API documentation : [docs](https://docs.gitlab.com/ee/api/)
  - Create a private token : [docs](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html)
  - Manage permissions : [docs](https://docs.gitlab.com/ee/user/permissions.html)
- More about **Github** :
  - API documentation : [docs](https://docs.github.com/en/rest)
  - Create a private token : [docs](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
  - Manage permissions : [docs](https://docs.github.com/en/organizations/managing-access-to-your-organizations-repositories/repository-roles-for-an-organization)

---
