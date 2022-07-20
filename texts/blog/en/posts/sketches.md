---
title: Architecture & sketches
tags: [ tech, R&D ]
created: 17/07/2022
author: Julien Paris
---

How do you transition from :

> — _Hey, how should use Git more in frontend projects ?_

 to :

> — _[Sir, do you have a minute to speak about Gitribute ?](https://www.youtube.com/watch?v=sghOYbR_fXA&ab_channel=TikTokTaciousShorts)_

This section focuses on the early works and brainstorming processes that lead to make Gitribute someting more than a good idea : [a plan, a roadmap, an architecture allowing being "agile"](https://www.linkedin.com/pulse/agile-approach-methodology-carlo-occhiena/).

_There's no wizard jizz in [making stuff](https://www.youtube.com/watch?v=N4IfPtl3W_M&ab_channel=exurb1a), [only a lot of engineering](https://www.youtube.com/watch?v=qE0UimODxNg&ab_channel=exurb1a)_

Brace yourself for a little trip...

## Sketches & wireframes

Gitribute have some _core_ components and functions, reusable among other components.

The _core functions_ are mainly contained in the `utils` folder : requesting APIs, converting a raw csv to a javascript object, etc...

The front data are stored in a nodal _vuex store_ : locale, user infos, current branch, file infos, etc... are stored there.

Finally some _complex components can be re-used_ by others such as the `EditCell` or `GitributeTable` ones, reusable by `explowiki` or `gitfile` high-level components or within a table.

We are proud (and a bit ashamed too) to apply `#passionSchema` to our brainstorming process...

![SCHEMA-GITRIBUTE-02](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-schema-02.png)

> **Note** : More about the widgets in the **["Documentation > Overview"](/docs-widgets-overview)** section

## Components wireframes

Gitribute started with an idea, while sitting at a cafe near Paris, outside, with a bright sun on a sunny sunday. No laptop around.

We started designing Gitribute a bit in an "old-fashion" way : with a pen and a paper. No fancy tools like Figma at this precise moment at the cafe.

Keeping on with this approach the "wireframes" you will se below are more ideas or sketches than real design canvases. But drawing can still be relevant and more straight-to-the-point, even in the digital world.

After all, how did they build those pyramids, any building, any painting, anything needing a bit of planning... before the computers ?

### Widget for `md` preview and edition

We were inspired a lot by [HedgeDoc](https://hedgedoc.org/) and [Hackmd](https://hackmd.io) interfaces.

**The only thing we added was `diff` view**, as an intermediary between preview and edition.

![GITRIBUTE-WIREFRAME-EDIT-MD-01](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-wireframe-edit-md-01.png)

> **Note** : More about editing and diff view in the **["Tutorials > Edit a document"](/tutorial-edition)** section

## Dialog before saving changes (send a contribution)

To "save" one's changes over a data, we use Git for version control.

More precisely we rely on Git service providers like Github or Gitlab. 

The [Git syntax](https://en.wikipedia.org/wiki/Git) could seem a bit tricky at first sight.

"Merge requests", "branches" and this kind of weirds notions are not terms your grandma' or grandpa' are _really_ interested in.

_( If they seem to, call a doctor.)_

At the contrary _"saving"_, a document became something quite usual for most humans in the XXIth century.

**"Contributing" lays halfway between the tech world and common cultural habits.**

The challenge was to find an "user path" - and a design - to express this intention **simply** and **honestly** :

- "Simply" by avoiding any dispensable information, straight to the point ;
- "Honestly" by letting the user learn step by step what those weird terms (tooltips), keeping technical information in the background (in another tab, but accessible), etc...

![GITRIBUTE-WIREFRAME-DIALOG_SAVE-01](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-wireframe-commit_dialog-01.png)

That said it is not completly useless to have a basic understanding of Git, and [many](https://www.atlassian.com/git) [websites](https://learngitbranching.js.org/?locale=fr_FR), [videos](https://www.youtube.com/watch?v=2ReR1YJrNOM&ab_channel=ProgrammingwithMosh), or sometimes people are available to learn the basics.

> **Note** : More about contributing in the **["Tutorials > Contribute to a document"](/tutorial-contribution)** section

<br>
<br>
