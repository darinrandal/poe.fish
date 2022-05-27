---
layout: page
title: Scourge Fishing Modifiers & Water Fishing
description: 3.16 Scourge league added brand new fishing modifiers. One of these interesting mods is "Cannot Fish while standing in Water"
permalink: /scourge-modifiers-fishing/
---

# Scourge Fishing Modifiers
## Scourge modifiers
3.16 Scourge league brought in a number of new fishing modifiers that can be scourged onto items. The following is a list of all fishing modifiers introduced in 3.16:

##### Upsides
-    (10–30)% increased Size of Fish caught during Daytime
-    (13–16)% increased Fishing Range
-    (20–25)% increased Rarity of Fish Caught
-    You can catch Scourged Fish

##### Downsides
-    (30–40)% reduced Fishing Line Strength
-    (50–100)% increased Fishing Pool Consumption
-    Fish Rot upon being Caught
-    (30–60)% reduced Reeling Stability
-    Cannot Fish while standing in Water


> „You can catch Scourged Fish“ modifier was not obtained by playerbase and, thus, has been lost.

These new modifiers provide an additional insight about Fish in Path of Exile:

- Fish can Rot
- Fish can be Scourged
- Fish can be Caught during Daytime
- Fish can have variable Size
- Fish are associated with a Reeling Speed stat
- Fish are associated with a Reeling Stability stat
- Players can Fish while standing in Water
- Cannot Fish while standing in Water

The other Scourged mods not implied from this list merely reused existing "Fishing mechanics", so they weren't new. For example, there's a Scourge mod that affects Fishing Pool Consumption -- but that "mechanic" already existed from the Calming prefix found on regular basetype Fishing Rods.

It is interesting to note **Fish** is capitalized in these modifiers and very well might be the first time a mechanical term for the action of fishing has been capitalized. The term "Fish" is a keyword object that describes entities. But in this Scourged Downside mod, the term "Fish" is a *player* verb, likewise capitalized like other game mechanics are.

(To clarify, compare to e.g. *Cannot Block* or *Cannot Knock Enemies Back*. "Block" and "Knock Enemies Back" are player verbs, and appropriately capitalized.)

## Water and Dry Fishing

Imagine for the sake of argument that the wording "Cannot Fish while standing in Water" was very carefully intended, and not an accident.

1. Consider two Fishing Rods, WetRod and DryRod. Assume they are identical except DryRod has the modifier "Cannot Fish while standing in Water" and WetRod does not.

2. Assume a player knows that they qualify as "standing in Water" (whatever that means). For example, assume that positioning one's character inside the bounding box of a water asset qualifies as "standing in Water", and it's not something more insidious.

3. Now the player can switch between rods to test actions to see if they qualify as the act of Fishing.
4. For example, does using Default Attack to swing a Fishing Rod count as an attempt to Fish? If so, then it should be possible to Default Attack while wielding WetRod, but it should not be possible to Default Attack while wielding DryRod.

Exhaustively testing eligible player actions with WetRod and DryRod and observing no restrictions would allow the player to blacklist-eliminate specific actions, verifying them as Not Fishing.

However, since the Scourge mod is a negative constraint, it cannot be used to whitelist-verify an unknown action as Fishing. The action must be known.

For example, imagine that Fishing is "Perform a sacred rain dance, then Default Attack". If the player does not know the sacred rain dance, they cannot test this action.

At minimum this does give a tool to rule out hypotheses. 

If someone speculates that e.g. "Killing a Writhing Worm with a Fishing Rod and then Default Attacking counts as Fishing", they could test that hypothesis and see if some steps are unexpectedly impossible when wielding DryRod and standing in Water.

All of the above is predicated on GGG very carefully and intentionally selecting the wording of "Cannot Fish while standing in Water".

So, was it written with intent and care? Yes, it was.

> Mark_GGG
> This is intentional - "Fish" can be both a noun and a verb, differentiated by context, similar to "Attack". Preventing Fishing is distinct from preventing Catching.

Mark's verification means that the mod text was indeed carefully considered. So if the act of fishing is in fact possible in-game, it's reasonable to assume that "Cannot Fish while standing in Water" truly is a means of testing hypotheses about what constitutes "fishing".

For any intrepid experimenters working on shot-in-the-dark testing, if you haven't already played around with this mod, consider trying it!

{.is-info}
