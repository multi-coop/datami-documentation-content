# Architecture & sketches

How do you switch from :

> — _"Hey, how should use Git more in frontend projects ?"_
 
 to :
 
> — _"[Sir, do you have a minute to speak about Gitribute ?](https://www.youtube.com/watch?v=sghOYbR_fXA&ab_channel=TikTokTaciousShorts)"_

_There's no wizard jizz in [making stuff](https://www.youtube.com/watch?v=N4IfPtl3W_M&ab_channel=exurb1a), [only a lot of engineering](https://www.youtube.com/watch?v=qE0UimODxNg&ab_channel=exurb1a)_

This section focuses on the early works and brainstorming processes that lead to make Gitribute someting more than a good idea : [a plan, an architecture](https://agileflow.co.uk/2016/06/08/agile-planning/).

Brace yourself for a little trip...

## Sketches & wireframes

Gitribute have some _core_ components and functions, reusable among other components.

The _core functions_ are mainly contained in the `utils` folder : requesting APIs, converting a raw csv to a javascript object, etc...

The front data are stored in a nodal _vuex store_ : locale, user infos, current branch, file infos, etc... are stored there.

Finally some _complex components can be re-used_ by others such as the `EditCell` or `GitributeTable` ones, reusable by `explowiki` or `gitfile` high-level components or within a table.

We are proud (and a bit ashamed too) to apply `#passionSchema` to our brainstorming process...

![SCHEMA-GITRIBUTE-02](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-schema-02.png)

> _**Note** : More about the widgets in the **["Widgets > Overview"](/docs-widgets-overview)** section_
