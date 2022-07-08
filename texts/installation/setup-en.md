# Quickstart for developpers

Gitribute is a frontend project developped with Vue.js (Javascript).

If you feel curious about our stack check **[this page](/stack)**.

Here are the basics steps to do for local development.

---

## Project setup

```bash
nvm use
npm install
cp example.env .env
```

### Notes about the `.env` file

Gitribute uses some environment variables to work perfectly :

```env
DEFAULT_GITHUB_TOKEN=<YOUR-GITHUB-USER-TOKEN>
DEFAULT_GITLAB_TOKEN=<YOUR-GITLAB-USER-TOKEN>
VUE_APP_GITRIBUTE_DEPLOY_DOMAIN=gitribute.multi.coop
```

- `DEFAULT_GITHUB_TOKEN` : an user token allowing to use the github API
  - 🤫 ... it's a secret...
- `DEFAULT_GITLAB_TOKEN` : an user token allowing to use the gitlab API
  - 🤐 ... we told you already, it's tooop secret...
- `VUE_APP_GITRIBUTE_DEPLOY_DOMAIN` : the domain name you deploy your instance on, so the copy-paste button works correctly
  - default value : `gitribute.multi.coop`

---

### Compiles and hot-reloads for development

Once the dependencies are installed you can run the Vue.js' hot-reload server for local development :

```bash
npm run serve
```

By default Gitribute will run on `https://localhost:8080`

---

### Compiles and minifies for production

For a production build you need to run :

```bash
npm run build
```

---

### Lints and fixes files

Linting is sooo useful, don't forget to switch on your `autofix`...

```bash
npm run lint
```

---

### Run your unit tests

We are a bit short for now on the topic of testing, but - cross my heart - we'll work on it soon...

```bash
npm run test:unit
```
