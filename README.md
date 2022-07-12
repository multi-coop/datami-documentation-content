# GITRIBUTE DOCUMENTATION CONTENT

Website : https://gitribute-docs.multi.coop

This repo contains all contents for the gitribute's documentation website, including the site's architecture : website name, locales, navbar, routes, footers, images, and text contents...

Thoses contents are organized so they could be deployed as a website, thanks to a softawre developped by the digital cooperative **[multi](https://multi.coop)**.

---

## Render those contents as a websitte

🚀 &nbsp; Here you'll find the [**"multi-site-app" source code**](https://github.com/multi-coop/multi-site-app) to deploy the `.md` contents contained in this repo.

---

## Organisation

This repo is organized in the following order :

```env
.
├── README.md
├── LICENCE.md
├── config folder: to deploy a website with the `multi-site` app
│   ├── global.md : global config file (md and yaml head)
│   ├── navbar.md : config file for navbar butttons and links (md and yaml head)
│   ├── route.md : config file for routes (md and yaml head)
│   └── footer.md : config file for footer links (md and yaml head)
├── images folder: contains images
├── texts folder : contains all markdown files, including 

```

---

## Deployment

The contents are deployed with Netlify 

- Test deploy : [![Netlify Status](https://api.netlify.com/api/v1/badges/5a774814-2a6a-4da7-a8b5-1cc3d654df2a/deploy-status)](https://app.netlify.com/sites/multi-site-app-test/deploys)
- Official deploy : [![Netlify Status](https://api.netlify.com/api/v1/badges/5be5abcb-7667-4b96-b1d1-952839f70c2f/deploy-status)](https://app.netlify.com/sites/multi-website/deploys)

---

## Mini server for local development

A mini server is writen in the `server.py` to serve this folder's files, so we could test and develop locally while running [multi-site-app]()

To install the mini-server :

```sh
pip install --upgrade pip
python3 -m pip install --user virtualenv
python3 -m venv venv
source venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

or

```sh
sh setup.sh
source venv/bin/activate
```

To run the server on `http://localhost:8800`:

```sh
python server.py
```

or

```sh
sh run_server.sh
```

Files will be locally served on :

- `http://localhost:8800/content/<path:folder_path>/<string:filename>`
- `http://localhost:8800/statics/<path:folder_path>/<string:filename>`

---

## Contributions

If you want to propose somme enhancements to our content please make pull requests against the `main` branch. We will review that with great pleasure :)

You can also add issues directly in the reop, or add notes or issues from our [gitlab "board" page](https://gitlab.com/multi-coop/gitribute-documentation-content/-/boards).

---

## Notes / tutorials' section images

Here are the links to the source documents (slides) we used to create the tutorials's images : 

- [Gitribute tutorial - 01](https://docs.google.com/presentation/d/1hS5GqXxUJzquXDgO4Ch8O3klNekf-Ih-MNbJ8Ikp45M/edit#slide=id.g13be72e9310_0_24)
- [Gitribute tutorial - 02](https://docs.google.com/presentation/d/1DjJGQn80bHzxpNdMHIufwLLaUB3lJVPqvMVGpSRScb0/edit#slide=id.p)
