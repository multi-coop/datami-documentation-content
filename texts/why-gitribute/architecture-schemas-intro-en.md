
## Schemas & wireframes

Gitribute have some _core_ components and functions, reusable among other components.

The _core functions_ are mainly contained in the `utils` folder : requesting APIs, converting a raw csv to a javascript object, etc...

The front data are stored in a nodal _vuex store_ : locale, user infos, current branch, file infos, etc... are stored there.

Finally some _complex components can be resued_ by others such as the `EditCell` or `GitributeTable` ones, reusable by `explowiki` or `gitfile` high-level components or within a table.

We are proud (and a bit ashamed too) to apply the `#passionSchema` hashtag to our brainstorming process...

![SCHEMA-GITRIBUTE-02](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-schema-02.png)

---
