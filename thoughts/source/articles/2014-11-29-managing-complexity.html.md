---
title: "Managing Complexity: Spelunky vs League of Legends"
date: 2014-11-29
tags: interfaces, experience design, game, complexity
---

I'm not afraid of complexity. As I've mentioned in the past, I love learning new things across many different domains, from mathematics to art to experience design. However, some things are easier to learn than others because of their mental models.

It is easy to learn things that behave in accordance with your expectations, and learning something new that builds on your existing understanding of the world is relatively simple. Learning something that doesn't is much harder. Someone who speaks two romance languages probably won't have as much trouble learning a new romance language as learning Chinese, for example. Someone who experiences math as formula memorization probably won't be able to apply Calculus outside of the classroom context within which they learned it.

A few days ago, I went to a Thanksgiving party, helped make and eat lots of great food, and played digital games with some of my friends. Among them were Spelunky and a 5v5 game of League of Legends (a MOBA commonly known as LOL).

Spelunky and LOL are fantastically complex. They each have many items and characters, each with different properties that substantially affect gameplay.

While becoming proficient at these games is quite challenging, the different ways in which they manage complexity makes Spelunky much easier to understand than LOL, and I think it has a much better overall design as a result. Why does Spelunky excel where LOL falls short?

1. Consistency

	To be consistent, a system has to follow its own rules and conventions. Spelunky is very consistent. Treasure chests always contain items. Gold bars give you a predictable amount of gold. You can only carry one thing in your hands. The environment is deadly. Even though every level is procedurally generated, it will always have one exit that leads to the next level. Every game has the same progression of stages.

	LOL has problems with consistency, especially with respect to items and the item shop:

	![Item Shop](2014-11-29-managing-complexity/ItemShop.jpg)

	LOL has many different items that all fall into different categories. The most important ones (from what I can tell as a first-time player) are consumable (single-use), passive (always in-use), or active (need to be triggered with an associated cooldown).

	However, the item shop doesn't use that classification for items. All the items look consistent even though they aren't. Players can switch to the list of all items to see this:

	[![All Item Shop Items](2014-11-29-managing-complexity/ItemShopAll.jpg)](https://www.youtube.com/watch?v=kdELk30I8qE)

	Since LOL is a fast-paced game of team competition, the only way to make effective item choices is to memorize the descriptions of the items to determine how they work when the game isn't running.

	Even more problematic is the "trinket" slot next to the 6 other item slots. A certain type of item, called a trinket/ward can only fill that one spot. Again, the store presents this item type consistently with the others. When I had filled 6 of my item slots, I couldn't understand why I couldn't buy another item even though I still had an empty slot. Since 6 of my slots were filled, the only visual distinction (the low-contrast eye emblem) failed to help me differentiate the function of the 7th slot from the others.

2. Affordances

	An affordance is part of a system that broadcasts its use by its form. Door plates afford pushing while vertical door handles afford pulling. The spikes in Spelunky look particularly deadly -- and they are. The only locked chest in Spelunky has a large golden lock with a matching golden key, and the purpose of the key is evident from its appearance.

	LOL has many poor affordances. Why does clicking on the store (which looks similar to the other buildings) make a modal dialog fill the screen, but clicking on the other buildings does not? Why do radar dishes on the ground explode when you get close to them when real radar dishes are used to scan objects at a distance?

3. Feedback

	True learning comes at the price of repeated failure. When something doesn't behave as you expect, you adjust your expectations based on your experiences. When a system encourages failing fast and provides good feedback that helps you understand your mistakes, you can build a better mental model of the system more quickly.

	Spelunky is a brutal game; death means restarting from the beginning. However, it associates every failure with the feedback you need in order to prevent making the same mistake again. Since every playthrough is different but pits you against a new configuration of the same obstacles, the game encourages true learning rather than memorizing a sequence of actions.

	Theoretically, LOL has a framework for providing much more relevant feedback than Spelunky because death means respawning back at the base. In fact, LOL does use feedback to manage complexity more effectively than consistency and affordances. LOL displays a death recap modal after every death. While this modal is probably extrordinarily useful to intermediate players, it didn't help me, as a beginner, understand many of my deaths because they were so sudden and revolved around placement as much as on the abilities of the other players. I think LOL beginners would benefit from a death replay similar to Towerfall Ascension, a game that also has very rapid deaths.

	![LOL Death Recap](2014-11-29-managing-complexity/DeathRecap.jpg)
	[![Towerfall Death Recap](http://i.imgur.com/zIPk1sU.gif)](http://towerfallr.tumblr.com)


Spelunky is an original title while League of Legends was inspired by a mod of Warcraft III called Defense of the Ancients. LOL is built around mental models that don't make much sense in the context of a standalone game. Consequently, it would probably be much harder to perfect LOL than to create a much better game by making a completely original MOBA (a path a number of other games have attempted). Nonetheless, I think LOL could be substantially improved with more thought given to consistency, affordances, and feedback while still meeting the needs of its legacy userbase.