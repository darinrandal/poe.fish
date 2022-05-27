---
layout: page
title: Angler's Plait FAQ and Discussion
description: Detailed log of the process of determining how to find Angler's Plait by u/poorFishwife
permalink: /fishing-items/anglers-plait-faq-discussion/
image: /assets/img/anglers-plait.png
---

# How in damnation did you figure this out?

The hard way.

When I first made this secret my business, I extensively researched all past evidence of Plait drops. (I'm oversimplifying a huge effort here!) Then I spoke to every Plait owner. I set up a livesearch for new Plaits. I spoke to dozens of people about their experiences. Many cases were dead-ends, e.g. people who merely bought the ring and didn't remember the seller. But sometimes I was able to trace the item back to the person who originally found it and sold it. Sadly, oftentimes the originator was an innocent newbie who was scammed out of their drop.

Eventually I built up info on "Trustworthy Plait Drops" -- situations where I was timely enough to gather character data, or where a person was trustworthy and forthright. Over time I collected a few just-in-time snapshots of characters. That allowed me to start checking correlations.

No one I spoke to had any clue how they'd found the ring. All original finders discovered it accidentally. Usually I was the one informing them, e.g. I'd say "It has something to do with Slitherpinch, but I don't know all the factors yet."

I was highly confident that just Slitherpinch was insufficient due to extensive trials done by others who had been suspicious about that item. (For those that do not know, Slitherpinch is a [confirmed fishing item](/fishing-items#slitherpinch-bronzescale-gauntlets).)

Once I felt my research was sufficient, I started testing.

There were false starts. The craziest correlation coincidence was a statistical improbability around mod rolls on Slitherpinch. I'd noticed all Slitherpinches had even numbers on their mod rolls. (Ex: 46 Dex, 8% APS, 82% Eva.) On a single item that's not noteworthy -- but all of them were like that. I'd never heard of mod roll values being important before, but at that point I couldn't rule out anything. The probability of that observation was insanely low; thankfully, eventually some counterexamples finally appeared.

After a couple of my own finds, I began attempting to isolate factors. Some factors are extremely difficult to "disprove" with an item this rare, but I was still able to add evidence and update my overall confidence. (Naturally, some factors I've listed will be unlucky coincidences, just like "Even Numbers on Slitherpinch" was. That's how judgment under uncertainty works!)

I also did a ton of negative testing, seeking counterexamples. Example: I grinded with setups designed to minimize Fleeing/Invasion/Ambush occurrences. In those setups I never found a Plait. Once again, this doesn't remotely prove anything, but I had to try. I won't be surprised when someone eventually produces a counterexample for one or more factors.

Along the way I noticed a couple other people who seemed to be trying for Plaits. As I spied on their progress, they seemed to have poor results. One person finished multiple level 100 characters. Comparatively my playtime is low (I spend all my time on secrets, hah!); and yet here I had multiple Plaits.

After realizing that I might be the most successful "Plait farmer", I knew I'd need to share what I'd learned. I can't be confident about everything here, but I feel this is a sufficient guide that makes it a reasonable target.

# I found an Angler's Plait!! What should I do?

Please make a post with full details and screenshots, or ideally a video. Include as much information as you can. Key information to include along with screenshots: (1) your full character details, as a POB export snapshot; (2) the map mods on the area; (3) a corpse-targetted shot of the mob which dropped it; (4) a walkthrough of the area to observe what hidden zone modifiers might exist, such as Strongboxes; (5) anything else you can think of.

Your observation might help us further discriminate which factors matter and which are superfluous. Please take the time to document and post if you find one!

# Chance to Flee, though? Really? Wtf?

However unusual, the pattern exists. It is very possible this is a mislead, but we'd need good evidence to rule it out (e.g. a video of a Plait from a mob under conditions where it is impossible for the mob to be affected by Fleeing or engaging its Flee AI script behaviour).

To avoid potentially wasting a ton of your time, if you are farming Angler's Plait, make sure you have a way to inflict Fleeing.

In the Factors section I mentioned 100% of all "Trustworthy Plait Drops" have come from situations where the character had a means of applying the Fleeing condition on the mob which dropped the item. This includes all of my personal finds as well.

Even a Hallowed Ground (the bugged version of Angler's Plait that erroneously appeared in-game before Plait was released) was discovered by a player wearing Blackheart. Blackheart has the unusual mod '10% chance to Cause Monsters to Flee'.

Other items Plait-finders have claimed to use include Voidheart, Blackheart, Wake of Destruction, and Lion's Roar. My own successful setups all used a 21/23 Chance to Flee gem.

One person used minions and had no player chance to ignite (RT). I hoped this would finally be a counterexample. But their build emphasized minion crit. They had a single jewel with "Minions deal 8 to 10 additional Fire Damage". As most players know, critting with any amount of Fire Damage can Ignite. As most players do not know, some mobs naturally Flee when Burning. This includes all Human-types, monkey-types, Sea Witches, and others. Thus the build had a clear way to cause Flee, and I couldn't use it as a counterexample.

Many mobs also have an AI Script action to Flee regardless of player gear. Here's an example from Bloodstained Archer: [Flee 9 OnlyLastTarget TargetNear NoRepeat TargetIsEnemy]. So to be sure that Flee is unrelated to Plaits, we'd need to see a video of the specific mob that drops the item.

I sense a clever expert out there shouting at their screen: "But rare mobs don't Flee!" The stat governing this on Rare mobs is "Monster does not flee.", which is actually "Monster has a 100% chance not to flee". The stat dictates which behaviour the mob will take, not necessarily its condition. (Contrast to Unaffected vs Immune; e.g. if you are Immune to Poison you cannot have the Poisoned condition.) Of course, rare mobs can also Flee on their own accord regardless of the player, if the mob has "Flee" in its AI Script.

It's hard to prove that Flee doesn't matter.

Fleeing is also connected to fishing. Here's an incomplete list of examples.
- The most overt connection is the Albino Rhoa. The Albino Rhoa never attacks; it always flees. Specifically, its behaviour is permanently set to "Flee" with the condition "TargetIsEnemy". For a long time in POE's history this behaviour was unseen on any other mob. And, of course, the Albino Rhoa Feather has multiple connections to fishing.
- In the ItsYoji Reefbane Reveal video (which includes footage supplied by GGG and has other known hints), ItsYoji's Templar character appears in one scene [wearing Wake of Destruction](https://youtu.be/TGIF6MfC7E0?t=57). This could be a coincidence, an artifact of ItsYoji's own decisions -- or it may be an intentional hint.
- This is a stretch, but: Wordplay between Flee/Catch might be relevant. Consider the famous Darkshrine "Player Muted" outcome: "The fishing was good; it was the catching that was bad". It's fair to say a player must "Catch" a fleeing Albino Rhoa.
- Legacy fishing rods could roll a corruption implicit of 'n% chance to Cause Monsters to Flee', although this was not unique to rod basetype items.

GGG wrote recent patch notes on Fleeing, despite the condition being so unused. (Perhaps this just stems from a low-risk bugfix given to a new developer or something, though.)

> "Fixed a bug where monsters that were Fleeing would do so for a much shorter distance than intended." ([3.8.1.D](http://s3.pathofexile.com/forum/view-thread/2655286/page/1))

All this could be a series of unusual coincidences connecting Fleeing to Plaits. It might be a complete mislead and utterly superfluous. But for now, better safe than sorry: make sure you have a way to cause Fleeing.

# In the Factors section, you said that X was not required. But even if it's not required, what if it has an impact?

This is possible, but extraordinarily difficult to determine.

Maybe wearing other fishing items increases (or decreases!) Plait droprate. Maybe IIR and IIQ actually have a negative impact. Maybe fishing stats like IFQ, IRQ, or Fish Bite Sensitivity matter.

But to be confident of any of those wild guesses, we'd need a rigorous controlled experiment where each condition's testers drop multiple Plaits. Rough!

# Is this all a big joke? I want more proof!

Astute record-keepers will notice the exact Plaits I've shown have never appeared on /trade. I'm happy to link them in-game to anyone who asks.

Ideally I'd show you a video of a Plait dropping. Unfortunately, I do not stream. Fortunately, I am sure that by reading this post, certain streamers (_cough slipperyjim8_) will produce a video of them finding a Plait. Then, your reasonable desire for hard video evidence will be sated. Sorry that you'll have to wait; as they say, [fishing requires patience](https://twitter.com/pathofexile/status/1228956010854772736).

I hope in the meantime that the extensive matter-of-fact information I've provided sufficiently shows that I am completely serious. This is not a troll; as Krillson says, "Red Herrings annoy me."

# Why the heck are you giving away such a valuable secret?

Many reasons. But mostly: revealing this information will make a lot of people very happy.

I hope this makes you happy too.