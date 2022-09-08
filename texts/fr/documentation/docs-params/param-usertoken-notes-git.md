
#### Notes à propos du paramètre `usertoken`

Le paramètre `usertoken` est un des paramètres les plus importants du projet Datami. Vous avez besoin d'un _token_ (ou "jeton") d'accès pour effectuer des opérations sur vos données. C'est par le biais de ce _token_ qu'il est possible d'automatiser un certain nombre d'opérations _via_ les APIs de services Git et de permettre une contribution ouverte avec Datami.

- **Créer une nouvelle branche** depuis la branche de référence du fichier source ;
- **Créer un _commit_** sur cette nouvelle branche ;
- **Créer une _merge request_** depuis la nouvelle branche vers la branche de référence.

Notre stratégie pour simplifier ces opérations pour des gens qu'on dira "normaux" (qui se fichent de Git comme Boris Johnson se fiche de son coiffeur) a été de créer un ou plusieurs "utilisateurs fantômes", de sorte qu'on puisse configurer des _tokens_ et les permissions sur un _repo_ à l'avance.

Afin de déployer une instance de Datami (par exemple sur http://gitribute.multi.coop) on pourra choisir d'injecter un _token_ d'utilisateur fantôme dans les variables d'environnement (ou dans un fichier `.env` à la racine par exemple). On a ainsi plusieurs stratégies pour injecter ce _token_ par défaut :

- Créer un fichier `.env`, mais cela suppose que vous déployiez votre propre instance de Datami ;
- Faire un copier-coller du bloc `html`d'un widget existant,et de remplacer la valeur du paramètre `usertoken` du widget par un _token_ de votre choix ;
- Laisser ce paramètre vide et demander aux utilisateurs.rices du widget de créer leur propre compte et _token_ sur Github ou Gitlab...

Davantage de documentation sur le sujet des _tokens_ personnels d'accès ici => 

- Plus d'infos sur **Gitlab** :
  - Documentation de l'API : [docs](https://docs.gitlab.com/ee/api/)
  - Création d'un _token_ personnel : [docs](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html)
  - Gestion des permissions sur un _repo_ : [docs](https://docs.gitlab.com/ee/user/permissions.html)
- Plus d'infos sur **Github** :
  - Documentation de l'API : [docs](https://docs.github.com/en/rest)
  - Création d'un _token_ personnel : [docs](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
  - Gestion des permissions sur un _repo_ : [docs](https://docs.github.com/en/organizations/managing-access-to-your-organizations-repositories/repository-roles-for-an-organization)

---
