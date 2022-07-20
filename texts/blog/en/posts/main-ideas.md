---
title: Main ideas
tags: [ R&D, ideas ]
created: 17/07/2022
author: Julien Paris
---

Gitribute is designed as a light micro-service, letting you chose among a small collection of widgets you can reuse to **display the data you want**, **where you want**, and all that **for free**.

To make this possible we designed Gitribute as a pure frontend.

No backend in Gitribute's stack : too much maintenance, to expensive, a pain in the *** to say the least...

That said, if we wanted to visualize any data _**the data did need to come from somewhere, ain't it ?**_ 

### Git providers as databases

As developpers ourselves we have a daily and extensive use of Github or Gitlab, and let's agree to say those are AMAZING infrastructures ! 

Every day, we (I mean we developpers) enjoy those services :

- Version management ;
- Secure authentication ;
- APIs ;
- Robust and scalable infrastructures ;
- etc...

So if we - developers - store our data and code over there the whole time, let's keep it that way and let you enjoy this same relief.

**Gitribute's prefered database is "no" database in a common sense, so let it be Github or Gitlab**. There is an extensive documentation to know how to get or modify the data via their APIs.

The other important feature those "Git providers" deliver us is the ability to create `branches` and `pull requests`. Think of it as "contribution proposals" sent to a dataset's owner : **the owner can accept, reject, or amend a proposal before merging it to its dataset**.

We consider the "pull request" - and the moderation it leads to - as the more polite way to collaborate : propose something to someone, and let they chose to accept it or not.

That kind of contribution process have _[manners](https://idiomorigins.org/origin/manners-maketh-man)_.

### Basic interoperabilty

In the "tech" world - and especially in the open source movement - "full interoperability" is the Graal we all crave for. Http protocol, RSS, XML, Semantic web, activityPub, were or still are great inventions reaching for this goal.

Digital world is full of standards, tools, frameworks, languages, uses, etc... Some standards are adopted and widely accepted, other are struggling to become so.

Many actors (corporations or else) fight to defend their own standard(s), which is always better than the competitor's standard, and it goes on and on...

_A little though here for the mini-disc standard, the blu-ray, and many other standards who died fiercly... And a less tender though for Apple and their habit to change plugs shape every ten minutes._

But this tech world could seem... you know... kinda very technical, at least for "normal" people.

Try to explain the pros and cons of semantic web to your grandpa' or grandma', I dare you.

So instead of "extensive interoperability" we prefer to imagine Gitribute posture about this topic as reaching for the **"best interoperability between noobs & machines"**, as the combination of :

- **"What people commonly use"** : excel spreadsheets, gsheet, airtable... for instance.
- **"What could be read by any machine today"** : `json`, `csv`, `markdown` ...

We won't say Gitribute is interoperable, it's just it tries to use standards having the best chance to be commonly used by human and machines **altogether**...

### Data and schema agnostic

Data comes in every shapes and forms. 

Usually - if you did not produce this data - they come in forms you don't expected... at all...

A key idea in Gitribute is it should display **any data in a common format**, disregarding what's inside : **Gitribute tries to stay "data agnostic"**.

Taking this as the ground step for displaying data, we also wanted to append - if and only if necessary - more options so your data could be shown as beautiful you imagined it.

Knowing the more common way to write data were the "table" format, we included very early in our developments a keystone feature allowing **to apply a [table schema](https://specs.frictionlessdata.io/table-schema/)** and other custom properties **to your `csv` or `tsv` files**.

### A widgets collection...

Gitribute is constituted by of a collection of widgets you can use separatly or compose with.

We didn't want to centralize a service and/or your data.

After all _you_ sweat to produce it, _you_ own it, therefore _you_ are responsible for it.

But if you want to **valorize** and **refine your data** the best chance to do so is to **let other people reuse and contribute to YOUR data**.

Sharing. [This is the way](https://www.youtube.com/watch?v=uelA7KRLINA&ab_channel=Gabriel)...

"Sharing data" means letting people reuse YOUR data where THEY want.

Widgets are the solution we though of to allow this, without the risk to lose entirely the control over your data :

- The data source stays in _your_ repository ;
- But _anybody_ can make a proposal...

Let's dare say again that **"[Manners maketh commoner](https://www.youtube.com/watch?v=hUtNQAdhIR4&ab_channel=RodStickler)...** _you know what that means ?_"

### ... For noobs

We believe you don't have to be an engineer to have or share your knowledge.

Knowledge _is_ data, and likewise it comes in all shapes and forms.

But in a digital world **interfaces** are the key to make possible the expression and sharing of people's knowledge.

The last - and perhaps more important - principle we follow is the **major importance of UX and UI design**.

We won't emphasize this enough : **a good design is a design you don't have to ask or care about**.

Now let's do our best to fulfill this promise...
