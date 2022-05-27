---
layout: page
title: Reefbane
description: A page dedicated to this glowy unique Fishing Rod - Reefbane- and what it can tell us about zones it glows in
permalink: /fishing-items/reefbane/
image: /assets/img/reefbane.png
---

![Reefbane Unique Fishing Rod](/assets/img/reefbane.png "Reefbane Unique Fishing Rod")

# Overview

Reefbane is a unique fishing rod that has a special affix: *_Glows while in an Area containing a Unique Fish_*. Most of the research around Reefbane is around determing what this glowy fishing rod can tell us.
  
# Dropping a Reefbane
  
Our current operating assumption is that Reefbane does not have any special drop requirements, and is merely mirror-tier rarity. (In fact, if Reefbane is not somehow drop-restricted, it might be the rarest unique item in the game.)
    
Per the [Inscribed Ultimatum Unique Item Tier List](https://docs.google.com/spreadsheets/d/11sO9YrtGGFJ-g51hiA5kLpQ5rQ1syP4QJehZL2P1ibs/edit#gid=0), Reefbane is a T0 Unique -- the rarest category.

- **Sources of drops**: We've seen examples of natural Reefbane drops from regular white chests, Lab chests, rare mobs, unique mobs, and more. (There are also deterministic ways to obtain Reefbane, e.g. via Reliquary Keys, cards, using an Ancient Orb on SOTS, buying from an old Forsaken Master for 1 mir, etc. -- but we're interested here in natural drops.)

- **Areas / locations**: We have hard proof of natural Reefbane drops occurring in the following Areas: {Waste Pool, Shipyard, Bazaar, Lab, Bog}. The following locations are also Trustworthy / High-Likelihood, but we do not have hard proof for them: {Tunnel (aka Crystal Ore), Bazaar, Arid Lake, Promenade, Arena}. There are many other casually reported drop locations as well. In short, specific areas (or area tags) do not seem to matter.

- A Song of the Sirens can be Ancient Orb'd into a Reefbane in any Area, which implies that Reefbane does not have a special League- or Area-based drop restriction. But one cannot use an Ancient Orb to transform a Reefbane into a Song of the Sirens. This is a one-way recipe that can destroy SOTSes while generating Reefbanes.

- We know for certain that Fairgraves' Tricorne is not required for Reefbane to drop. This is a pretty well-known exception in the broader community, too.
  
- We've only really seen multiple Reefbanes drop consistently for characters running minmax'd legacy magic find on Standard with Harvest-horizon'd anointed maps using perfect maximum juicing. This is another testament to its extreme scarcity.
  
# Reefbane's Glow

After long investigation, it was found that Reefbane's Glow can only trigger in Areas that have the area_with_water tag.
  
 > What where the steps to figure this out?
 
If you spam enough new instances of a zone, Reefbane eventually glows. Sometimes this requires hundreds of attempts; the probability of occurrence is low (rough estiamtion of ~1%).

**However, few zones were found were Reefbane never glowed:**
- Act 9 The Quarry (n > 2000)
- Act 9 The Tunnel (n > 2000)
- Act 9 The Crystal Veins (n ~ 600)
- Act 4 The Mines 1 & 2 (n = {400, 800})

The sample sizes n listed above were the number instance creation attempts by our experimenters. All of these values are pretty substantial. With the assumed probability of 1% for a Reefbane proc, failing to see a proc after 600 trials in a zone that can proc has probability ~0.24% - exceedingly unlikely.

**The next obvious research question was: Why does Reefbane seemingly fail to glow here? What is special about these zones versus others?**

Here are a few statements that was noticed during the testing:

