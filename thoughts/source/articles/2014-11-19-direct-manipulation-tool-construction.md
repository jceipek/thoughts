---
title: "Direct Manipulation Tool Construction"
date: 2014-11-19
tags: interfaces, direct manipulation, user experience design
---

I've been busy exchanging skills with my classmates at [USC's graduate Interactive Media and Games Division](http://interactive.usc.edu). I taught Unity programming and learned prop making and baking:

![Skitter Mask](2014-11-19-direct-manipulation-tool-construction/mask.jpg)

![Journey Cake](2014-11-19-direct-manipulation-tool-construction/cake.jpg)

Both of these arts revolve around direct manipulation; you bend foam and fondant, cut components into the right shape, and use tools to shape your work.

It's important to note that the end result rarely matches the original designs, and that this is a Very Good Thing. Working on physical objects involves many implicit constraints that shape the end result and inspire solutions that would otherwise never have been considered.

This is the power of direct manipulation: constantly getting feedback as you are working and changing your work in response to that feedback. Interfaces (and more generally, systems) without constant feedback are inherently limited to an initial design, which is a problem because, as you work, you often realize that the original design is flawed. For a commonly accepted example of this in software and engineering, consider the derided [Waterfall](http://en.wikipedia.org/wiki/Waterfall_model) development technique.

Working with physical materials, I constantly felt the urge to improvise. If I didn't have a tool I thought I would need, I would take a minute or two to create an ad-hoc tool for the specific task I was working on at the time. How can I bend this part into the shape that I want? I can just use a bowl. I'm missing a rolling pin small enough to flatten this gum paste, so I'll use this thin wooden dowel. How can I draw a large perfect circle without a compass? I'll tape two pencils to a wooden board.

I think the ease with which you can construct useful one-off tools through direct manipulation is sorely lacking in the digital space. Yes, some interfaces are scriptable through simple programming languages like Lua and Python, but the barrier to entry is much higher than taping miscellany together. Moreover, since it is so hard to make a tool to begin with, once you have decided to make it, you are much more inclined to waste the time you could have been using to make the thing you were working on by making the tool 'reusable' even if you'll only actually need it once.

The closest analogue I can think of to direct manipulation tool construction in the software space is a recorded macro that can automate repetitive actions. Unfortunately, they are a poor substitute for the flexibility of making your own tools.

While our software involves so little user feedback and so much indirect manipulation of hidden state (see Bret Victor's [Learnable Programming)](http://worrydream.com/LearnableProgramming/)), I don't think we can do much better than macros and scripting languages. If you can directly manipulate something, you can have many more opportunities to easily make your own tools. Play [Euclid: The Game](http://euclidthegame.com) to get an inkling of what that might be like.