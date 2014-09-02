---
title: Set, System Analysis
date: 2014-09-01
tags: constraints, system analysis
---

I'm studying how systems work at [USC's Interactive Media and Games Division](http://interactive.usc.edu), and I decided to explore how the design of Set cards is tied to the rules for the game. I initially wrote this with no resources other than a deck of Set cards and a Python interpreter, but I have since amended some of my initial impressions after reading [this](http://en.wikipedia.org/wiki/Set_(game)).

We can use playing cards in myriad ways, including building card castles, throwing cards at targets, using cards to propel projectiles, floating cards down streams ala [Poohsticks](http://en.wikipedia.org/wiki/Poohsticks), laying cards side-by side like dominos, and bending cards to create three dimensional shapes.

[Set](http://en.wikipedia.org/wiki/Set_(game)) is a simple card game with a deck of 81 standard-size playing cards that are uniquely suited for exactly one purpose that doesn't involve the destruction of the cards: for playing the game of Set.

One side of each Set card bears the logo of the game on a matte surface, while the other is devoted to one or more large symbols displayed on a glossy white canvas.

The symbols on any given card can differ in the following ways:

- Quantity (each card has one, two, or three symbols)
- Color (a given symbol can be green, red, or purple, and all symbols on a card share the same color)
- Shading (symbols can be solid-colored, striped in parallel with the longest side of the card, or consist of empty - outlines, and all symbols on a given card share the same shading)
- Shape (each symbol on a card is either tilde-shaped, diamond-shaped, or capsule-shaped, and each symbol on a given card has the same shape)

Note that each of these four properties has exactly three variants, which allows for the `3`<sup>`4`</sup>`=81` unique cards in the deck.

Consequently, it would be impossible to play a standard match-2 game with a Set deck; by virtue of having three variants for each property, the game materials are optimized for 3-card combinations. The logo of the game reinforces this notion; it contains a visualization of stacks of three cards with different shading, calling to mind the card properties.
While there are `511920` unique 3-card combinations possible in a deck of Set cards, not all of these combinations can be meaningful. If every 3-card combination with at least one shared property variant were considered a "match," then around `36%` of the possible combinations would qualify, which would eliminate much of the depth present in the Set card game. Instead, a match, known as a "Set," occurs when each property varies either entirely or not at all. People playing the game compete to find and collect as many such Sets as possible.

The following three cards form a Set because they all have the same quantity variant but differ in every other property:

- `3-Green-Empty-Tilde`
- `3-Purple-Solid-Capsule`
- `3-Red-Shaded-Diamond`

These cards do not form a Set because two of the cards have the solid shading variant:

- `3-Green-Empty-Tilde`
- `3-Purple-Solid-Capsule`
- `3-Red-Solid-Diamond`

Only around 1% of the possible 3-card combinations are Sets. However, the probability of discovering a 3-card Set in a collection of `n` cards increases quite quickly with `n`.

These are the probabilities of a Set in a given collection of `n` cards drawn from the deck at random, at the start of the game (determined via numerical simulation in Python, using `100,000` samples for each `n`-card collection):

![Graph](2014-09-01-set-analysis/graph.png)

Card games typically involve cards held in the player's hands, but holding more than seven cards is ungainly, and there is only a 39% chance that seven random cards will contain a Set. Furthermore, the size and position of the symbols on the cards does not afford holding several of them in a hand; doing so obscures the property information which is integral to forming Sets. The cards are clearly designed to be placed face up on a level surface.

From the diagram above, we can see that we get increasingly diminishing returns in the probability that an initial collection of n cards will contain a Set for `n>10`. In fact, for `n=20` and greater, the probability is `100%`. When `n=12`, the quantity used in the game of Set, the probability is initially `97%` (although it quickly drops to about `93%` as the game progresses and Sets are removed and replaced with new cards from the deck). Furthermore, the average amount of Sets present in a collection increases rapidly with `n`. For the sake of challenging players to find Sets, `n` should never be too high, so `n=12` is a logical choice, although it does sometimes require the addition of new cards from the deck when no Sets are present (the rules to Set call for the addition of three new cards in this situation, which ensures that the amount of face-up cards on the table is always divisible by the amount of cards in a Set). Elegantly, `12` is `4x3`, the number of properties multiplied by the number of variants for each property.

Although there are several [Set variants](http://magliery.com/Set/SetVariants.html), I would argue that the cards for Set are perfectly designed to match the primary game for which they were created, and that many of these alterations oppose the simplicity of the core game and/or the design of the cards. For example, the variants frequently call for holding some cards in one's hand, removing cards, or adding betting tokens. Nonetheless, I applaud the ingenuity of the player base.
