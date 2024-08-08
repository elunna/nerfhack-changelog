# NerfHack Feature Set

This changelog exists to track the changes in NerfHack: https://github.com/elunna/NerfHack.

## Big changes from NetHack 3.6/3.7

* Removed the **mysterious force** from the game (xnh).
* To bring back the feeling of the 3.4.3 **stealth** mechanic, the chance of sleeping monsters waking up and growling has been lowered dramatically and is based on luck.
  * 0 Luck: 12.5% chance of a monster screaming when roused.
  * 2+ Luck: 0.3% chance
  * Negative luck has at least a 30% chance of rousing monsters.
* Reverted the majority of **level flips** from 3.7. Flipped levels only appear in Sokoban and the big room special level.
* **Items that are 'lost'** from the players inventory will no longer be un-identified. 
* **Stinking clouds** no longer block line of sight
* **Disabled vampire shapeshifting** for all vampires except Vlad; this includes vampshifting or the player polymorphed into a vampire as well.
* **Branchport** always brings you to the entry level of a branch
* **Partially revert 5c7c9d10a** - Rejigger anti-magic traps. I thought the severity of the
  original change was actually fine, anti-magic traps were historically a joke in NetHack
  3.4.3 so this makes them somewhat threatening.
* Items that grant **steadfastness** will do so even if the hero is flying or levitating.
* **Reverted 82f0b1e8e** - Scared hostile monster which cannot move away will attack. Players will be able to stand on scrolls of scare monster or Elbereth without risk of random melee attacks from scared or fleeing monsters.

## QUALITY OF LIFE FEATURES

* Removed the quest turn limit (Un)
* Players can enter the quest as soon as they reach level XL 10 (Un)
* Crysknives are never auto-quivered
* Chaotics do not get alignment penalties for casting healing at pets (xnh)
* Chaotics do not get alignment penalties for angering peacefuls (xnh)
* When you polymorph into a 'nolimbs' monster, you are able to slip out of a ball & chain (Evil)
* Phasing allows escape from being engulfed (Evil)
* Restrict pets from blowing you up via gas spore, so they won't attack one while you are adjacent (xnh)
* Don't livelog events in explore mode
* Swapping weapons take 0 turns (dnh)
* Running and traveling no longer pushes boulders (xnh)
* When traveling, grave engravings will not be stopped on or considered 'interesting'
* Random secret doors are secret less of the time (xnh)
* Random secret corridors have been removed (xnh)
* Pets never displace player from stairs when entering a level (Dyna).
* Lessen confusing messages for confuse monster effects wearing off.
* Because see invisible cannot be gained intrinsically - peaceful monsters will not make themselves invisible by means of potions, wands, or spells.
* Passive fire damage burns away slime.
* Allow #terrain while impaired (xnh)

### Safer bags of holding:
In the NetHack community, the blowing up of Bags of Holding seems to be an honored tradition that is upheld and broadcast on the servers when it occurs. However, I find it a severe punishment that kills games for both the player and the devs. Most of the time when a player has this happen, they simply quit. Since I would rather keep players going, I believe the right approach is to punish players who make these kinds of mistakes willingly and earlier in the game. Once a player has identified the dangerous items for a bag of holding, it is virtually implausible that one would purposefully attempt to blow up their bag of holding.

The following safeguards were added to protect players from exploding bags:
* Players cannot put **known** wands of cancellation or magical bags into **identified** bags of holding. Keep in mind, unknown wands and bags are still dangerous and should be handled with care until formally identified (dnh)
* Players are prevented from tipping **known** explosive items into **identified** bags of holding
* Empty wands of cancellation may still be placed inside bags of holding (no risk of blowing up)

### STREAMLINED IDENTIFICATION FEATURES

A general design philosophy of NerfHack is to automatically identify items that are unambiguous from various effects. If a quick wiki lookup is all that is needed (ie: sink ring identification) let's save the player from opening up a browser.

* All roles start out knowing potions of water, blank scrolls, and scrolls of identify
* When dropping a container on an altar, the BUC status of all contained items is revealed (NetHack4)
* Your primary wielded weapon is auto-identified after killing enough monsters with it (Evil)
* Auto-ID potions of acid when water explosions result from dipping (xnh)
* Auto-ID potions of acid when a lichen corpse is dipped into one
* Auto-ID potions of sickness when they coat a weapon in poison
* Auto-ID potions of sickness and fruit juice when dipping unihorn in sickness
* Auto-ID potions of restore ability when quaffed
* Auto-ID amethyst, fruit juice, and booze when dipping amethyst into booze (Fourk)
* Auto-ID some potions when inhaling their vapors (xnh)
* Auto-ID scroll of scare monster if it crumbles from picking up (Un)
* Auto-ID scrolls of confuse monster when read
* Auto-ID scrolls of enchant armor when they erodeproof or make dragon scale mail
* Auto-ID scrolls of food detection if they have an obvious effect.
* Auto-ID enchant armor when it erodeproofs or hardens dragon scales.
* Auto-ID rings dropped into a sink (Un)
* Auto-ID ring of regeneration if it heals you (Un)
* Auto-ID wand of cancellation after destroying a bag of holding (Un)
* Auto-ID wands when engraving (xnh)
* Automatically use a process of elimination for auto-identifying wands when available (Un)
* Auto-ID loadstones when attempting to drop or stash them (Un)
* Auto-id flint yielded from applying rocks to eachother
* Auto-ID tin whistles, tooled horns, magic flutes, and magic harps upon use (Un)
* Auto-ID magic lamps and oil lamps when rubbing (Un)
* Auto-ID dunce cap when it's first put on (Un)
* Auto-ID jumping boots upon wearing (Un/Ace)
* Auto-ID water walking boots when they waterwalk (xnh)
* Auto-ID kicking boots when they are kicked
* Auto-ID BUC of products from BUC identified tinning kit or horn of plenty (UnNetHack++)
* Auto-ID BUC of wands when they backfire
* Blessed stethoscopes can identify eggs (Evil/Spork)
* Make rustproof/erodeproof/fixed known by default (Dyna)

### INTERFACE CHANGES 

* Detailed object and monster is available in the in-game lookup (Pokedex), ported from xNetHack with updates from HackEM.
* Peaceful monsters are underlined (TTY and curses) (xnh)
* Magic cancellation (MC) value is shown on the bottom line (Evil)
* Skill caps and percentage towards next level is available in #enhance
* Show available skill slots in #enhance menu (Dyna)
* Add inventory weight/carrycap and n/52 items display
* /> or < can be used to autotravel to stairs (autostairtravel option)
* Display AC values for armor in the hero's inventory (Splice)
* Pets' items can be managed with #loot
* Prayer statistics (like when you last prayed, reconciled with your god, or received a gift) can be viewed in the attributes menu (via Ctrl-X)
* All position prompts may be aborted
* Show warning level 0 for very weak monsters (Dyna).
* We are able to see when a monster is sleeping, fleeing, withering, or berserking from farlook information (Evil/Splice/xnh)
* We can see if our pets are confused, stunned, or blinded.
* We are able to see what weapon a monster is wielding from farlook (Evil)
* We are able to see roughly how much armor a monster is wearing on farlook (Evil)
* More descriptive combat messages have been added to enhance hits and misses (xnh)
* The SLASH'EM style message is used for getting zapped by cancellation
* Show messages for objects that are randomly cursed (Dyna).
* Print an explicit message when summon nasties occurs as part of wizard harassment.
* Special room and special level walls can have their own unique coloring. For example, cockatrice nests and bee hives are yellow, and Sokoban walls are blue. (Splice/xnh)
* The first 2 levels can have a helpful engraving in the room with the upstair. This hint system was imported from UnNetHack and gives the player direct tips for survival and using the new mechanics.
* Disabled **#chronicle** from auto-completing (so #chat will autocomplete as normal)
* Enabled autocomplete for #twoweapon
* Disabled **farlook help**
* Disabled the 3.7 **tutorial**
* Enable **full options** by default.
* Changed the symbol for **sinks** back to #
* The hero's color reflects their race (SLASH'EM)

### New config options
* **showdamage:** Displays damage and flanking bonuses/penalties
* **noflipsoko:** Enables player to choose whether they want Sokoban levels to be flipped. If enabled, incurs Sokobon penalty for use.
* **invweight:** Show weights of objects in inventory (invweight option)

### WIZMODE FEATURES

* The #wizcrown command has been added for testing crowning (Evil)
* The #wizclear (^z) command, clears all monsters on the screen (Splice)
* Wizard mode can override an artifact ignoring you (xnh)
* Allow teleportation into unteleportable spots in wizard mode
* Allow wishing (^W) for monsters in wizmode (Un)

## RESOURCE CONTROL(NERFS) AND MECHANIC CHANGES

* Magic resistance and spell damage reduction only halve magic missile damage instead of preventing it (Evil)
* The chance of gaining levels from wraiths has been reduced using the SLASH'EM version of edible wraith corpses.
* Bones file trimming. When bones files are left, there's a high chance of items being polymorphed or shuddering away. This nerfs the common strategy of dumplog peeking.

* Strength gain nerfs: giant corpses have less of a chance of conferring strength gain (from 50% to 25%) (SLASHEM)
* HP gains from healing potions are subject to nurse dancing limits, but the limit is always observed as if the players level is maxed out at 30.
* Falling downstairs does more damage - 2d3 instead of 1d3. (K-Mod)
* Falling down a hole or pit while fumbling (or very low dex) can make you fall on a wielded weapon.
* Going downstairs while stunned always results in falling, confusion sometimes does.
* Don't allow stunned jumping. Confused jumping has a 20% chance to fail (Evil)

### Slow Luck timeouts (modified)

In NerfHack, Luck items greatly slow down Luck timeout rather than stopping it completely - this is similar to how it works in UnNetHack. However, the timeouts have been modified and extended to cover negative base luck situations. The timeouts have also been reduced heavily from the UnNetHack calculations.

The modified Luck timeout depends on how far your Luck is from your base Luck: the higher or lower your Luck, the less the timeout is slowed. The timeout is calculated every turn, meaning gaining or losing a point of Luck could result in that point timing out immediately.

The modified Luck timeout is calculated by the following formula:

    Timeout = 25 * (20 - base_distance) * (20 - base_distance)

base_distance is how far you are from your base luck. If your base luck is 0 and you have 3 Luck, the base_distance is 3. If you have -10 base luck and 10 Luck, the base_distance is 20. The following chart shows how many turns it takes to timeout from one luck level to the next and the total turns to reach the base distance of 0.

| base distance | Timeout | Time to base Luck |
| ------------- | ------- | ----------------- |
| 0             | ∞       | 0                 |
| 1             | 9 025   | 9 025             |
| 2             | 8 100   | 17 125            |
| 3             | 7 225   | 24 350            |
| 4             | 6 400   | 30 750            |
| 5             | 5 625   | 36 375            |
| 6             | 4 900   | 41 275            |
| 7             | 4 225   | 45 500            |
| 8             | 3 600   | 49 100            |
| 9             | 3 025   | 52 125            |
| 10            | 2 500   | 54 625            |
| 11            | 2 025   | 56 650            |
| 12            | 1 600   | 58 250            |
| 13            | 1 225   | 59 475            |
| 14            | 900     | 60 375            |
| 15            | 625     | 61 000            |
| 16            | 400     | 61 400            |
| 17            | 225     | 61 625            |
| 18            | 100     | 61 725            |
| 19            | 25      | 61 750            |
| 20            | 0       | 61 750            |

### ENDGAME CHANGES

