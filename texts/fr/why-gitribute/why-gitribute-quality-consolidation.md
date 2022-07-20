### Consolidation de données

Nous rencontrons de multiples cas où il peut être nécessaire de "consolider" un jeu de données, que ce soit en changeant une valeur incorrecte d'un champ, ou bien en vérifiant qu'une valeur respecte bien certains critères.

"_Consolider_" - de manière générale - signifie que vous avez besoin de modifier vos données pour les rendre plus "propres", plus "précises", ou plus "complètes", par exemple :

- [Géolocaliser une adresse](https://adresse.data.gouv.fr/csv) ; 
- [Valider qu'un jeu de données respecte un schéma](https://validata.fr/) ; 
- [Générer un identifiant unique ou UUID](https://heidi.etalab.studio) ;
- [Récupérer des informations publiques sur une société](https://api.gouv.fr/les-api/api-entreprise)
- ... ou [beauuuuuuucoup d'autres cas](https://api.gouv.fr/).

La consolidation peut concerner soit certaines entrées d'un tableur, soit le jeu de données au complet.

Enfin, le besoin de consolidation sur un jeu de données est en géral lié à un besoin "métier" spécifique, à une profession, à une thématique, à une organisation... Les cas et les combinatoires sont infinis.

Étant donnée cette infinité des cas où un.e utilisateur.rice aurait à consolider des données, l'intention de Gitribute est d'intégrer un système permettant de **déléguer la consolidation à des services tiers**, essentiellement des _APIs_ (*).

(*) _"API" pour "[Application Programming Interface](https://en.wikipedia.org/wiki/API)"_

Pour ce faire nous avons conçu une manière de configurer des requêtes à des APIs, requêtes que vous pouvez personnaliser en fonction des spécificités de tel ou tel jeu de données. **Gitribute laisse le.s propriétaire.s du jeu de données décider quelle API il.s souhaite.ent inclure dans un widget, vues les particularités du jeu de données**.

L'intégration d'un **service tiers de consolidation via API n'est pas écrit "en dur" dans Gitribute** : un widget Gitribute **nécessite une légère configuration** pour peupler le champ de [consolidation](/tutorial-edition).

Nous avons d'ores et déjà testé l'intégration de ces APIs tierces dans des widgets Gitribute :

- [API-entreprises](https://api.gouv.fr/les-api/api-entreprise) : permet de récupérer des informations publiques sur une organisation étant donné son numéro de SIREN ;
- [Base Adresse Nationale](https://adresse.data.gouv.fr/api-doc/adresse) : permet de récupérer la géolocalisation étant donné un code postale, adresse au format textuel... ;
- ... et bientôt bien d'autres.

> **Note** : Plus de détails sur la consolidation dans la partie **["Tutoriels > Éditer un document"](/tutorial-edition)**.