- Reefbane can glow in instances containing Masters, e.g. Niko. (We'd wondered if there might be a conflict with Masters spawning and consuming "space" needed by whatever effect Reefbane detects.)
- Reefbane can glow in instances which contain league events such as Essences, Abyss, Strongboxes, etc. (Ditto.)

**We selected these zones for testing (Quarry, Mines, etc.) because of a clue left in the Reefbane Reveal video.**

ItsYoji's Reefbane Reveal video used substantial GGG footage. One scene compares Reefbane's "Glowing" and "Not Glowing" states.

We realized that this scene may be a hint instead of just a demonstration: the area selected for the "Not Glowing" state may have been an intentional clue. Thus, we began testing zones with tilesets similar to the one shown.

In retrospect the hint seems pretty obvious! [There is an all-caps "NO GLOW" message, after all.](https://i.imgur.com/KB0inVF.png)

For other examples of how crucial hints are in GGG media, [check out the discussion on Reddit.](https://www.reddit.com/r/pathofexile/comments/f0cyfr/serious_anglers_mate_1_wraeclasts_best_and_only/fgsvggj/)

# Does Reefbane _detect_ or _cause_ a glow in an instance?
  
  This question was asked in the Fishcord:

> Is the glow from Reefbane _caused_ by creating an instance with Reefbane equipped/held, or does Reefbane _detect_ an inherent property of certain instances?
  
  The answer is the latter: **Reefbane detects a hidden property in certain zone instances, including instances which are created without Reefbane involved.** Contrast this statement with instances which inherit character data; for example, when a player creates an endgame map, the game checks character data to determine mods for that endgame map instance (it pulls from the character's sextant data, their atlas status/bonus, etc.).

The reason this is important: a special attribute of certain instances exists independent of Reefbane. Reefbane is a detection tool. Reefbane itself does not _cause_ an instance to be "glowy". The glow procs only in instances which already have a preexisting special attribute.
  
### How this was tested
  
There were two main ways to test this which occurred to us: (1) party up and have one player create instances, which are then joined by a second player who has Reefbane equipped; (2) drop Reefbane outside of a zone, create a new instance without Reefbane, and then retrieve Reefbane and reenter to see if it procs. We picked the latter method just to have a bigger sample.

We had two players testing independently; following cryptographic tradition, we'll call the players Alice and Bob.

Procedure used:
- Unequip all gear items and jewels except for Reefbane.
- Enter A1 The Coast.
- Drop Reefbane.
- With zero items equipped, create a new instance of A1 Mud Flats.
- Return to A1 The Coast.
- Pick up Reefbane.
- Re-enter the existing instance you created of A1 Mud Flats, this time with Reefbane equipped.
- Check and see if Reefbane glows.
- Repeat from Step 2.

**Trials**: n > 250 for Bob; n = {149, 2, 45} for Alice. In all cases Reefbane was observed to glow in instances that were created without Reefbane (or any other items) equipped. These trials took a long time.

**Miscellany**: Bob tested using a fresh low level character; Alice tested using a high-level character who had completed all storyline + optional quests + maps; Alice tested the first trial batch while wearing other fishing gear. None of these miscellany seemed to have any effect on results.

**An additional interesting note**: In the last trial, both Bob and Alice each created an instance which proc'd Reefbane's glow within the exact same real-world minute, possibly near-simultaneously. This is very low likelihood. This may imply real-world clocktime matters for Reefbane. (Or it could just be a very unusual coincidence, of course.)
 
 
 

# Other Neat Reefbane Facts
- If Reefbane glows in an instance, each party member holding a Reefbane will exhibit their own glow.
- Did you know that if you equip Reefbane onto an Animated Guardian in a zone in which Reefbane glows, [the AG's Reefbane glows too?](https://i.imgur.com/EQk7Oqr.png)
- The same holds true for casting Animate Weapon on a Reefbane in a "Glow" zone: the animated Reefbane will glow as well. Though you'd have to sacrifice a Reefbane to see it for yourself -- Unthinkable!

# References
- [Reddit - Angler's Mate #1](https://www.reddit.com/r/pathofexile/comments/f0cyfr/serious_anglers_mate_1_wraeclasts_best_and_only/fgsvfl4/)
- [Reddit - Valuable Fishing Questions and Reefbane Discovery](https://www.reddit.com/r/pathofexile/comments/eurdi7/serious_valuable_fishing_questions_plus_a_small/)
- [Reddit - Valuable Fishing Questions and Reefbane Discovery Comment](https://www.reddit.com/r/pathofexile/comments/eurdi7/serious_valuable_fishing_questions_plus_a_small/ffr0sds/)