* Occasional earthquakes can occur during the ascension run (Un/Evil). These will cease after entering the planes.
* The identity of the Riders hidden via farlook (Un)
* The correct temple on the Astral Plane will not be revealed due to fleeing monsters (Un)
* **"Purple/Astral Rain" nerf:** Taming is much more difficult on the Astral Plane; attempts to tame monsters only have a 1 in 5 chance of succeeding.
* Replaced undead on Astral Plane with random A (xnh).
* Wizard harassment (after initially killing the Wizard of Yendor) has been increased by 20-25%
* While the player is carrying the Amulet of Yendor, monsters flood from the upstairs (Un/Evil). After entering the planes, this extra monster generation will subside.
* Demon lords and princes can be summoned (as part of the Wizard's harassment) when you possess the Amulet of Yendor. After entering the Astral Plane, this threat will cease.
* Level-teleporting in hell (or wiz/vlad's towers) causes major pain. The levelport will still succeed as normal, but costs a large fraction of the hero's HP and energy.

### FINITE ALTAR NERFS

* When donating to priests - the gold vanishes upon receipt
* Protection that can be bought from priests or granted by your god only ever grants 1AC per granting; the more protection the player has, the less likely it is to be granted (K-Mod)
* Greater chance of hostile minions appearing when converting an altar. Especially if the altar is in an occupied temple (Evil)
* Removed the "temple of the gods" theme room. This themed room contains 3 altars, one of each alignment. It was removed to make the finite altars mechanic more relevant.
* Intrinsics speed, stealth, and telepathy are no longer granted by the gods when #offering.

#### Altar cracking

- **Once the player has received two gifts or has been crowned, altars have a 50% chance to crack with each subsequent gift.**
* There are two stages to the cracking. In the first stage the altar becomes partially cracked, which is purely cosmetic and doesn't affect the altar's functionality. This cracked status can be seen on an altar by farlooking. However, receiving another gift from a cracked altar will certainly destroy it, losing it forever.
* Being crowned also counts as a gift. If you are crowned on a cracked altar, it will also almost always destroy it in the process (however - there is a 1 in 13 chance that the altar will survive the process).
* Altars on the Astral Plane will never be destroyed. Note that they can still become cracked but are safe from destruction.
* Altars also sometimes generate cracked. 1 in 4 altars will generate pre-cracked (doesn't apply for temples or pre-mapped altars).
* Altars are always cracked after level 15.
* Converting an altar will also frequently crack it. This occurs 1 in 13 times the altar is converted or 1/3rd of the time hostile minions are summoned.

The original altar nerf came from SpliceHack, where altars had a 50% chance of being destroyed after 2 artifact gifts had been bestowed.

A new conduct was added to the #conduct menu so that players can track how many altars have been destroyed in their current game. Altar cracking is livelogged on game servers for the entertainment value.

#### #offer GIFT ODDS

* The odds have been adjusted in favor of the player, especially after 2 gifts have been granted.

| Gifts Granted | Old odds | New odds |
| ------------- | -------- | -------- |
| 0             | 10.00%   | 12.50%   |
| 1             | 8.33%    | 10.00%   |
| 2             | 5.56%    | 8.33%    |
| 3             | 3.57%    | 7.14%    |
| 4             | 2.38%    | 6.25%    |
| 5             | 1.67%    | 5.56%    |
| 6             | 1.22%    | 5.00%    |
| 7             | 0.93%    | 4.55%    |
| 8             | 0.72%    | 4.17%    |
| 9             | 0.58%    | 3.85%    |
| 10            | 0.48%    | 3.57%    |

However, altar gift frequency is also tempered by your experience level (EvilHack).

As your level increases, the probability of receiving an artifact increases. Under level 4 is not possible:
* level  4: 10% chance
* level  9: 20% chance
* level 12: 30% chance
* level 14: 40% chance
* level 17: 50% chance
* level 19: 60% chance
* level 21: 70% chance
* level 23: 80% chance
* level 24: 90% chance
* level 26 or greater: 100% chance

This rewards leveling up and slows down the power grab that some characters might go for with a guaranteed sacrifice gift (ie: Barbarians). It also slows down the rate at which altars are cracking and getting destroyed, giving more time to utilize them for other things like building Luck or getting crowned.

* The number of artiwishes is not factored in when determining the chance of a gift. The revised gift probabilities still apply, just filtered through the level check.

### PET THEFT

* Pet theft from shops has been totally nerfed.
* Pets will never pick up objects in shops (Gnoll)
* You also cannot #loot items to/from your pet that are unpaid.
* Artifact costs have been reduced to 1/5th of their previous cost. Since they can't be stolen via pet theft, they have been adjusted to make them affordable.
* Shopkeepers start with more gold, usually more than double the standard amounts (gnoll)
   
### WISHING

* Quest artifacts cannot be wished for (dnh)
* Attempting to wish for quest artifacts doesn't use up a wish
* Wishes no longer increase prayer timeout (Dyna)
* Wishes from thrones are much more rare. The chance of getting a wish from sitting on a throne is now about 1.5%. If the player doesn't get a wish, they lose 1 point of Luck. Once the player is granted a wish from a throne, the throne is guaranteed to disappear. (Evil with adjustments)
* The chance of getting a djinn from a smoky potion has been halved. The actual chances of getting a wish from the djinn have not been changed.
* Players have a chance of getting a wish from crowning now (if no intrinsics were granted).
* Artiwishes only care about previous **successful** artiwishes.

**The chance of receiving the artifact from a wish is:**

    1 in [number of previous artifact wishes + 1]. 

  * Artifact wish #1: 1 in 1 chance of success (100%)
  * Artifact wish #2: 1 in 2 chance of success (50%)
  * Artifact wish #3: 1 in 3 chance of success (33%)
  * And so on.

### POLYMORPHING OBJECTS

* The number of items you have polymorphed can be viewed in #conduct
* Non-magical potions, scrolls, spellbooks, and wands are much less likely to transform into magical items. These items only have a 1% chance of transforming into something magical. This is now comparable to other non-magical items polymorphing into magical. (dnh)
* The chances of getting a golem from polypiling have been increased (K-Mod)
* The enchantment level or charges can be randomly reduced on polymorphed objects (Spork)
* Amulets of unchanging can't be polymorphed (Un)

### CROWNING

* Crowning requires 13 Luck (from dnh). 
* Crowning only grants *up to* 3 intrinsics. In Vanilla, crowning would grant fire, cold, poison, sleep, and shock resistance, as well as see invisible.
* Intrinsic see invisible is no longer granted via crowning
* Intrinsic telepathy is no longer granted via crowning
* In NerfHack, the game will roll 3 times to pick random intrinsics. On each roll, if the player already possesses that intrinsic, the roll is lost - otherwise the player gains it permanently. If a player fails to gain any new intrinsics, they instead are granted a wish.
* Crowning gifts are only granted when crowned, never for #offer.

New intrinsics available when crowned:
* Acid resistance (this is the only way to receive this resistance intrinsically)
* Disintegration resistance
* Petrification resistance (exclusive to crowning)
* Sickness resistance (exclusive to crowning)


### Leveling up bonuses

Players get a to-hit bonus after reaching level 20 (from EvilHack with adjustments)
    * Level 22: +1 to-hit
    * Level 24: +1 to-hit, and so on.

Leveling up grants damage bonuses (SlashTHEM)
    * Level 10, +1 damage to attacks.
    * level 20+: +1 damage bonus for every additional level gained.
    * For example: At level 25, you would get a combined total of +7 damage (+1 for reaching XP 7 and +6 for levels 20-25).


### AC PENALTIES

#### Dexterity affects AC

* Ported from EvilHack
* Being encumbered negates AC bonuses from dexterity
* Wearing any kind of heavy metallic body armor (not mithril) or other rigid material also negates beneficial AC bonuses

| Dexterity | AC change |
| --------- | --------- |
| <= 6      | +3        |
| 7-9       | +1        |
| 10-14     | +0        |
| 15-16     | -1        |
| 17-18     | -2        |
| 19-20     | -3        |
| 21-23     | -4        |
| 24-25     | -5        |

#### Encumbrance affects AC

* Being encumbered has a severe negative effect on your AC and inflicts +4AC for each level of encumbrance.

| Encumbrance | AC change |
| ----------- | --------- |
| Burdened    | +4        |
| Stressed    | +8        |
| Strained    | +12       |
| Overtaxed   | +16       |
| Overloaded  | +20       |

* **The "wounded legs" status** also inflicts a severe AC penalty for bearing weight. You get +1AC for every 100aum you are carrying while you are wounded. Many traps can cause this condition, but now the jungle boots can be useful to prevent it.

### ARMOR CHANGES

* **The protective effect of hard helmets** has been reduced when heavy objects fall on the hero's head.
* Only elves can safely enchant elven armor over +3. Other races will get a warning vibration if their elven armor is enchanted over +3.
* Worn armor has a 25% weight reduction (xnh/FIQ)
* Dwarves and elves get a +1 bonus for each racially aligned piece of armor they wear (Evil)
* Orcs and gnomes get a +2 bonus for each racially aligned piece of armor they wear (Evil/THEM)
* Plate mail now grants 8AC
* Crystal plate mail now grants 9AC
* Bronze plate mail now grants 7AC
* Leather armors don't grant any MC.

#### Dragon scales and scale mail changes

* The AC of dragon scales has been reduced from 3AC to 1AC 
* The AC of dragon scale mail has been reduced from 9AC to 4AC
* Dragon scale mail weighs 80.
* **Dragon scale mail cannot be wished for**
* Any wishes for scale mails will simply be converted to the equivalent dragon scales instead. For example, if you wish for "yellow dragon scale mail", you will receive "yellow dragon scales".
* When wishing for dragon scales, any specified enchantment is nullified to +0 (xnh)
* Green dragon scale mail also grants regeneration.

### INTRINSIC CHANGES
* Invisibility and see invisible cannot be permanently gained intrinsically (xnh)
* Telepathy cannot be permanently gained intrinsically
* Teleportitis cannot be permanently gained intrinsically.
* Teleport control cannot be permanently gained intrinsically.
* Amnesia can make you forget intrinsic telepathy.
* Intrinsic disintegration res doesn't protect items from disintegration.

#### Eating Jewelery & Accessories
* Eating rings and amulets only confers an intrinsic for a temporary period.
*  To compensate for the temporary nature of these intrinsics, the possibility of actually getting the property has been inversed.
 * Before, the chance of getting an intrinsic from a ring by eating it was 1 in 3. It has been changed to 2 in 3. The chance for an amulet by eating it was 1 in 5. It has been changed to 4 in 5.
 
** Summary of revised eating effects:**
 - Eating a ring now grants 750-1500 turns of it's property intrinsically.
 - Eating an amulet now grants 1250-2000 turns of it's property intrinsically.
 - Eating the amulet of reflection now gives intrinsic reflection for 1250-2000 turns. Previously it would not grant anything.
 - Eating the amulet of flying now gives intrinsic flying for 1250-2000 turns. Previously it had no effect.
 - Eating an amulet of life saving can reset saving grace.
  
#### Aggravate Monster changes
* Cannibalism causes aggravation for 10-15k turns instead of permanently.
* Eating domestic animals causes aggravation for 5000-7500 turns instead of permanently.
* Intrinsic aggravate monster increases monster difficulty by 5 (stacks with extrinsic).
* Aggravate monster spell cast at hero causes intrinsic aggravation for 50-300 turns.
* Aggravate monster causes monsters not to flee and not be scared of musical instruments.
* Ring of aggravate monster causes pets to attack anything without fear.
* Ting of aggravate monster increases the monster generation difficulty by 15 (this was already implemented in NetHack 3.7, but it's worth including here as a recent change)

### PARTIAL INTRINSICS

* Ported from EvilHack

* Instead of binary resistances where the player either has it or doesn't, the player gradually builds up their resistance from 0% to 100%.
* When eating a corpse, player gains a percentage of certain intrinsics instead of the full intrinsic at once.
* Percentage gained is based on the weight of the corpse; minimum being 2% and maximum at 50% (capped at 100%).
* Although the maximum percent is 50%, the percentage is calculated by taking half as guaranteed, and rolling the other half. So, instead of a dragon granting 50%, it grants 25% + (d25)%.
* Tins convey the same percentage from whatever they are made from.
* You will always get a percentage intrinsic from each corpse eaten.
* You receive all intrinsics that the corpse can convey if there are multiple intrinsics it can give (ie: eating a black pudding corpse grants a small percentage each of poison, cold, and shock resistance.)
* Damage dealt/effects felt are adjusted based on the percentage intrinsic currently possessed. Damage reduction is rounded down, requiring slightly more resistance to be effective.
* Gremlins steal half as much intrinsics (25 + d25)% instead of (50 + d50)%. This is because their intrinsic stealing attack can trigger anytime of day.
* Cold traps and ice demons steal the same amount of cold resistance as gremlins.
* Enlightenment always shows the partial percentage acquired for intrinsics. If you have an extrinsic source that will be displayed separately.

### PARTIAL REFLECTION

* Ported from EvilHack
* Reflection will deflect most, but not all, of the effects of ray attacks.
  * Example: You are hit by a cold ray, it reflects off your amulet of reflection, but you don't yet possess cold resistance.
* If you don't have sleep resistance, but you reflect a sleep ray, you will fall asleep for a maximum of 1d6 turns.
* If you reflect disintegration ray, you still take 6d6 damage unless you possess disintegration resistance.
* If you reflect a death ray, you still take damage and lose max HP. This can be mitigated by magic resistance and half-spell damage, but is impossible to fully prevent.
* Item destruction from elemental effects (like fire or cold) is prevented when rays are reflected.
* Reflection only provides partial protection from **floating eye gazes** - the player will still be subject to d6 turns of paralysis without free action. This is weighted on Luck, so the higher your Luck the better the chance to avoid the gaze.
* **Medusa's gaze** cannot be reflected back from more than 3 squares away.
* If reflected, Medusa will protect herself from her own gaze 98% of the time.


### DAMAGE CHANGES

### Gaze attack protection

* Displacement protects from gaze attacks, only letting 1 in 11 gaze attacks find the player
* Invisibility protects from gaze attacks, only letting 1 in 11 gaze attacks find the player
* Darkness offers protection from gaze attacks (as long as the player is on a dark square and the gazer doesn't have infravision and the player is infravisible).
* If a gazer is in melee range, it will bypass invisibility and darkness protection.

### SKILL CHANGES

The skill system for achieving proficiency in weapons and spells has been adapted from the UnNetHack system. In UnNetHack most of the requirements for advancing skills have been substantially increased. The major exception is that training skills from unskilled only takes 50 uses compared to UnNetHack's 100.

This chart shows the number of successful uses of a skill required to reach each level.  These values are:

| Skill level  | Successful uses | Old value |
| ------------ | --------------- | --------- |
| Unskilled    | 0               | 0         |
| Basic        | 50              | 20        |
| Skilled      | 200             | 80        |
| Expert       | 400             | 180       |
| Master       | 800             | 320       |
| Grand Master | 1600            | 500       |

* 1-damage hits train weapon/unarmed skills (Dyna)
* Riding skill is exercised more quickly, closer to vanilla (Un)
* Skill gain for spells is faster than skill gain for weapons (Un)
* Training skill in pick-axe affects how fast you can dig (Evil)
    * Skilled gives you the same bonus as a dwarf (x2)
    * Expert gives you double the bonus of a dwarf (x4)

### EXPERIENCE CURVE CHANGES

| XP Level | XP Required |
| -------- | ----------- |
| 1        | 0           |
| 2        | 20          |
| 3        | 40          |
| 4        | 80          |
| 5        | 160         |
| 6        | 320         |
| 7        | 640         |
| 8        | 1 280       |
| 9        | 2 560       |
| 10       | 5 120       |
| 11       | 10 000      |
| 12       | 15 000      |
| 13       | 22 000      |
| 14       | 33 000      |
| 15       | 50 000      |
| 16       | 75 000      |
| 17       | 113 000     |
| 18       | 170 000     |
| 19       | 256 000     |
| 20       | 384 000     |
| 21       | 576 000     |
| 22       | 864 000     |
| 23       | 1 297 000   |
| 24       | 1 946 000   |
| 25       | 3 200 000   |
| 26       | 3 520 000   |
| 27       | 3 840 000   |
| 28       | 4 160 000   |
| 29       | 4 480 000   |
| 30       | 4 800 000   |

### SPELLCASTING CHANGES

Most of these changes are to strengthen natural spellcasters abilities and to dull roles
that don't specialize (like fighters). Non-specialists can still attempt to utilize spells
but they will have to work harder to maintain their spells. Cavemen will have a very
difficult time with spellcasting.

* The base memory retention ("KEEN") for spells is now 10000 turns, reduced from 20000 (SLASH'EM). When reading or re-reading a spellbook, you will bring the retention back up to 10000
* Primary spellcasters (healers, priests, monks, wizards) get a memory boost of 500 turns when they cast spells (SLASH'EM)
* Casting your special spell also grants a retention bonus of 500 turns no matter what role you are
* Wielding a quarterstaff provides a small bonus to spellcasting (about a 1/3rd of the bonus a robe confers) (Fourk)
* A welded cursed quarterstaff doesn't block spellcasting (xnh)
* Hungerless casting ignores too hungry to cast penalty (xnh)
* Spellbooks' weight is directly related to their level (xnh)
* When casting a SKILLED attack spell, you can choose to cast basic fireball or cone of cold (xnh/dnh)
* You get a 100 turn reminder for spells that are close to fading away
* Spellcasting no longer exercises wisdom
* **Hungerless spellcasting nerf:** Total hungerless casting is not possible anymore and the intelligence requirements have been increased.
* Healing spell effectiveness is determined by skill (Evil)
* Spellbook of identify was raised to level 5 (SLASHEM)
* Cure sickness is now directional (Evil).

### ITEM EROSION AND DESTRUCTION

* Objects can be completely destroyed via rusting/rotting/corroding (Evil)
* Almost all items are erodeable/destroyable (Evil) - amulets, rings, wands, and tools are now eligible for erosion. These new erodeable items can be erodeproofed via confused enchant weapon scrolls.
* Silver items can corrode (xnh)
* The iron ball and chain cannot be destroyed from rusting (Evil)
* Poison gas clouds can rot organic armor
* Monsters can wear down and destroy **ANY** armor with the destroy armor spell (Evil)
* Item erosion can be repaired by dipping into a potion of restore ability (xnh)
* Scrolls also can burn up when hitting hot ground in Gehennom. 3.7 introduced potions being shattered when dropping on hot ground, but we have taken it a step further.
* Potions can shatter when dropped on cold floor (this shows up in Sokoban and in Gehennom)
* Getting hit by potions of acid can corrode armor. Monster acid attacks and spit also corrode armor. Passive acid attacks corrodes armor more often. Thrown potions of acid can corrode items when they hit a monster or the player.
* Water damage may disintegrate scrolls (Dyna)
* Disintegration rays can vaporize boulders

#### Refactor, unify, and nerf item destruction

* Ported from xNetHack
* This patch fixes some problems with item destruction, making it less random and more dependent on the damage dealt in the interaction. Overall, players should expect to get a more fair deal with fewer items destroyed.

### NEW GREASE EFFECTS

Many of these changes were introduced to work in conjunction with the new grease trap.
* Greased items can't be disarmed with a bullwhip
* Greased items are harder to steal
* Glib hands makes applying any item except towels drop them
* Towels can be used to remove grease from specific objects (with the risk that they in turn
  become greased)
* Grease can be washed off towels by wetting them
* Greased towels now operate the same way that cursed towels do
* Grease can be washed off your feet/boots by dipping '-' in water, same action as dipping the player's hands. 
* Kicking monsters can sometimes get the grease to wear off your boots/feet.


### FORGING & FORGING RECIPES

* Ported from EvilHack with modifications.
  * No artifact forging
  * No forging armor
  * Much narrower list of forgeable weapons, mostly bladed and blunt weapons.
  * Only samurai can forge katanas and tsurugi. No other restrictions on other items.
  * Forging recipes are displayed in the object lookup.
    
Aside from the recipe changes - the biggest change is that we no longer have a #forge or #craft command. Simply get a hammer and (a)pply it when standing over the forge.

### GEM ALCHEMY

* Ported from UnNetHack, originally from SLASH'EM.
* This allows you to dip a gem into a potion of acid, to alchemize a potion with a specific appearance.
* This adds some serious value to potions of acid and most gems.
* Gem alchemy recipes can be viewed in the object lookup entry for "potion of acid". Other potions and gems should display their respective recipes.

## NEW MONSTERS

| Monster              | sym | origin        | changes                                                                                 |
| -------------------- | --- | ------------- | --------------------------------------------------------------------------------------- |
| giant praying mantis | a   | SpliceHack    | Ignores Elbereth and all magical scaring                                                |
| locust               | a   | EvilHack      |                                                                                         |
| third eye        | e   | SLASHEM/YANI      |                                                                                         |
| glowing eye          | e   | SLASH'EM      |                                                                                         |
| blinking eye         | e   | SLASH'EM      |                                                                                         |
| kamadan              | f   | SLASH'EM      | recolored to light green<br/>can jump and has infravision<br/>has poisonous snake bites |
| weretiger            | f/@ | SLASH'EM      | can jump, red                                                                           |
| deep one             | h   | SLASH'EM      |                                                                                         |
| deeper one           | h   | SLASH'EM      |                                                                                         |
| deepest one          | h   | SLASH'EM      |                                                                                         |
| alhoon               | h   | EvilHack      | not covetous, now speed 15<br/>can displace monsters                                    |
| redcap               | i   | SpliceHack    |                                                                                         |
| diamond piercer      | p   | SpliceHack    |                                                                                         |
| god piercer          | p   | SpliceHack    |                                                                                         |
| landshark            | q   | SpliceHack    | recolored to bright blue                                                                |
| jumping spider       | s   | SpliceHack    | May appear in small groups                                                              |
| will-o'-the-wisp     | y   | SpliceHack    |                                                                                         |
| zoo bat              | B   | SpliceHack    | Eating makes you confused                                                               |
| athol                | B   | SLASH'EM      | increased size, weight, and nutrition<br/>strong, berserks, flanks, and has infravision |
| byahkee              | B   | SLASH'EM      | recolored to yellow                                                                     |
| nightgaunt           | B   | SLASH'EM      | recolored to purple                                                                     |
| gray fungus          | F   | Evil/THEM     |                                                                                         |
| adherer              | M   | SpliceHack    |                                                                                         |
| ha-naga              | N   | SpliceHack    |                                                                                         |
| alchemist            | Q   | SpliceHack    | can alchemize acid potions                                                              |
| troll mummy          | M   | SLASH'EM      |                                                                                         |
| vampire mage         | V   | SLASH'EM      |                                                                                         |
| merfolk              | ;   | Splice/THEM   | Changed to bright green                                                                 |
| thing from below     | ;   | SpliceHack    | can see invisible                                                                       |
| grave troll          | T   | SpliceHack    | can spawn in graves/graveyards<br/>                                                     |
| elven cleric         | @   | EvilHack      | (was elven wizard in Evil)                                                              |
| like-like            | P   | NerfHack      | Can eat your shields and cloaks when engulfing                                          |
| ogre mage            | O   | SLASH'EM      |                                                                                         |
| shadow ogre          | O   | SLASH'EM      | Spawns invisible, drain life attack                                                     |
| ghoul mage           | Z   | SLASH'EM      |                                                                                         |
| lava demon           | &   | Convict Patch | Can emerge from forges                                                                  |
| assassin bug         | a   | SLASH'EM      | Stronger                                                                                |
| shadow               | X   | SLASH'EM      |                                                                                         |
| giant anacondas      | S   | EvilHack      |                                                                                         |
| giant centipede      | s   | EvilHack      |                                                                                         |
| velociraptor         | z   | SpliceHack    | Stronger                                                                                | Only appears for cavemen. Same strength as SLASHEM's kangaroos. |
| T-Rex                | z   | SpliceHack    | Can berserk                                                                             | Only appears for cavemen. Can berserk. Can roar.                |
| acid sphere          | S   | Splice/Evil   |                                                                                         |

### New demons lords:
* Kostchtchie (Splice)
* Lolth (Evil)
* Buer (Splice)
* Baphomet (Splice)
* Malchanthet (Splice)
* Mephistopholes (Splice)

## MONSTER CHANGES

### Dangerous piercers
* All piercers are mindless and can grow up
* Much more AC is required to dodge dropping piercers (before -2AC would nullify their drop attacks, now -22AC is required)
* Piercing damage scales with their level (monster level * 6) with a minimum of 4d6 being dealt.
* Piercers actually pierce helmets; if the damage roll is (12 + (helmet enchantment * 6) or greater, any hard helmet blocking the attack is destroyed. If a helmet is destroyed in this fashion, it absorbs some of the damage.
* Piercers and lurkers/trappers always generate hidden if possible. 

### Reviving and Poisonous Zombies
* Zombie corpses may auto-revive similar to trolls (Evil/xnh)
* Cancelled or beheaded zombies and trolls don't revive (Evil)
* Wielding Sunsword prevents zombies corpses from appearing (Evil)
* Playing as a priest reduces the chance of zombie revival by 50% (Dyna)
* All zombies get an additional poisonous bite attack that can drain constitution.
* Sometimes zombies will try to bite the players legs, inflicting wounded legs for a short time.

### Demons
* Many major demons have been given flight (xnh)
* Ice and bone devils are now lawful (xnh)
* ice devils have speed 8 (K-Mod)
* ice devils' cold sting and claw attacks have been buffed, they have the power to strip cold resistance from the player or monsters (xnh)
* pit fiends have speed 8 (K-Mod)
* Lava demons are huge
* Horned devils get a butt attack (because horns)
* Demonic bribes are much more expensive.

### Dragons
* Overall, dragons have been overhauled to more closely resemble the versions in SLASH'EM.
* An attempt has been made to make each dragon have a special quality or perk.
* Part of the challenge in SLASH'EM was that adult dragons (and therefore dragon scales) were more difficult to come by. Baby dragons are plentiful and can potentially be tamed and grown up into adults, but with the large gap in levels the process is long and difficult. It's possible they might not be guaranteed in Ludios or the Castle anymore either, but the increased frequency means they should show up in Gehennom much more often.

#### Baby dragon changes
* All baby dragons are level 4 and difficulty 7 (SLASHEM)
* Reduced their size from HUGE to LARGE (eliminates possible knockback on the player)
* Reduced their weight from 1500 to 1000.
* black baby dragons are difficulty 9 since they can drain life
* They can generate randomly in the dungeon with a frequency of 1, but not in Gehennom
* Baby dragons get a special 1d6 bite attack instead of a 2d6 physical bite (K-Mod).
  * For most dragons, it matches their adult breath attack (red = fire bite, blue = shock bite, etc)
* All baby dragons get an additional 1d6 claw attack

**Specific tweaks:**

* baby dragon alignments match their adult counterparts (Evil)
* baby red dragons can berserk
* baby blue dragons are slightly faster at speed 12.
* baby green dragons are slightly higher level and difficulty, and regenerate.
* baby yellow dragons also get a passive acid attack.
* baby gray dragons also flank.
* baby white dragons are weaker.
* Baby gray dragons get a disenchanting bite.
* Baby black dragons get a drain life attack.

#### Adult dragon changes
* They get a 3d8 bite and 2d4 claw attacks, and are frequency 2.
* speed has been increased from 12 to 20, and have a small buff to their claw attacks (FIQ)
* all dragons stalk/follow the player (FIQ)

**Specific tweaks:**
* red dragons can berserk
* blue dragons are faster (speed 24)
* green dragons are slightly higher level and regenerate
* orange dragons get a engulf digestion attack
* black dragons get a terrifying roar
* yellow dragons get a passive acid splash attack
* white dragons are weaker than other dragons
* shimmering dragons get teleport control (still deferred)
* gray dragons can flank.

### Misc monster changes

* all quest GUARDIAN colors were changed to cyan
* all A monsters are immune to death magic (xnh)
* baluchitherium is now huge; strengthened claw attack from 5d4 to 5d12; increased difficulty
* all bats can see invisible
* captains are considered princes (xnh)
* captains and watch captains generate with keys (Evil)
* centaurs will keep their distance from the player naturally (xnh)
* changlings turn back to their base form when killed (SLASH'EM)
* couatls get sleep and shock resistance (Fourk)
* couatls get a stunning gaze and can generate invisible
* dragons, nagas, and golems don't balk at approaching as much.
* all elementals resist sickness
* elf-lords get 9AC, elvenkings get 8AC (K-Mod)
* ettins count as giants and are vulnerable to sling damage
* floating eyes inflict less passive paralysis; wisdom limits duration (Dyna)
* fog clouds don't leave traces of steam (so they show up as v)
* foocubi gain a level when draining one from the player (xnh)
* giant spiders can ensnare monsters in webs (Evil)
* gnome lords and kings always get gnomish suits.
* gnomish wizards always get a gnomish helm.
* gnomes get candles in the mines twice as often as before
* goblins can generate in small groups (Spork)
* grave trolls no longer have thick skin (they used to in SpliceHack)
* green slimes can hide on the ceiling (xnh)
* green slimes are faster, going from 6 to 13 speed)
* green slimes have a passive sliming attack (Grunt)
* gremlins can steal intrinsics no matter the time of day (FIQ)
* hezrou and steam vortices don't leave clouds unless they moved. This guarantees that they won't obscure their own visibility with self-generated clouds.
* hobbits can get flint with their slings (xnh)
* jellyfish get a passive paralyzing attack
* Keystone Kops cannot be genocided (Un)
* Keystone Kops are tougher: they flank and have increased levels, speed, and attack damage; removed their wander flag (K-Mod)
* leprechauns do not stash gold in the ground after stealing it (reverted from 3.7)
* lizards appear with slightly less frequency
* ki-rin get shock, sleep, cold, and poison resistance (xnh)
* lords and princes never get negative weapons or armor (xnh)
* lieutenants are considered lords (xnh)
* master liches and arch-liches can see invisible (FIQ)
* mastodon is now huge; strengthened butt attacks from 4d8 to 4d16; increased difficulty
* mastodon gets a hug attack and can berserk (Evil)
* mind flayers are bright magenta
* mind flayer attacks can make hero forget skills (Evil)
* minotaurs resist death magic (SLASHEM)
* minotaurs have a thick hide
* Mordor orcs can spawn with orcish boots
* mummies get a nasty withering attack (xnh/Evil)
* nazgul can shriek, inflicting stun damage (xnh)
* olog hai get poison resistance
* orc captains now are lords and have speed 9 (xnh)
* orc shamans and kobold shamans are skittish (FIQ)
* priests of Moloch are always generated hostile (SLASHEM)
* quasit buffs: faster, stronger attacks, they now see invisible, and they can appear in small groups (xnh)
* queen bees can displace monsters
* quest leaders resist death magic (Evil)
* rock trolls are stoning resistant (xnh)
* all spheres (shocking spheres, flaming spheres, freezing spheres) cannot be genocided.
* all spheres also explode on death (shocking/flaming/freezing/acid)
* skeleton/shade slow attack is ineffective vs undead
* soldiers get half as many C-and-K-rations and cannot load both types of rations (K-Mod)
* soldiers and their higher ranks get level, speed, AC, and MR boosts (K-Mod)
* Soldiers can generate with shuriken
* sewer rats hide under objects (xnh)
* scorpions are tiny
* shades get 20MR
* shopkeeper base level has been raised to 13 (xnh)
* shopkeepers and priests are colored yellow (xnh)
* titans can see invisible (FIQ)
* titans resist death magic (SLASHEM)
* titans are level 17 (K-Mod)
* tigers are orange (Evil)
* tigers can also jump
* titanothere is now huge; strengthened claw attack from 2d8 to 8d8; increased difficulty
* trappers and lurkers above are mindless and speed 6
* troll meat provides temporary intrinsic regeneration (xnh)
* unique monsters cannot be tamed
* violet fungi get a passive hallucination attack
* all vortices (v) resist shock damage
* vampire mages can see invisible
* all werefoo in animal form get infravision
* Wargs have a thick hide.
* werefoo revert back to their base form when killed (SLASH'EM)
* werewolves have a higher level and difficulty, stronger attacks
* weretigers have a higher level and difficulty, stronger attacks
* wraiths also no longer "stalk" the player and follow them across levels (Dyna)
* wumpus is now huge; strengthened bite attack from 3d6 to 6d9; increased difficulty
* xans can't fly (dnh)
* yellow and black light explosions are directionless (xnh)
* yellow molds puff out clouds of stunning spores (as a corollary, pets will attack them less often now)

### Unique monster changes
* Croesus can move other monsters out of his way (Evil)
* Ixoth can berserk. Like other dragons also has buffs: level raised from 15->18, speed raised from 12 to 20, AC raised from -1 to -4, stronger claw attacks.
* Ixoth gets poison resistance (Evil)
* Lord Surtur can berserk
* The Master Assassin is poison resistant (xnh)
* The Master Assassin is stronger, faster, sees invisible, resists sleep, and gets one additional attack.
* Yeenoghu's magic missile attack has been buffed to 6d6 (Evil)
* Vlad gets stoning resistance.

#### Medusa
Inspired by EvilHack, Medusa gets an overall difficulty boost:
* She goes from level 20 to 24
* She gets -8AC (a big buff from 2AC)
* Her weapon attack goes from 2d4 to 4d4
* Instead of a single poisonous bite, she gets three poisonous snake bite attacks.
* Medusa gets infravision

#### Wizard of Yendor
* Rodney is bright magenta (Evil)
* Rodney will never steal the quest artifact of the current role (Un)
* Rodney gets a strong weapon and the ability to use it (Evil)
* Possible vampire mage guarding Rodney
* Guaranteed thing from below guarding Rodney.

### MONSTER BEHAVIOR

#### Monster item use

* Monsters can use figurines and magic flutes (Evil)
* Monsters can use scrolls of remove curse (Evil)
* Monsters can throw (lit) potions of oil at you (xnh)
* Monsters can throw potions of polymorph (Evil)
* Monsters can throw potions of hallucination at you (xnh)
* Monsters can zap wands of cancellation at the player (Evil)
* Monsters can read scrolls of stinking cloud (Evil)
* Hostile monsters wielding a digging tool can break boulders (Evil)
* Monsters can quaff potions of restore ability to un-cancel themselves (Evil)

#### Steeds

* Steeds are more aggressive - if your steed has a tameness level of 15 or more, it will actively attack monsters instead of merely reacting to being attacked. (Evil)

#### Misc monster behavior changes

* Monsters with a negative AC get damage reduction from melee attacks (Evil)
* Monsters will switch to their melee attack intelligently (Spork)
* When a monster spawns with a weapon, it wields it immediately (xnh)
* Intelligent monsters pick up keys and lock picks (Un)
* Magic-liking monsters will pick up magical tools (xnh)
* Covetous monsters will equip wearable items that they target (xnh)
* Monsters will use ranged combat in melee as a fallback option (Grunt)
* Monster stunning has been implemented to more closely mirror the effects it has on players (xnh)
* Prevent some super strong monsters from generating in the mines
* Add more spears in monster starting inventory (Fourk)
* Hallucination protects against skeleton bone rattling (xnh)
* Headless and breathless monsters don't cough in poison gas clouds
* Players can use gaze attacks in melee range when polymorphed into monsters with a gaze attack.
* Monster knocking you (or other monsters) back is noisy.
* Conflict negates Elbereth and scare monster protection (Evil)
* You can't dust engrave while being held by a monster.
  
#### Flanking behavior

* Ported from SpliceHack, with enhancements
* Monsters with this property have the M2_FLANK tag.
* Any two monsters can flank a player (or another monster) if they sandwich the target. However, monsters with this property ("outflankers") are more tactical and will actively seek opportunities to flank you.
* Monsters gain a large to-hit bonus when flanking
* Flanking now scales with monster level (it used to be a flat +4 AC penalty in SpliceHack):
  * AC penalty = 4 + (mdifficulty - 4) / 2
* Flanking has been applied to many monsters in NerfHack.

* Using a pet, you can also take advantage of flanking. Simply place yourself and your pet in such a way as to "sandwich" the monster. You (or your pet) will get a flanking bonus on the victim when attacking.

Flanking restrictions:
* You cannot flank if hallucinating, afraid, confused, punished, fumbling, wounded, unaware, or stunned.
* You must be able to see the monster you want to flank.
* Monsters cannot flank if eating, sleeping, fleeing, confused, stunned, trapped, petrified, sick, diseased, or hiding.

#### Berserking behavior

* Ported from EvilHack, with modifications
* Monsters with this property have the M3_BERSERK tag and can be quite dangerous if you take them for granted
* When berserkers are below 50% of their health, they have a high chance to go into berserk mode
* Monsters can also immediately go berserk if they are woken and angered
* When a monster goes berserk it turns hostile and regains a roll of it's max HP, possibly
  recovering all of its HP.
* Nearby denizens are also woken up when a monster goes berserk (it screams a battle cry)
* When berserking, monsters totally ignore Elbereth or Scare Monster. If they are usually skittish or trying to keep away, they will instead actively approach
* Berserking monsters also never flee when their HP gets low
* A berserking monster deals double damage rolls when hitting you
* Taming berserking monsters only un-berserks them, it doesn't pacify or tame
* Monsters that can berserk: all dwarves, mordor orcs, uruk-hai, mumaks, zruty, fire giants, frost giants, storm giants, ettin, all ogres, owlbears, sasquatch, and balrog.
* Berserkers get angry when stuck in traps.

#### Rabid monsters

This is a brand new mechanic, debuting in NerfHack!
* The rabid rat has been removed and in its place any eligible monster can generate as a rabid version of itself. Any place in the code where rabid rats were previously, has been replaced with wererats.
* There is a fairly small probability of a monster spawning rabid, but bats and coyotes always have a 1 in 10 chance of spawning infected.

Effects of the rabid status on monsters:
* Rabid monsters get an additional bite that can cause the player to become rabid. This bite attack is also poisonous (damaging CON), similar to the rabid rat.
* Rabid monsters don't regenerate
* They grudge all non-rabid monsters (that are capable of catching rabies).
* They occasionally move erratically (from confusion)
* They will never flee or become scared and will actively approach.
* Rabid monsters cannot quaff potions.
* Rabid monsters cannot be tamed.
* If a tame pet becomes rabid, it immediately loses its tameness.
* Rabid monsters grant a little extra XP.

Effect of being rabid on the player:
* You cannot regenerate
* You become bloodthirsty in your attacks (similar to wielding Stormbringer).
* You occasionally move erratically - 1 in 10 moves is confused.
* When the player is infected a timer starts from 100 + d(CON*2) turns.
  * At 40 turns, you develop a fear of water and cannot quaff potions.
  * At 10 turns, you become confused.
  * At 0 turns, you die.

Curing rabid:
* Generally the same guidelines for illness apply, you can apply a unicorn horn, drink healing potions (in the early stages), cast cure illness, pray (counts as a major trouble), or eat a eucalyptus leaf.
* Rabid monsters that poly can stop being rabid if the new form is immune - the same goes for the player.

#### Diseased monsters

* Ported from EvilHack
* Monsters can become infected with terminal illness, with a short countdown to death.
* Monsters can cure themselves if they have the means, and the player can use cure sickness or eucalyptus leaves to heal sick pets.

#### Accurate behavior

* Ported from EvilHack, with modifications
* Monsters with this property have the M3_ACCURATE tag 
* Some monsters are more accurate in melee and with projectiles
* These monsters get a large to-hit bonus of +5 or more
  * all piercers, all centaurs, all elves, all mercenaries, 
  * Dwarf king,  orc-captain, gnome lords, kop kaptains, ogre kings,
  * Uruk-hai, scorpions, angels, archons, titans, cobras, olog hai, Vlad, Nazgul, shopkeepers, nurses, sandestin, hunters, ninjas
  * Scorpius, Master Assassin

* Players are the elven starting race or polymorphed into elves also enjoy a to-hit bonus that scales with your level.

#### Ported jumping behavior

* Ported from EvilHack and SpliceHack
* These monsters can jump at you from a few squares away, quickly bridging the gap between you
* They can also cross short barriers like water and lava

## MONSTER SPELLCASTING

* Peaceful monsters won't cast make invisible on themselves. They also won't drink potions
  of invisibility or zap themselves with wands of make invisible.
* Monster spellcasters will prioritize healing when wounded.

**protection (clerical spell):**
* Ported from EvilHack
* This is the monster version of the protection spell already available to the player.
* Provides a temporary magical shield that increases the monster's AC protection.
* Can be dissipated with a blast of cancellation.

**reflection (mage spell):**
* Ported from EvilHack
* A spell that creates a shimmering globe around the caster, granting them reflection for several turns.
* Can be dissipated with a blast of cancellation.

**acid blast (mage spell):**
* Ported from EvilHack
* Explodes an acid blast on its target and the surrounding squares. The damage output is dependent on the level of the monster casting it.
* The acid from this spell also has a chance of eroding any unprotected weapons or armor in open inventory.
* Ranged, can be cast at the hero up to 13 squares away.


**ice bolt (mage spell):**
* Ported from EvilHack
* This spell explodes a small ice storm upon its target (and surrounding squares)
* Any non-protected objects in open inventory are subject to being frozen.
* This is a low-level spell, so access to this spell is given to every monster spellcaster that has access to mage-based spells.
* Ranged, can be cast at the hero up to 13 squares away.

**fire bolt (mage spell):**
* Ported from EvilHack
* This spell explodes a small fireball upon its target  (and surrounding squares)
* Any flammable objects in open inventory are subject to being burned.
* This is a low-level spell, so access to this spell is given to every monster spellcaster that has access to mage-based spells.
* Ranged, can be cast at the hero up to 13 squares away.

**destroy armor (mage spell):**
* Altared from Vanilla NetHack, ported from EvilHack
* Having magic resistance is no longer full protection against this spell. Any piece of armor being worn can have its fixed status removed, and then can be deteriorated to the point that it's completely destroyed. Even armor that is normally erodeproof (dragonhide and dragon scales, etc) is affected. Having MR keeps the erosion level at one per cast, otherwise the erosion level is of one to three levels per cast. Blessed pieces of armor have a small chance of resisting. Armor-based quest artifacts are immune to this spell, as is crystal plate mail.

**geyser spell (clerical spell):**
* The core spell is unchanged from Vanilla NetHack, however now the geyser also rusts armor and instakills iron golems (Evil)

**entomb (mage spell):**
* Ported from xNetHack
* Mage spell. (xnh).
* Used by a monster when they are low on health or fleeing. It is primarily for escape and when cast surrounds the player with boulders. 
* Any mage-spellcaster can use it when desperate.
* In xnh there was also a chance to create solid walls to block the player in, this effect was removed so it only drops boulders.

**hobble (clerical spell):**
* Clerical.
* Inflicts wounded legs on you
* This clerical spell smashes the hero's legs with a magical force and inflicts you with wounded legs for 50-149 turns.
* Ranged, can be cast at the hero up to 13 squares away.

**call undead (mage spell):**
* Ported from SLASHEM
* Call Undead can only be cast by undead and demon spellcasters
* Ranged, can be cast at the hero up to 13 squares away.

**blight (clerical spell)**
* Ported from xNetHack
* In xnh this spell was reserved for 'dark speech' - a nasty group of curses that Asmodeus and Demogorgon can use. But I thought it would be pretty cool if extracted out and used as a new clerical spell. Not too many monsters use clerical spells, but they tend to be potent. The spell itself is pretty straightforward: it inflicts withering on the player. Since withering cannot be cured, this could end up quite dangerous if multiple blights are cast.

    In xnh, the duration of the withering was 100-140 turns. For the big demons this might fly, but for lesser spellcasters I reduced it to 20-60 turns. In xnh I believe this could only be cast in melee range, but now it can also be cast up to 8 squares away - further increasing its deadliness.
* Being polyd into a non-living form protects against the blight spell.

**evil eye (mage spell):**
* Ported from dNetHack
* When successfully cast on the hero, this lowers your Luck by 1 point.
* Evil eye can only be cast by undead and demon spellcasters.
* Because this is implemented as a gaze attack, the player can increase their protection by being invisible or displaced. There is no maximum range to this spell.

**cure self**:
* Spellcasters can use Cure Self for illness, blindness, withering, and rabid statuses.

## ROLE CHANGES

### ARCHEOLOGIST
* An Archeologist wielding a bullwhip will not fall through trap doors (SLASHEM)
* Archeologists get bonus when searching (FIQ)
* Archeologists can reach basic skill in spears.
* Archeologists can reach basic in axe.
* Archeologists start out knowing dwarvish mattocks.
* Archeologists always get an extra id when reading scrolls of identify.
* Archeologists start with an extra scroll and spellbook (SLASHEM).

**Archeologists vs snakes!**
* Archeologists get a -1 to-hit penalty when fighting snakes (any S class monsters).
* Snakes get a +1 to-hit bonus on archeologists
* All snakes have the potential to paralyze archeologists in fear when they successfully connect a hit. Free action only protects the hero 75% of the time vs these paralyzing attacks. 
* Some giant anacondas have a chance of appearing in the arc quest now.

### BARBARIAN
* Barbarians can reach skilled in riding (Evil)
* Barbarians get a blood rage bonus for low health.
    * Only occurs when barbarians reach level 4 and higher.
    * When under 50% of their max HP, they get a damage bonus that scales with their level.
    * When under 25%, this bonus is doubled.
    * This feature was adapted from the SpliceHack skill system.

### CAVEMAN/CAVEWOMAN CHANGES
* They cannot receive spells from their deity (Evil)
* They have an 80% chance of failing to read any spellbook
* They can increase their max-HP at each level-up if they remain illiterate (Spork/THEM)
* Their special spell has been removed (Evil)
* When reading scrolls of identify, cavemen will never be able to identify all items, they will be instead identify 1 instead.
* The caveman quest has been updated and filled with more jungle type monsters: tigers, pythons, and the like. There is also a lot of water added and ; monsters to occupy it (from SlashTHEM)
* Chromatic Dragon: Like other dragons also has buffs: level raised from 15->18, speed raised from 12 to 20, AC raised from -1 to -4, stronger claw attacks.

Cavepeople have also been gifted with more skills in rudimentary tools like rocks and flint:
* They start the game with more flint and no rocks (xnh)
* Cavemen can lash flint to arrows, making them do slightly more damage (Spork/THEM). When arrows are flinted, their enchantment is also revealed.

* The narrow passageways in their quest have been opened up for convenience (Evil)
* Their quest narration and dialogue is more caveman-like (xnh/Fourk)
* Cavepersons can get an alignment boost via cannibalism (Spork)
* Cavepersons' gods sometimes don't respond to prayer. There is a 10% chance of being ignored (Spork/THEM)

* Skill adjustments for cave dwellers (Evil)
    knife:          Skilled     -> Restricted
    dagger:         Basic       -> Restricted
    polearms:       Skilled     -> Restricted
    morning star:   Basic       -> Restricted
    unicorn horn:   Basic       -> Skilled
    attack spells:  Basic       -> Restricted
    matter spells:  Skilled     -> Restricted
    riding:         Restricted  -> Basic

* Cave dwellers also cannot have skills in edged or pointy weapons unrestricted. Note that they can still receive these weapons as altar gifts. The exception is unicorn horns, which the cave dwellers can reach skilled in.
* Cavemen get Keolewa as their first sacrifice gift.

### HEALER
* Add L's Wounds patch: healers can see damage on monsters
* Healers start with 2 eucalyptus leaves.
* Healers get a large bonus when applying unicorn horns
* Healers can use an uncursed unicorn horn as if it is blessed.
* Healers get sickness resistance instead of warning at level 15 (Evil).
* Cyclops can berserk

### KNIGHT
* Only lawful Knights can dip for Excalibur (Evil/Spork)
* Knights start with a +0 studded leather armor instead of a +1 ring mail (K-Mod)
* The knights quest has been infested with a swarm of merfolk

Skill adjustments for knights
    dagger          Basic       -> Restricted
    knife           Basic       -> Restricted
    axe             Skilled     -> Restricted
    pick-axe        Basic       -> Restricted
    club            Basic       -> Restricted
    trident         Basic       -> Restricted
    crossbow        Skilled     -> Restricted
    broad sword     skilled     -> Expert
    polearms        skilled     -> Expert
    spear           skilled     -> Expert

### MONK
* Dramatically increased the monk's body armor penalty (Evil)
* Player feedback for monks wearing/removing body armor
* Stop giving Monks "You feel guilty message" eventually (xnh)
* Removed crossbow skill.
* Monks can reach expert in quarterstaff.

### PRIEST
* Priests start with a +2 small shield (SLASHEM)
* Priests cannot have edged weapon skills unrestricted (Evil)
* Priests don't receive edged/pointy artifact weapons via altar sacrifice (Evil)
* Instead of the standard crowning gift, priests always receive Mjollnir (Evil)
* Priests reduce the chance of zombie revival by 50% (Dyna); when a zombie is killed for good, you get a special message
* Priests can reach basic in riding skill.
* Priests start with more garlic and wolfsbane (similar to the undead slayer in SLASH'EM)

### RANGER
* Rangers get extended range for seeing object's dknown appearance (this lets them see potions and gems from much further away)
* Rangers get auto-id for launchers when they reach XP level 7
* Rangers get auto-id for ammo enchantment when they reach XP level 10 (xnh)
* Rangers are not stunned from using portals (they are used to quick travel)

### ROGUE
* In the Rogue quest, some hidden doors were added to the Master Assassin's lair to make accessing the nemesis a little easier.
* Rogue's can inflict **backstab damage** for the first thrown weapon. In 3.4.3 this was a very powerful mechanic that was nerfed in 3.6. We are bringing it back in a limited form as a callback to 3.4.3 but also because it strongly fits the theme of the role.

* Rogues get bonus backstab damage when using stilettos in melee
* Rogues also get a multishot bonus for knives.
* Rogues start with a +2 stiletto instead of a short sword
* Rogues start with a stack of knives instead of daggers
  
**Rogues can counterattack while wielding knives and daggers:**
* While wielding a knife or dagger, a rogue has a chance of counter-attacking an opponent. There are many restrictions:
  * Their attack must be a weapon, bite, claw, or kick attack type.
  * You can't be polymorphed
  * You can't be wearing any heavy metallic armor or wielding a bulky shield.
  * You cannot be weak (or worse from hunger), and you cannot be encumbered.
  * You cannot be fumbling or unaware (sleeping or paralyzed).
  * You must be able to see the monster.
  * The chance of countering goes up with your skill in the wielded weapon.

### SAMURAI
* Samurai start with +3 wakizashi (Dyna)
* Samurai can reach expert in spears.
* Samurai get to-hit and damage bonuses for twoweaponing a katana with a wakizashi.
* The samurai quest was updated to have more water and monsters (jellyfish, more ninjas, some nagas).

### TOURIST
* Tourists get automatic type identification for shop items (Un)
* Tourists start with more darts to compensate for more training being needed to advance weapon skills (Un)
* Tourists start with all of their optional equipment (FIQ)

### VALKYRIE
* More fire traps on valk quest
* Lord Surtur can berserk now

### WIZARD
* Most of the wizard's combat based skills have been restricted and removed (Evil)
  * knife, axe, short sword, club, mace, polearms, spear, trident, and shuriken skills
* Wizards start with a cloak of protection instead of magic resistance.
* Wizards always start with the spellbook of magic missile.

## NEW ROLES

### CARTOMANCER
* The cartomancer is a unique role ported over from SpliceHack. Cartomancers are spellcasters with a focus on using scrolls and summoning temporary minions to do their bidding. Many parts of the role are inspired by or pay homage to various trading card games.

**Starting inventory:**
    * Fedora
    * Graphic tee
    * 40 +0 razor cards
    * 2 random cards
    * 4 random summon cards
    * 2 random zap cards
    * 1 random spellbook

**Skill-set:**
    * Dagger: basic
    * Knife: basic
    * Quarterstaff: skilled
    * Sling: basic
    * Dart: basic
    * Shuriken: expert
    * Unicorn horn: basic
    * Attack spells: basic
    * Healing spells: basic
    * Divination spells: expert
    * Enchantment spells: skilled
    * Escape spells: basic
    * Matter spells: basic
    * Riding: skilled
    * Bare-handed combat: basic

**Quest artifact: Holographic Void Lily**
    * Chaotic credit card
    * Intelligent
    * Grants magic regeneration while carried
    * Grants half spell damage and reflection while carried
    * Can be invoked to summon a horde of tame spell beings.

* While playing as a cartomancer, much of the standard NetHack terminology is revised:
    * scrolls are renamed to "cards". Whenever you or a monster reads a scroll, they instead
      "play" that card.
    * scrolls under $100 are labeled as "common"
    * scrolls for $100 are labeled as "uncommon"
    * scrolls for $200 are labeled as "rare"
    * scrolls for $300 are labeled as "legendary"
    * spellbooks are renamed to "rulebooks"
    * credit cards are known as "banned cards"
    * boomerangs are "bent cards"
    * expensive cameras are "holographic cards"
    * hawaiian shirts are "graphic tees"
    * lock picks are "worthless cards"

**Play mechanics:**
* Cards (ie: scrolls) only weigh 1 for cartomancers.
* The camera is played as a holographic card for cartomancers, doesn't break when thrown.
* When applying a deck of cards, cartomancers will always be able to use them as if they
  were blessed. This enables you to tell your current luck easily by applying the deck.

**Card abuse penalties**:
* Cartomancers receive severe alignment penalties for forging or defacing cards. 
  - writing cards: -20 alignment, -5 luck
  - cloning cards: -20 alignment, -5 luck
  - poly zap/dip of cards: -10 alignment, -2 luck


**Spell beings:**
* Spell beings originally came from SLASH'EM. Whenever the flame sphere or freeze sphere
  spells were cast, they would summon a temporary sphere which counted as a spell being.
  These beings are tame and act like pets, but they have a limited life span. (In SLASH'EM
  there was no life span unless you left them on a level to become untame). Here, when the
  cartomancer plays a summon card - it will summon a spell being with a predetermined life
  span that will fight aggressively for you. If you get credit for killing a spell being,
  they only ever grant 1XP. Spell beings also never leave corpses and spawn with no
  inventory.

**Summon cards:**
* Cartomancers will start out with a few summon cards, and they will also have the
  opportunity to build a collection of them as they slay monsters. Low level monsters rarely
  drop their own summon cards, but any death drop has a small chance to leave a higher level
  monster. As your level grows, so does the strength of the rare drops.
* The price of summon cards scales with their monster difficulty.
* In addition to reading summon cards, cartomancers can also throw them to activate them.
  This lets you keep monsters at a distance by throwing the summon directly next to the
  threat.
* Monsters can read summon cards as well.

**Razor cards:**
* In SpliceHack, razor cards were simply shuriken relabeled.
* In NerfHack, razor cards have been properly implemented as their own weapon type using the shuriken skill.
* Deals d6 vs small and d6 vs large, +2 to-hit, weighs 1.
* Cartomancers recognize the enchantment and BUC status of all razor cards.
* Razor cards will appear as part of the cartomancers regular death drops and will sometimes
  take the place of a summon card or zap card. These follow the same rules as any stacked weapon type, so you may receive a stack of 6-11 that could be blessed/cursed/uncursed, and possibly poisoned.

**Zappable cards:**
* These can also drop when cartomancers kill monsters. They act as one-use wands. These have a 0% generation chance so that other roles will not see them randomly, but they could see them in bones.

**Changes to the cartomancer quest:**
* Created a unique duelist monster to take the place of students in the cartomancer quest.
* The cartomancer quest levels have received some updates and detailing.
* Buffed cartomancer quest leader.

Cartomancer gets adjusted different item generation odds.
    To make up for less corpse drops, they get more food.
    They also get much fewer wands because they get zap cards.

Cartomancers get speed at level 10. This is sort of my lazy way of implementing the card combo technique from the original SpliceHack. This lets the cartomancer get a larger benefit though and the player doesn't have to do anything special, they can just cast more cards naturally.
The cartomancer also starts with a fedora.

## PLAYER RACE CHANGES

* Removed infravision from dwarves, elves, gnomes, and orcs. 
* Added infravision to vampires - they are the only race that starts with infravision.
* Elves can always squeeze between two trees (xnh)
* Elves get see invisible at level 8
* Elves can always reach Basic in enchantment spells (xnh)
* Dwarves can always reach Skilled in pick-axe (xnh)
* Gnomes are good at slipping free from grabbing attacks
* Gnomes start with a nightvision radius of 2 (dnh)
* Gnomes start with an interesting tool
* Gnomes get stealth at level 5 (SLASHEM)
* Gnomes get a damage bonus for shooting crossbows
* Gnomes can always reach Skilled in crossbow
* Gnomes can always reach Basic in club (xnh)
* Orcs start with sickness potion (Spork)
* Orcs get an alignment boost for cannibalism (dnh)
* Orcs can always reach Skilled in saber (xnh)

### New race/role combos.

* Elven archeologist
* Elvish healer
* Dwarven knight
* Dwarven priest
* Orcish priest
* Elvish rogue
* Gnomish rogue
* Elvish tourist
* Gnomish tourist
* Dwarven barbarian

### Racial item preferences

* Monsters of certain races will usually prefer their own equipment and find other racial equipment awkward or uncomfortable to use.
  * Elves hate dwarvish, gnomish, and orcish objects
  * Orcs hate dwarvish, gnomish, and elven objects
  * Dwarves hate orcish, gnomish, and elven objects
  * Gnomes hate dwarvish, orcish, and elven objects
  * Humans hate gnomish objects (too small) - but otherwise they can use all other racial equipment
  
The effects of wearing armor or wielding weapons you hate:
* +2AC penalty for each piece
* -5 to-hit penalty for each piece
* You receive an explicit message when wearing or wielding any hated object - this is to make the mechanic obvious.
* You'll also receive periodic messages when fighting to remind you your to-hit is suffering.
* When throwing items your race dislikes, they have a 1 in 7 chance of slipping. This is the same as a cursed or greased projectile.

This mechanic also applies to monsters, but they will also simply avoid using items they don't like.

Gnomish boots, helms, and suits were imported to help augment gnomes toughness.

## New races
### Vampires
Vampires have an interesting history in the NetHack world. They first surfaced in SLASH'EM, then in UnNetHack, then dNethack, and SpliceHack, and even Hack'EM. Each one was implemented a little differently, so we aimed to take the best of each and release a vampire that is fun but balanced. Our vampiric race starts you off strong, you won't have any cheesy poison or GWAWOD deaths, nor will you have to worry about sleeping gas traps or any of the floor traps that you can just fly over. What you *will* have to worry about is your new worst enemies: silver and hunger:

You'll also have to move quickly and attack aggressively to keep draining blood for nutrition. The corpse draining mechanic from SLASH'EM has been removed. It created quite a few bugs in the nutrition code, it resulted in tedious draining of corpses (which often are wasted anyway), and a better alternative was found in SpliceHack, which was simply doubling the nutrition from feeding on life blood during combat. The main drawback to this approach is that now vampirics cannot gain intrinsics or benefits from eating corpses. To compensate, you start off with the many intrinsics a regular vampire enjoys. 

* When attacking particularly dangerous monsters like cockatrices, medusa, or green slime, the bite attack will be prevented to avoid stupid deaths.
* Even though all vampires have drain level resistance, they are susceptible to the drain life bite attacks from other vampires.
* Vampires feed at a much higher rate when their victims are impaired by confusion, incapacitated, or trapped (Hack'EM).
* While playing as a vampire, most food rations are replaced by blood potions.
* Vampires prefer their blood to be cursed, not blessed!
* Some vampires get an opera cloak (much rarer than SLASH'EM).
* Vampires get a charisma bonus for wearing opera cloaks (UnNetHack).
* Potions of blood and vampire blood (SLASH'EM) give vampires a drinkable food source.
* Vampires can no longer shapeshift via #monster.
* Vampires now start the game with infravision.
* Silver weapons generate more often when playing as a vampire.
* Vampires cannot handle silver items or weapons. They also cannot wear silver rings or zap silver wands. When the player is ready to perform the invocation, they may apply the silver bell on the invocation square, but otherwise silver items are unusable for vampires.
* Vampires won't receive any silver artifact gifts from their gods.
* Vampires cannot handle garlic.
* Vampires can use any racial items except gnomish items (mostly because they are too small)
* Vampires can use tinning kits to bottle blood from corpses (from SlashTHEM). These tins are simply generic blood and do not convey any intrinsics.

* Vampires are Inherently Evil (from EvilHack)
    * This is adapted from the Infidel role in evil. In general, vampires suffer very little
      alignment penalties for general cruelty. They can attack and kill peaceful monsters
      with no worries, and for other actions they have lessened alignment penalties.
    * Even without conflict, you will "desire conflict" upon entering the Astral Plane.
    * Standing on Elbereth results in a -5 alignment penalty.

Vampires get these resistances and abilities:
    - Level 1:     Regeneration
    - Level 1:     Breathless
    - Level 1:     Flying
    - Level 1:     Poison resistance
    - Level 1:     Drain resistance
    - Level 1:     Immune to death magic
    - Level 5:     Hunger
    - Level 9:     Sleep resistance
    - Vampires are also immune to lycanthropy, withering, and rabid statuses.

With the vampire race available you will be able to play as a archeologist, barbarian, priest, cartomancer, rogue, or wizard. Only the chaotic alignment is available since they are inherently evil creatures.

## ITEM CHANGES

* Reduced weight of land mines to 40 aum (xnh)
* Reduced weight of beartraps to 50 aum (xnh)
* Reduced weight of bullwhips to 7 aum
* Reduced weight of flint stones to 2 aum (xnh/Spork)
* Reduced base cost of flint stones to 1.
* Reduced weight of rocks to 4 aum
* Reduced weight of pick-axe to 75 aum (SLASHEM)
* Reduced weight of most armors by 50 aum (K-Mod)
* Reduced weight of elven gear by about 1/3'rd (Evil)
* Reduced weight of morning star to 50.
* Increased weight of war hammers to 120.
* Increased weight of dwarvish and elven mithril coats to 200 aum
* Increased weight of dragon scales and scale mail to 80 aum
* Increased weight of shuriken to 2 aum each.
* Increase the prices of many magical tools
* Raised price of magic marker to 500
* Raised price of magic lamp to 500 (xnh)
* Raised price of wand of nothing to 500 (EvilHack)
* Levels of erosion on an object can affect its price (Evil).
* Port FIQHack's ring initial enchantment rules
* Port the Oily Corpses Patch (xnh)
* Rocks can be broken (a)pplied to produce flint stones (xnh). When the player breaks rocks, they enter into an occupation which continues until the rocks are used up.
* Flint stones can be struck (applied) against objects made of iron, producing sparks (fire). This can scare certain monsters away who fear fire. (Spork/THEM)
* Buff the effects of the scroll of light (xnh)
* Reverse the name of the HACKEM MUCHE scroll
* Using a cursed unlocking tool has a chance to break (Evil)
* Using eroded unlocking tools also has a chance to break.
* Credit cards may slip through a lock when cursed or hero is fumbling (xnh).
* Playing eroded musical instruments can break the instrument or fail to play.
* Applying rusty stethoscope is much less effective.
* Rusty tin openers can break.
* Amulets of magical breathing are immune to water damage
* Reduce crystal ball paralysis if player has free action (Dyna)
* Make kicking boots supersede thick_skin/clumsy (Splice)
* Mud boots provide protection from wrapping attacks
* Hiking boots let you avoid pit traps
* Hiking boots provide extra carrying capacity (dnh)
* Fencing gloves provide +2 to-hit when you are attacking with a free off-hand (dnh)
* old gloves don't take erosion damage (dnh)
* padded gloves provide an extra point of AC (dnh)
* combat boots provide 1AC and +1 to-hit (dnh)
* jungle boots provide protection from wounded legs (dnh)
* gauntlets of dexterity grant +1 to-hit while using bows (Evil)
* saddles are now twice as common (FIQ)
* mummy wrappings always generate rotted
* orcish equipment is usually generates rusty and/or corroded
* dwarven items frequently spawn as fixed. 
* The ring of levitation is a valid starting ring.
* Cursed food items will no longer tame or pacify monsters.
* Eucalyptus leaves can never be rotten unless cursed.

### Weapon changes

#### Higher max weapon enchantment
* Weapons can be enchanted much higher, with a soft limit of +11.
* This means that the new "+5" is "+11", and +13 is easily attainable by reading a blessed scroll of enchant weapon with a +11 weapon.
* To compensate, weapon enchantment gives variable to-hit bonus instead of flat bonus. This means that instead of a +7 weapon granting +7 to-hit, it grants a random to-hit bonus from 0 to +7.
* Random weapons have a small chance to generate with very high enchantment.
* Lords, princes, and uniques will also appear with much higher enchantment on their weapons.
* Beware, over-enchanted weapons that vaporize now explode.

* Any slashing or piercing weapons can now be poisoned (SLASHEM)
* All short swords get +1 to-hit (Dyna)
* Reduced probability of long swords generating (K-Mod)
* Wielded polearms grant +2AC
* **Spears** at expert skill can skewer through enemies, allowing you to hit the enemy directly behind the target. Peacefuls are prevents from being hit unless the spear is cursed. We also won't auto-skewer the spot unless it is visible. Skewering doesn't trigger most passive attacks unless it's a passive electrifying attack and you attack with a metal spear.
* **Spetums** can skewer up to 3 monsters when used in melee while riding a steed
* **Ranseurs** can disarm monsters or the player when pounded or used in melee while riding a steed.
* **Bardiches (long poleaxes)** have a 1 in 100 chance of beheading monsters (or the player)
* +4 to-hit bonus for attacking with a scimitar on a steed.
* Wielding and unwielding **curved swords** takes 0 turns.
* **Morning stars and flails** can stun monsters (or the player) on critical hits. Player must be skilled or better.
* Special weapon effects (like rogue backstab, flail stunning, and samurai katana weapon smashing) have been enabled when two-weaponing.
* **Crossbows** no longer grant multishot, instead their damage output is multiplied by your skill (dnh)
* No multishot when **fumbling**
* 
#### Slings
* Projectiles receive a powerful strength bonus when using slings (xnh)
* Gem class projectiles do minimal damage vs thick-skinned monsters
* Launching gem class projectiles from slings has the potential to instakill H
  
### Magic markers
* Appear randomly much less often (1/5'th of the frequency in Vanilla)
* They can still be creating from polypiling

### Wands of wishing
* **Always generate pre-charged**, meaning they can never be re-charged, otherwise they will explode (many variants incorporate this)
* Wands of wishing only generate with d2 charges
* The maximum possible wishes from any WoW is 3 wishes

### Unicorn horns

* Success depends on their enchantment level (SLASHEM)
* Now one-handed, dealing d6 vs small/d7 vs large
* Having skill in unicorn horn has a positive impact on your success when applying, having no skill has a negative impact.
* Basic skill grants a 10% bonus to success, skilled 20%s, and expert 40%. This allows roles that can attain proficiency to not have to enchant it so high.

* Successfully applying a unihorn also exercises your skill in it by 5 points. 
* The healer gets a bonus when applying unicorn horns. Instead of the standard 30% success rate when the unihorn is +0, they have a 40% success rate.
* Cancelled unicorn horns become degraded, unusable for curing.
* Unicorn horn drops decrease as the number of unicorns killed increased.
* Adapted unicorn horn enchantment to higher weapon max enchants.

### War Hammer
* war hammers have been changed from a one-handed weapon into a competitive two-handed weapon (xnh)
* They now deal 2d6 vs small monsters and 2d8 vs large

### SCROLLS

* Scrolls of genocide only clear a single monster species on the level (uncursed) or globally (blessed) (Un)
* Endgame genocide nerf. Monsters cannot be fully genocided after entering the planes. Any genocides executed in the end game will be uncursed and only have a 1 in 4 chance of destroying each monster of that species. This is a soft counter to the plane of water genocide strategy that most players employ. Players can still genocide ; before entering the planes, but beware, there might be more dangerous replacements waiting for them.
* Enchant armor: Ability to choose worn piece of armor to enchant/repair (Evil)
* Give enchanting vibrate warning for all weapons/armor (Dyna)
* Blessed scroll of destroy armor asks which armor to destroy (xnh)
* Confused cursed scroll of destroy armor prompts for armor to fix
* Confused scroll of identify gives enlightenment (xnh)
  
### POTIONS

* Dipping an eroded item in restore ability repairs the erosion (xnh)
* Acid potions are immune to being destroyed by freezing (xnh)
* Implement behavior for cursed potion of gain ability (xnh)
* More potion breathing effects (xnh)
* Thrown potions of hallucination confuse monsters (Evil)
* Potion of paralysis lasts 3-24 turns on monsters (Evil)
* Withering can be cured by quaffing holy water.
* Blessed restore ability only restores a few levels (Evil).

### WANDS

* Raise odds of a cursed wand exploding to 1 in 30 (Un)
* Cursed wand backfire patch (Evil)
  * If a directional wand is cursed and the player zaps it, there's a 1 in 8 chance it will backfire, hitting the player instead.
* Blessed and uncursed wands wrest much more often
  * blessed wands wrest 1/7 of the time
  * uncursed wrest 1/23 of the time
  * cursed wands still wrest 1/121 of the time
* Wand of cancellation extensions
  * Monsters can zap the player with wands of cancellation
  * Being cancelled removes the protection spell effects
  * Small chance dragon scale mail will revert back to a set of scales if cancelled (Un/Evil)
* Increase wand to-hit chance for high-dex characters  (Splice)
* Wands of secret door detection can be broken to detect traps.
* Wand explosions discharge their effects in an explosion (SLASH'EM).
* Wands generate with 4 more charges than they normally get in Vanilla (SLASH'EM).
* Monsters zapping cursed wands have double the chance of explosions.

## SHOP CHANGES
**Lighting shops:**
* Magic lamps are one notch rarer - down to 11.3% per game now overall (Spork)
* Potions of oil have been eliminated from appearing.
* Non-candle and non-lamp items have had their probabilities minimized.

## NEW ITEMS

**stomping boots:**
* Instakills any tiny monster you attack or run into (Splice)
* Small monsters can also get stomped with a 1 in 40 chance.
* Flying monsters, monsters in water, amorphous, and incorporeal monsters are immune to stomping.

**flying boots:** Levitation boots have been removed and replaced with flying boots which simply grant flight. Medusa's Island gets flying boots instead of levitation boots.

**gauntlets of force:** Increase strength bonus, makes forcing locks and opening doors take 1 turn. Chance of stunning. Can break iron bars, boulders.

**anti-magic shield:** Leather shield that provides magic resistance.

**gnomish boots:** Provides 0AC + bonus 2AC for gnomes (THEM)

**gnomish helm:** Provides 0AC + bonus 2AC for gnomes (THEM)

**gnomish suit:** Provides 1AC + bonus 2AC for gnomes (THEM)

**orcish boots:** Provides 1AC + bonus 2AC for orcs (Evil)

**wand of corrosion:** shoots acid rays (Splice)

**wand of poison gas:** shoots poison rays (Splice)

**wand of wonder:** shoots a random ray by picking a random wand on each activation (Splice)

**scroll of cloning:**
    * From SpliceHack
    * $300
      Cloning these objects has nerfed results (obviously for abuse or balance considerations):
    * magic marker -> athame
    * magic lamp -> oil lamp
    * wand of wishing -> wand of wonder
    * bell of opening -> bell
    * candelabrum of invocation -> wax candle
    * amulet of yendor -> cheap plastic imitation amulet
    * book of the dead -> blank spellbook
    * scroll of cloning -> blank scroll (prevents infinite cloning loops)
    * artifacts all copy the base item, but lose the name and the status of being an artifact.
    
    To copy the enchantment on an item, the scroll must be blessed.
    If the scroll is cursed, the resulting item will be cursed.
    
    All other properties on the item should be copied exactly as is. This enables fun tricks like cloning that +13 fixed crysknife, or that blessed figurine of an Archon you've been holding onto.
    
    When confused, the scroll clones the player. The resulting clone will have no inventory. A blessed scroll creates a tame clone, an uncursed scroll makes a peaceful clone, and a cursed scroll makes a hostile clone. An interesting side-effect of this is that cloning yourself reduces your current HP by half.
    
    Couple updates:
    * Unpaid items cloned in shops become property of the shopkeeper.
    * More item properties are carried over: erosionproofing, container status, and some other misc things to make sure items are truly cloned.
    * Intelligent monsters can use these scrolls to clone themselves!  I think this sort of balances out the scroll a bit, since a good number will be used up by monsters. When monsters read them, they always act as confused - so they can only clone themselves. It's a bit weird, but it's much easier than allowing them to clone items and needing to create a system for that mess...
    * Unique monsters can also use these scrolls... The Wizard of Yendor still has to go through the Double Trouble routine, so no more than 2 Rodneys will ever oppose you. But it's possible for other uniques to clone themselves more than once if the opportunity arises.

**scroll of knowledge:**
    * From SpliceHack
    * $50
    * Read to learn about a random magic item.
    * If blessed, there is a chance (based on luck) to learn about an additional item.
    * Archeologists get to specify a specific item to learn about in addition to the regular effects.
    * Unlike SpliceHack, this scroll can be written.
    
**scroll of water:**
    * From UnNetHack/xNetHack
    * $200
    * When read, this generates many water pools around the player.
    * If not blessed, there is a chance of creating water underneath the player.
    * If cursed, a pool is certainly created under the player. If uncursed, the chance is luck based (higher equals less chance).
    * When confused, this can dry up surrounding water tiles.

**rapier:** (SLASHEM)
* A sword using saber skill that deals d6 vs small, d8 vs large
* Made of unerodable metal, weighs only 15
* Base item for Mouser's Scalpel.

**scythe:**  (Splice)
* Classified as a polearm, but can also be used in melee.
* Damage vs. small: 1d8+1d4
* Damage vs. large: 1d10+1d4
* Base item for The End

**heavy sword:**
* Base item for Load Brand 
* Basically the same stats as a two-handed sword but it is made of mineral and weighs 500aum

**silver short sword** (SLASHEM).

**sling bullet** (EvilHack)

**potion of blood:**
* Decent food for vampires
* The nutrition granted has been raised from other variants, and grants 400 nutrition.

**potion of vampire blood:**
* Fantastic meal for vampires
* If drunk as a non-vampire, this polymorphs you into a vampire.

**playing card deck:**
* When applied, gives you a poker hand which correlates to your luck.
* If the deck is blessed (or you are a cartomancer), you get a clear indication of your luck
  by using the kicker.
* If uncursed, you get a rough indication of your luck by the hand strength.
* If cursed, the meanings are reversed.

**deck of fate:**
Grants random effects when you draw a card from it. When you apply it, you are prompted for
how many cards to draw. You can draw a max of 5 cards.

Card effects:
* The Tower - Magical and fiery explosions on self.
* The Wheel of Fortune - Draw two more cards.
* The Devil - Summons a demon.
* The Fool - Abuses int and wis.
* Death - You are subjected to the touch of death. If you are invulnerable, hallucinating,
  or a form that resists death, you are spared. If you have magic resistance, you still are
  subject to 8d6 drain life damage. If you have not used saving grace yet in your current
  game and you have positive luck, your life can also be saved that way.
* Judgment - You are punished.
* The Emperor - Curses two items.
* The Hermit - Get intrinsic teleportitis and invisibility for a brief period.
* The Hanged Man - Summons a rope golem.
* Justice - If you have negative alignment, you are paralyzed for 20-49 turns, otherwise you are
  unpunished.
* Temperance - Destroy two worn pieces of armor
* The Lovers - Summons a random foocubus.
* The Magician - If the Wizard of Yendor has been killed, he is resurrected - otherwise this
  increases your maximum power and refills it.
* Strength - Increases your strength.
* The High Priestess - Clears previous alignment abuse and you gain alignment.
* The Hierophant - Creates an altar, if the floor under you isn't already a dungeon feature.
* The Empress - Creates a throne, if the floor under you isn't already a dungeon feature.
* The Chariot - You get teleport control for 1 turn and a level teleport.
* The Sun - Gain (additional) intrinsic protection and divine protection.
* The Moon - Gain 7 luck.
* The Star - Identifies your inventory.
* The World - Prompts you to make a wish.


## NEW ARTIFACTS

| Name                | Align     | Type                  | From       | Notes                                                                                                                                                                               |
| ------------------- | --------- | --------------------- | ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Disrupter           | neutral   | mace                  | SLASHEM    | deals 1d30 damage and +d5 to-hit vs undead</br>grants warning vs undead                                                                                                             |
| Keolewa             | neutral   | club                  | EvilHack   | deals 1d8 shock damage, +d5 to-hit</br>grants shock resistance while wielded                                                                                                        |
| The End             | neutral   | scythe                | SpliceHack | deals 1d20 cold damage, +d3 to-hit</br>grants drain resistance while wielded                                                                                                        |
| Serpent's Tongue    | chaotic   | dagger                | SLASHEM    | deals double damage to all monsters<br/>bonus damage vs monsters that don't resist poison                                                                                           |
| Doomblade           | chaotic   | short sword           | SLASHEM    | deals 1d20 damage<br/>25% chance of (1d4 * 5) bonus damage                                                                                                                          |
| Poseidon's trident  | chaotic   | trident               | SpliceHack | deals +d7 damage, +d3 to-hit</br>grants magical breathing while wielded<br/>#invoke for water walking and an earthquake                                                             |
| Origin              | unaligned | quarterstaff          | SpliceHack | deals +d6 damage, +d2 to-hit</br>grants teleport control while wielded<br/>grants spellcasting bonuses while wielded                                                                |
| Hellfire            | chaotic   | crossbow              | SLASHEM    | bolts fired from Hellfire deal +d7 damage and explode in fire<br/>grants fire resistance while wielded                                                                              |
| Plague              | chaotic   | bow                   | SLASHEM    | arrows fired from Plague are auto-poisoned and deal +d7 damage<br/>grants sickness resistance while wielded                                                                         |
| Pridwen             | lawful    | large shield          | SpliceHack | grants 1/2 physical damage while wielded</br>grants steadfastness while wielded                                                                                                     |
| Quick Blade         | lawful    | elven short sword     | SLASHEM    | +d9 to-hit, +d2 damage                                                                                                                                                              |
| Carnwennan          | lawful    | knife                 | SpliceHack | deals +d8 damage<br/>+d3 to-hit<br/>grants stealth and searching while wielded                                                                                                      |
| Load Brand          | unaligned | heavy sword           | NerfHack   | weights 500aum<br/>deals +d40 damage<br/>Confers steadfastness and MC1 protection<br/>Confers 1/2 physical damage<br/>Absorbs curses like Magicbane                                 |
| Snakeskin           | Neutral   | robe                  | SlashTHEM  | Confers acid resistance<br/>Confers hallucination resistance                                                                                                                        |
| Blackshroud         | neutral   | cloak of invisibility | SlashTHEM  | Grants warning and drain resistance                                                                                                                                                 |
| Mirrorbright        | neutral   | shield of reflection  | SLASHEM    | Doesn't inhibit spellcasting<br/>Confers hallucination resistance                                                                                                                   |
| Deluder             | neutral   | cloak of displacement | SLASHEM    | Confers stealth and MC1 protection                                                                                                                                                  |
| Whisperfeet         | neutral   | speed boots           | SLASHEM    | Confers stealth and luck                                                                                                                                                            |
| Mayhem              | chaotic   | stomping boots        | NerfHack   | Confers conflict and warning vs undead                                                                                                                                              |
| The Lenses of Truth | unaligned | lenses                | NerfHack   | Confers see invisible, searching, and stun resistance when worn                                                                                                                     |
| Serenity            | lawful    | silver spear          | NerfHack   | +d5 to-hit, +d10 damage<br/>Blocks aggravate monster if present<br/>Prevents monsters from berserking<br/>Counters 80% of hostile monster spells<br/>Absorbs curses like Magicbane |
| Mouser's Scalpel    | neutral   | rapier                | slashem-up | +d5 to-hit, +1 damage<br/>Capable of multiple bonus hits with no limit                                                                                                              |
| Amulet of Storms    | chaotic   | amulet of flying      | xnh        | Confers shock resistance, can #chat to tame stormy monsters.                                                                                                                        |

Misc changes:
* Plague was changed from an orcish bow to a standard bow.
* Quick blade is a silver short sword instead of an elvish short sword

## ARTIFACT CHANGES

- Artifact weapons can now be dual-wielded (SLASHEM)
- Lawful and chaotic weapons cannot be two-weaponed (Evil)
* The Tsurugi of Muramasa has a 10% chance of bisection (SLASHEM)
* Magicbane is a quarterstaff (FIQ)
* Creating Excalibur will fix any negative enchantment on it (xnh)
* Fire Brand instakills highly flammable monsters and green slimes (xnh)
* Attacking with Fire Brand cures sliming
* Frost Brand instakills water elementals
* Vorpal blade grants see invisible while wielded
* Vorpal Blade provides warning vs jabberwocks (Evil)
* Vorpal blade gets a 10% chance of beheading (SLASHEM)
* The Heart of Ahriman now grants slotless flying and displacement instead of stealth (FIQ)
* The Orb of Detection grants clairvoyance while carried.
* Trollsbane grants regeneration while wielded (many variants)
* The Eyes of the Overworld protect against more gaze attacks (Evil)
* Prevent Cleaver from cleaving peaceful bystanders (xnh)
* Giantslayer is now a spear (Evil)
* Giantslayer conveys 18/\* strength while wielded (Dyna)
* Ogresmasher can also hurtle light-weight monsters (Evil)
* Werebane provides protection from shapechangers when wielded
* The Sceptre of Might gets a flat +10 damage buff and grants steadfastness when wielded.
* The Longbow of Diana confers half physical damage when wielded
* Increased Mjollnir's wakeup radius when it strikes monsters with lightning
* Mjollnir can be invoked for a lightning bolt (xnh)
* Sting actually cuts through webs when force-fighting
* Snickersnee grants stun resistance when wielded (Evil).
* Withering can be cured by the Staff of Aesculapius (xnh/Evil)

**Bane changes:**
* All banes provide warning vs their bane monster type when wielded (Evil)
* All banes glow red in response to their monster types (Evil)
* All banes can instakill their associated monster types with a 1 in 5 chance (Un)
* Sunsword and Disrupter don't get instakills. 
* Banes can't instakill unique monsters

## DUNGEON CHANGES

* The Rogue level has been disabled (many variants)
* Chickatrices and cockatrice eggs will now appear in cockatrice nests (xnh)
* Shops cannot have themed rooms with unusual floor textures (xnh)
* No special **themed rooms** generate until level 5
* Random rivers were added to many of the quest filler levels.
* Trees can generate in dungeon rooms (xnh)

### Castle changes

* The castle level is now marked as a graveyard
* Castle barracks may open into courtyard instead of throne room, letting soldiers flood the courtyard more quickly (xnh)
* Added iron bars to the castle perimeter
* Iron bars have been added to the castle towers (Spork)
* The location of the chest containing the wand of wishing has been obfuscated. You will find matching chests and scrolls in each of the towers if you use object detection. The other chests have wands of nothing inside. (Spork)
* The drawbridge passtune range has been expanded by one square. (xnh)
* The drawbridge also does not always close with the passtune, one out of five times it will malfunction when trying to close it. (xnh)
* Castle courtyards are unlit.

### Valley of the Dead

* Players can't regenerate hit points while in the Valley of the Dead (Evil)
* Instead of dart traps, the player will encounter magic traps (Evil)
* Less ghosts are guaranteed in the valley

### Shortened Gehennom

* Gehennom has been dramatically shortened to 5-7 levels.
* All the demon lairs have been removed.
* The fake wizard levels have been removed.
* The wizard's tower levels have been moved out of Gehennom and extracted to their own branch (xNetHack/EvilHack)
* The portal to the wizard's tower has been moved to a random castle tower and changed to a stair up.
* Some of the maze levels in gehennom have been trimmed out, most of the level generation is cave-like.
* All hell fill levels are either hot or cold.
* Disabled the ice/water levels in Gehennom.

### Sokoban

* Sokoban levels are cold and icy - legend has it a white dragon took the tower over, leaving a trail of frost in its wake. In addition to the level being colored blue with splashes of icey cyan, you will see random patches of ice form in the level. The upper levels of Sokoban are also "cold", meaning that if potions land on the floor, they have a chance of freezing and shattering.
* Note: A recent change from NetHack 3.7 also makes ice slide the player in a random, however, players will not slide while in Sokobon (this would make solving the puzzles more difficult than it already is).
  direction. This feature was implemented after cold Sokobon, but it amplifies the effect.
* Monsters are never generated peaceful in Sokoban (FIQ)
* Zombies don't revive in Sokoban and they won't dig out of the ground.
* Monsters won't break boulders in Sokobon.
* Cursed gain level can be used in Sokoban to bypass a floor (xnh)

* All the vanilla sokoban levels have been replaced with the SLASH'EM puzzles.
* The Dragon of Bactria level was added from NetHack Fourk; the green dragon was replaced with a weaker white dragon and actually all Soko zoos have the white dragon guarding the treasure.
* The zoos in Soko have been expanded slightly.
* In addition to the amulet and bag, the Sokoban prize can also be a cloak of magic resistance or a magic marker.
* Stop Sokoban guilt after acquiring the prize.

### Fort Ludios
* Ported two Fort Ludios variants (Evil/Un)
* Some mermaids were added to patrol the moats.

### Minetown/Mines End
* Ported zoo town and lavender town (Splice)
* Ported Creek Town and Mini-Castle town (THEM)
* Imported the Gnomish Sewer (xnh)
* Imported 3 mines end variants (THEM)

### Oracle
* Ported Oracle variations 2 and 3 (Splice)

### Temple to Moloch level
* Ported from SLASH'EM
* Gargoyles replace the statue gargoyles in the original map.
* 2 ghoul mages were added.

### Lost Tomb level
* Ported from SLASH'EM

### Big Room
* Ported bigroom variants from UnNetHack and SpliceHack.
* Imported two bigroom variants from xnh.

### Forges

* Forges were ported in from EvilHack
* Forges let the player repair metallic armor, bless items, dispose of zombies or organic items, dispose of the iron ball and chain, and summon lava demons and fire elementals.
* Forging recipes are available in the object lookup
* Weapons can be forged by applying a hammer while standing on a forge.
* Items can pass over forges.
* New forging feature: There is a one-time 1 in 30 chance of erodeproofing an item when dipping in a forge. After this occurs, the forge will instead emit a puff of steam.
* Cold rays can cool forges.

### Toilets

Toilets have received many enhancements after adapting them from SLASHEM. Notably, toilets can now appear on their own, separate from sinks, whereas in SLASH'EM, they only came in pairs with sinks. Overall, their frequency has been dialed way back so they are quite rare.

* Toilet prayer can now stop the vomiting process
* Praying at toilets can cure sickness.
* Sitting on toilets can alleviate satiated status.
* If giants sit on toilets, they break.

Toilet kicking:
* Like sinks, toilets now have a couple different effects from kicking them, including a few YAFM.
* Kicking now only breaks the toilet 1/7 chance (was 1/4 in SLASH'EM)
* Kicking can generate giant cockroaches and pools from kicking (1 in 17 chance)
* Kicking can generate brown puddings (only once per toilet)
* Kicking can generate a random tool. Normally this tool will weigh under 15aum, but sometimes you'll get a large tool that bonks against the piping. If a large tool bonks 3x - you'll get that tool no matter now big it is and the toilet is destroyed in the process.

Dipping an edged weapon into a toilet can poison it, but also probably rust any metallic items.

### Bloody tiles
* Ported from SpliceHack
* When a monster is killed, it can spray blood around the surrounding tiles depending on it's size.
* The blood is mostly cosmetic, however, players cannot engrave in the dust while blood covers that tile.
* Blood can be wiped off with a towel, or will wear off after enough activity.

### Traps

* At higher levels, boulders can drop from falling rock traps.
* Falling rock traps can result in stunning with sufficient damage.
* Polytraps disappear with 1 in 7 chance when a monsters steps on one.

A few new traps have been added:

#### Spear traps
* Ported from EvilHack
* Spear traps only start appearing after level 5
* Spear traps can be untrapped, potentially yielding a random spear type in the process.
* Flying and levitation usually protect from being harmed by spear traps, however, there is still a 25% chance of being hit (by a abnormally long spear)
* If you or a monster hit by the trap is thick skinned, the spear just breaks and the trap is deleted.
* The trap also doesn't affect unsolid monsters.
* When hit, it deals 7-14 damage and wounds your legs for 10-19 turns.

#### Magic beam traps
* Ported from EvilHack
* Magic beam traps only start appearing after level 10
* When you (or a monster) steps on this trap, it shoots a random ray type from a pre-set location that crosses through the beam trap. The beam type is set for each trap, so once you notice it shoots fire rays, it will always shoot fire rays.
* The trap graciously never will shoot disintegration or death rays but all the other ray types are possible.

#### Grease traps
* New creation debuting in NerfHack
* Grease traps function similarly to rust traps, but they spray a blast of grease at the player or monster that stepped on it.
* When you step on a grease trap, you either slip in a puddle of grease or get sprayed by a grease hose.

Puddle of grease:
  * If you don't have levitation or flying, you gain fumbling ("You step in a puddle of grease.")
  * Slipping in grease traps can cause you or monsters to become paralyzed for a few turns and inflicts a small amount of damage.
  * Mud boots and water walking boots protect from slipping on grease traps.

Grease hose:
  * If the grease hits your head, you are blinded unless you are wearing a visored helmet. Your blindfold/lenses/etc may also become greased and fall off.
  * If the grease hits your arm, your weapon(s) or shield can become greased and fall off. You also gain the Glib condition for 10 to 15 turns.
  * If the grease hits your feet, your boots can become greased and fall off.
  * Otherwise, the grease hits your torso and your outermost armor becomes greased. Random items you are carrying can also become greased and fall from your possession. If you are carrying a towel, there is a 50% chance it becomes greased as well. If you are riding a steed the saddle will get hit with grease, making you fall off.
* When a monster gets hit with grease, it will randomly grease an item in their inventory.
* The trap disarms with a random 1 in 15 chance.



#### Door traps
* Door traps actually explode in a ball of flame (Evil)
* These traps will start appearing at level 8.

#### Booby-trapped tins
* From xNetHack
* Randomly generated tins have a 1 in 30 chance of exploding in a blast of fire when opened.
* Tins that you create from tinning kits will always be safe.

## Special Rooms

### Art rooms

* Ported from SpliceHack
* These rooms have a one-time event that occurs upon entering a room
* Most of the time it's a fun piece of art depicting something with the denizens of the dungeon. But sometimes it's a special effect.
  * You might see an image of your god, invoking enlightenment
  * You might find a partial map of the level
  * You might encounter a scary image, stunning you for a few turns
* Art rooms help exercise INT and WIS, depending on the room
* To get any effects, you must not be blind when you enter the room

### Room colors patch
* Most special rooms get a distinctive color or combination of colors.

### New room: dragon lair (from SLASH'EM). 
* Dragon scales can sometimes appear in dragon lairs.
* Dragon lairs now produce special sounds when they appear on levels.

### New room: giant courtroom (from SLASH'EM). 
* Giant courts sometimes have tinning kits.
* Monsters in giant courts are always hostile.

### New room: Real zoo (from SLASH'EM).
* Monsters in real zoos are always hostile.

## CREDITS
NerfHack draws inspiration and ideas from many variants of NetHack:
* AceHack
* DynaHack
* EvilHack
* FIQHack
* FourkHack
* GnollHack
* GruntHack
* K-Mod
* SLASH'EM
* SlashTHEM
* slashem-up
* SLASHEM9
* SpliceHack
* SporkHack
* UnNetHack
* xNetHack

Many thanks to all the folks who have helped out with the original Hack'EM and NerfHack, contributing ideas, making patches, playtesting, or anything!

### Special thanks to:
- My wife - for being endlessly patient with this time-consuming endeavor!
- K2, for making the epic EvilHack, all his help during development, and pushing NerfHack (and previously HackEM) up to hardfought.
- amateurhour and qt for their endless debugging advice.
- cbus for many contributions
- mobileuser and hothraxxa for extensively playtesting the original HackEM
- malor for continuing maintenance of HackEM

### Thanks:
- amateurhour
- antigulp
- aosdict
- arahael
- Ardub23
- bhaak
- bouquet
- cbus
- Chris_ANG
- disperse
- Frozty
- hothraxxa
- Janis
- K2
- krm26
- Loggers_VIII
- malor
- mobileuser
- Nat Hall
- NetSysFire
- nh2465
- NoisyToot
- notifico
- oh6
- paxxed
- qt
- riker
- shadowrider38
- stenno
- terrapin
- transcendreamer
- Umbire
- VaderFLAG
- YesLaching
