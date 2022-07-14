### Notes about the `.env` file

Gitribute uses some environment variables to work perfectly :

```env
DEFAULT_GITHUB_TOKEN=<YOUR-GITHUB-USER-TOKEN>
DEFAULT_GITLAB_TOKEN=<YOUR-GITLAB-USER-TOKEN>
VUE_APP_GITRIBUTE_DEPLOY_DOMAIN=gitribute.multi.coop
VUE_APP_GITRIBUTE_DOCUMENTATION=gitribute-docs.multi.coop
```

- `DEFAULT_GITHUB_TOKEN` : an user token allowing to use the github API
  - 🤫 ... it's a secret...
- `DEFAULT_GITLAB_TOKEN` : an user token allowing to use the gitlab API
  - 🤐 ... we told you already, it's tooop secret...
- `VUE_APP_GITRIBUTE_DEPLOY_DOMAIN` : the domain name you deploy your instance on, so the copy-paste button works correctly
  - default value : `gitribute.multi.coop`
- `VUE_APP_GITRIBUTE_DOCUMENTATION` : the domain for Gitribute documentation
  - default value : `gitribute-docs.multi.coop`
