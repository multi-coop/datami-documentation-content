### Notes à propos du fichier `.env`

Gitribute utilise quelques variables d´environnement pour fonctionner correctement :

```env
DEFAULT_GITHUB_TOKEN=<YOUR-GITHUB-USER-TOKEN>
DEFAULT_GITLAB_TOKEN=<YOUR-GITLAB-USER-TOKEN>
VUE_APP_GITRIBUTE_DEPLOY_DOMAIN=gitribute.multi.coop
VUE_APP_GITRIBUTE_DOCUMENTATION=gitribute-docs.multi.coop
```

- `DEFAULT_GITHUB_TOKEN` : le token utilisateur par défaut pour requêter l´API de Github
  - 🤫 ... c´est secret...
- `DEFAULT_GITLAB_TOKEN` : le token utilisateur par défaut pour requêter l´API de Gitlab
  - 🤐 ... on vous a dit, c´est tooop secret...
- `VUE_APP_GITRIBUTE_DEPLOY_DOMAIN` : le nom de domaine où vous déployez votre instance, pour que le bouton copier-coller fonctionne correctement
  - valeur par défaut : `gitribute.multi.coop`
- `VUE_APP_GITRIBUTE_DOCUMENTATION` : le domaine pour la documentation Gitribute
  - valeur oar défaut : `gitribute-docs.multi.coop`
