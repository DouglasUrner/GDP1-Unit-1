# Formal Abstract Design Tools

**Doug Church, 16 July 1999**

What is a modern computer game made of? It fuses a technical base with a vision for the player's experience. All of the disciplines involved (design, art, audio, levels, code, and so on) work together to achieve this synthesis.

In most disciplines, industry evolution is obvious: The machines we play on are far more powerful, screens have better resolution and more colors, paint and modeling tools are more sophisticated, audio processing is faster, and sound cards are more capable. Technical issues not even in our vocabulary ten years ago are solved and research continues with essentially infinite headroom. The technical base on which games stand (game code and content creation tools) is evolving.

Across all genres and companies, we build on our own and others' past ideas to expand technical limits, learn new techniques and explore possibilities. Ignoring an anomaly or two, no single company or team would be where it is now had it been forced to work in a vacuum.

Design, on the other hand, is the least understood aspect of computer game creation. It actualizes the vision, putting art, code, levels, and sound together into what players experience, minute to minute. Clever code, beautiful art, and stunning levels don't help if they're never encountered. Design tasks determine player goals and pacing. The design is the game; without it you would have a CD full of data, but no experience.

Sadly, design is also the aspect that has had the most trouble evolving. Not enough is done to build on past discoveries, share concepts behind successes, and apply lessons learned in one domain or genre to another. Within genres (and certainly within specific design teams), particular lines have evolved significantly. But design evolution still lags far behind the evolution of overall game technology.

## How Do We Talk About Games?

The primary inhibitor of design evolution is the lack of a common design vocabulary. Most professional disciplines have a fairly evolved language for discussion. Athletes know the language of their sport and of general physical conditioning, engineers know the technical jargon of their field, doctors know Latin names for body parts and how to scribble illegible prescriptions. In contrast, game designers can discuss "fun" or "not fun," but often the analysis stops there. Whether or not a game is fun is a good place to start understanding, but as designers, our job demands we go deeper.

We should be able to play a side-scrolling shooter on a Game Boy, figure out one cool aspect of it, and apply that idea to the 3D simulation we're building. Or take a game we'd love if it weren't for one annoying part, understand why that part is annoying, and make sure we don't make a similar mistake in our own games. If we reach this understanding, evolution of design across all genres will accelerate. But understanding requires that designers be able to communicate precisely and effectively with one another. In short, we need a shared language of game design.

## A Language Without Borders

Our industry produces a wide variety of titles across a range of platforms for equally varied audiences. Any language we develop has to acknowledge this breadth and get at the common elements beneath seemingly disparate genres and products. We need to be able to put our lessons, innovations, and mistakes into a form we can all look at, remember, and benefit from.

A design vocabulary would allow us to do just that, as we could talk about the underlying components of a game. Instead of just saying, "That was fun," or "I don't know, that wasn't much fun," we could dissect a game into its components, and attempt to understand how these parts balance and fit together. A precise vocabulary would improve our understanding of and facility with game creation.

This is something we already do naturally with many technical innovations, since they are often much easier to isolate within a product or transfer to another project. A texture mapper or motion capture system is easily encapsulated. When everyone at the office gathers around some newly released game, major technical "evaluation" is done in the first five minutes: "Wow, nice texture mapping," or "Those figures rock" or "Still don't have a sub-pixel accurate mapper? What is their problem?" or "Man, we have to steal that special effect." But when the crowd disperses, few observations have been made as to what sorts of design leaps were in evidence and, more importantly, what worked and what didn't.

Design is hard to point at directly on a screen. Because of this, its evolutionary path is often stagnant. Within a given genre, design evolution often occurs through refinement. This year's real-time strategy (RTS) games clearly built on last year's RTS games. And that will continue, because design vocabulary today is essentially specific to individual games or genres. You can talk about balancing each race's unit costs, or unit count versus power trade-offs. But we would be hard pressed to show many examples of how innovations in RTS games have helped role-playing games (RPGs) get better. In fact, we might have a hard time describing what could be shared.

These concerns lead to the conclusion that a shared design vocabulary could be very useful. The notion of "Formal Abstract Design Tools" (or FADT, as they'll be referred to from here on) is an attempt to create a framework for such a vocabulary and a way of going about the process of building it.

Examining the phrase, we have: "formal," implying precise definition and the ability to explain it to someone else; "abstract," to emphasize the focus on underlying ideas, not specific genre constructs; "design," as in, well, we're designers; and "tools," since they'll form the common vocabulary we want to create.

"Design" and "tools" are both largely self-explanatory. However, some examples may help clarify "formal" and "abstract." For instance, claiming that "cool stuff" qualifies as a FADT violates the need for formality, since "cool" is not a precise word one can explain concretely — various people are likely to interpret it very differently. On the other hand, "player reward" is well defined and explainable, and thus works. Similarly, a "+2 Giant Slaying Sword" in an RPG is not abstract, but rather an element of one particular game. It doesn't qualify as a FADT because it isn't abstract. The general notion that a magic sword is based on — a mechanic for delivering more powerful equipment to the player — is, however, a good example of a FADT, so the idea of a "player power-up curve" might meet the definition above.

## Let's Create a Design Vocabulary — What Could Possibly Go Wrong?

Before we start investigating tools in more detail and actually look at examples, some cautionary words. Abstract tools are not bricks to build a game out of. You don't build a house out of tools; you build it with tools. Games are the same way. Having a good "player power-up curve" won't make a game good. FADT are not magic ingredients you add and season to taste. You do not go into a product proposal meeting saying "this game is all about player power-up curves." As a designer, you still have to figure out what is fun, what your game is about, and what vision and goals you bring to it.

But a design vocabulary is our tool kit to pick apart games and take the parts which resonate with us to realize our own game vision, or refine how our own games work. Once you have thought out your design, you can investigate whether a given tool is used by your game already. If it is, are you using it well, or is it extraneous? If it isn't used, should it be, or is the tool not relevant for your game? Not every construction project needs a circular power saw (sadly), and every game doesn't need every tool. Using the right tools will help get the shape you want, the strength you need, and the right style.

Similarly, tools don't always work well together — sometimes they conflict. The goal isn't to always use every tool in every game. You can use an individual tool in different ways, and a given tool might just sit in a toolbox waiting to see if it is needed. You, the designer, wield the tools to make what you want — don't let them run the show.

## Tools Would Be Useful — Where Do We Find Them?

So we need a design vocabulary, a set of tools underlying game design practice. There is no correct or official method to identify them. One easy way to start looking is to take a good game and describe concretely some of the things that work well. Then, from concrete examples of real game elements, we can attempt to abstract and formalize a few key aspects and maybe find ourselves a few tools.

There isn't enough space here to exhaustively analyze each tool or game — the goal here is to give an overview of the ideas behind and uses of FADT, not a complete view of everything. With that in mind, we'll start with a quick tour of some games, tools, and ideas. Since we are looking for examples of good game design, we'll start by examining *Mario 64*. Once we have explored some concrete aspects of the game itself, we'll step back and start looking for things to abstract and formalize that we can apply to other genres and titles.

From: http://www.gamasutra.com/view/feature/131764/formal_abstract_design_tools.php
