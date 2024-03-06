# NerfHack

NerfHack is intended to be a more difficult variant than Vanilla NetHack. By pulling changes from many variants and fine-tuning various exploitable aspects of the game, we have uncovered many pain-points that increase the difficulty. The general idea has been to quell numerous strategies commonly employed by seasoned players with the goal of making the game more interesting, fostering more creative use of items and resources.

## General guidelines:
1) Introduce new threats
2) Create resource scarcity for the player
3) Nullify many tried-and-true exploits
4) Introduce quality-of-life features
5) Make it easy to variant-hop
* The player should be able to easily transition from Vanilla NetHack to NerfHack. We hope players don't have to think too much about the changes. Most of the mechanics are designed to be understood intuitively based on game feedback.
* Don't require the player to memorize or lookup large tables of information (ex: forging recipes, tinker mechanics, object materials, object properties, gem alchemy, potion fermentation, etc, etc)
* Don't change anything major in the interface or functionality. 
* Don't introduce any new #extended commands (other than wiz-mode tools)
* Don't change any monster letters

There are definitely some changes that the player should know about, however, we will leave it up to the individual to decide what those are. The thrill of discovery should not be spoiled.


**Some coding principles:**
* When possible, put all changes for a mechanic into a single commit (avoid part 1, part 2, etc)
* No changelog will be kept in the repo. A changelog creates duplication of information and makes maintenance of the project more tedious. This README may act as a detailed summary in place of changelog updates that is updated with each minor version.
* Stay current with the main branch of NetHack.

## Big changes from NetHack 3.6/3.7

* Removed the **mysterious force** from the game (xnh).
* To bring back the feeling of the 3.4.3 **stealth** mechanic, the chance of sleeping monsters waking up and growling has been lowered dramatically and is based on luck.
  * 0 Luck: 12.5% chance of a monster screaming when roused.
  * 2+ Luck: 0.3% chance
  * Negative luck has at least a 30% chance of rousing monsters.
* Reverted the majority of **level flips** from 3.7. Flipped levels only appear in Sokoban and the big room special level.
* **Items that are 'lost'** from the players inventory will no longer be un-identified. 
* Disabled **#chronicle** from auto-completing (so #chat will autocomplete as normal)
* Enabled autocomplete for #twoweapon
* Disabled **farlook help**
* Disabled the 3.7 **tutorial**
* Enable **full options** by default.
* Changed the symbol for **sinks** back to #
* **Fog clouds** don't leave traces of steam (so they show up as v)
* **Hezrou and steam vortices** don't leave clouds unless they moved. This guarantees that they won't obscure their own visibility with self-generated clouds.
* **Stinking clouds** no longer block line of sight
* **Disabled vampire shapeshifting** for all vampires except Vlad; this includes vampshifting or the player polymorphed into a vampire as well.
* Rogue's can inflict **backstab damage** for the first thrown weapon. In 3.4.3 this was a very powerful mechanic that was nerfed in 3.6. We are bringing it back in a limited form as a callback to 3.4.3 but also because it strongly fits the theme of the role.
* No special **themed rooms** generate until level 5
* **Branchport** always brings you to the entry level of a branch
* Shops cannot have themed rooms with unusual floor textures (xnh)
* **Sting** actually cuts through webs when force-fighting
* Dragons, nagas, and golems don't balk at approaching as much.
* Partially revert 5c7c9d10a - Rejigger anti-magic traps.

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
* Pets never displace player from stairs when entering a level (from DynaHack).
* Lessen confusing messages for confuse monster effects wearing off.
  
### Safer bags of holding:
* Players cannot put known wands of cancellation or magical bags into identified bags of holding. Keep in mind, unknown wands and bags are still dangerous and should be handled with care until formally identified (dnh)
* Players are prevented from tipping known explosive items into identified bags of holding
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
* Auto-ID amethyst, fruit juice, and booze when dipping amethyst into booze (Fourk)
* Auto-ID some potions when inhaling their vapors (xnh)
* Auto-ID scroll of scare monster if it crumbles from picking up (Un)
* Auto-ID scrolls of confuse monster when read
* Auto-ID rings dropped into a sink (Un)
* Auto-ID ring of regeneration if it heals you (Un)
* Auto-ID wand of cancellation after destroying a bag of holding (Un)
* Auto-ID wands when engraving (xnh)
* Use the process of elimination for auto-identifying wands when available (Un)
* Auto-ID loadstones when attempting to drop or stash them (Un)
* Auto-id flint yielded from applying rocks to eachother
* Auto-ID tin whistles, tooled horns, magic flutes, and magic harps upon use (Un)
* Auto-ID magic lamps and oil lamps when rubbing (Un)
* Auto-ID dunce cap when it's first put on (Un)
* Auto-ID jumping boots upon wearing (Un/Ace)
* Auto-ID water walking boots when they waterwalk (xnh)
* Auto-ID BUC of products from BUC identified tinning kit or horn of plenty (from UnNetHack++)
* Auto-ID BUC of wands when they backfire
* Blessed stethoscopes can identify eggs (from EvilHack/SporkHack)
* Make rustproof/erodeproof/fixed known by default (from DynaHack)

### INTERFACE CHANGES 

* Peaceful monsters are underlined (TTY and curses) (xnh)
* Magic cancellation (MC) value is shown on the bottom line (Evil)
* Skill caps and percentage towards next level is available in #enhance
* Show available skill slots in #enhance menu (from DynaHack)
* Add inventory weight/carrycap and n/52 items display
* /> or < can be used to autotravel to stairs (autostairtravel option)
* New config option to show damage and flanking bonuses (showdmg option)
* Show weights of objects in inventory (invweight option)
* Display AC values for armor in the inventory (Splice)
* Pets' items can be managed with #loot
* Prayer statistics (like when you last prayed, reconciled with your god, or received a gift) can be viewed in the attributes menu (via Ctrl-X)
* All position prompts may be aborted
* Show warning level 0 for very weak monsters (Dyna).
* We are able to see when a monster is sleeping, fleeing, withering, or berserking from farlook information (Evil/Splice/xnh)
* We are able to see what weapon a monster is wielding from farlook (Evil)
* We are able to see roughly how much armor a monster is wearing on farlook (Evil)
* More descriptive combat messages have been added to enhance hits and misses (xnh)
* The SLASH'EM style message is used for getting zapped by cancellation
* Show messages for objects that are randomly cursed (Dyna).
* Print an explicit message when summon nasties occurs as part of wizard harassment.
* Special room and special level walls can have their own unique coloring. For example, cockatrice nests and bee hives are yellow, and Sokoban walls are blue. (Splice/xnh)

### WIZMODE FEATURES

* The #wizcrown command has been added for testing crowning (Evil)
* The #wizclear (^z) command, clears all monsters on the screen (from SpliceHack)
* Wizard mode can override an artifact ignoring you (xnh)
* Allow teleportation into unteleportable spots in wizard mode
* Allow wishing (^W) for monsters in wizmode (Un)

## RESOURCE CONTROL AND INTRINSIC NERFS
   
* Conflict negates Elbereth and scare monster protection (Evil)
* Magic resistance and spell damage reduction only halve magic missile damage instead of preventing it (Evil)
* The chance of gaining levels from wraiths has been throttled. The chance scales with your level. You have an (XP level) in 40 chance of gaining a level from eating a wraith corpse now.
* Bones file trimming. When bones files are left, there's a high chance of items being polymorphed or shuddering away. This nerfs the common strategy of dumplog peeking.
* Amnesia can make you forget intrinsic telepathy.
* Invisibility and see invisible cannot be permanently gained intrinsically (xnh)
* Telepathy cannot be permanently gained intrinsically
* Teleportitis cannot be permanently gained intrinsically
* Strength gain nerfs: giant corpses have less of a chance of conferring strength gain (from 50% to 25%) (SLASHEM)
* HP gains from healing potions are subject to nurse dancing limits, but the limit is always observed as if the players level is maxed out at 30.
* Falling downstairs does more damage - 2d3 instead of 1d3. (K-Mod)
* Half-physical damage and half-spell damage have been adjusted to only provide quarter (1/4) damage reduction.
* Don't allow stunned jumping; and confused jumping has a 20% chance to fail (Evil)

### Slow Luck timeouts (modified)

In NerfHack, Luck items greatly slow down Luck timeout rather than stopping it completely - this is similar to how it works in UnNetHack. However, the timeouts have been modified and extended to cover negative base luck situations. The timeouts have also been reduced heavily from the UnNetHack calculations.

The modified Luck timeout depends on how far your Luck is from your base Luck: the higher or lower your Luck, the less the timeout is slowed. The timeout is calculated every turn, meaning gaining or losing a point of Luck could result in that point timing out immediately.

The modified Luck timeout is calculated by the following formula:

    Timeout = 25 * (20 - base_distance) * (20 - base_distance)

base_distance is how far you are from your base luck. If your base luck is 0 and you have 3 Luck, the base_distance is 3. If you have -10 base luck and 10 Luck, the base_distance is 20. The following chart shows how many turns it takes to timeout from one luck level to the next and the total turns to reach the base distance of 0.

| base distance  | Timeout | Time to base Luck |
|----------------|---------|-------------------|
| 0              | ∞       |      0            |
| 1              | 9 025   |  9 025            |
| 2              | 8 100   | 17 125            |
| 3              | 7 225   | 24 350            |
| 4              | 6 400   | 30 750            |
| 5              | 5 625   | 36 375            |
| 6              | 4 900   | 41 275            |
| 7              | 4 225   | 45 500            |
| 8              | 3 600   | 49 100            |
| 9              | 3 025   | 52 125            |
| 10             | 2 500   | 54 625            |
| 11             | 2 025   | 56 650            |
| 12             | 1 600   | 58 250            |
| 13             | 1 225   | 59 475            |
| 14             |   900   | 60 375            |
| 15             |   625   | 61 000            |
| 16             |   400   | 61 400            |
| 17             |   225   | 61 625            |
| 18             |   100   | 61 725            |
| 19             |    25   | 61 750            |
| 20             |     0   | 61 750            |

### ENDGAME CHANGES

* Occasional earthquakes can occur during the ascension run (Un/Evil)
* After the invocation, the maximum difficulty limit for generating monsters is removed (xnh)
* The identity of the Riders hidden via farlook (Un)
* The correct temple on the Astral Plane will not be revealed due to fleeing monsters (Un)
* "Purple/Astral Rain" nerf: Taming is more difficult on the Astral Plane; attempts to tame monsters only have a 1 in 4 chance of succeeding.
* Replace undead on Astral Plane with random A (xnh).
* Post wizard death harassment has been increased by 20-25%
* While the player is carrying the Amulet of Yendor, monsters flood from the upstairs (Un/Evil)
* Demon lords and princes can be summoned (as part of the Wizard's harassment) when you possess the Amulet of Yendor.

### FINITE ALTAR NERFS

* Altars only start appearing after level 4
* When donating to priests - the gold vanishes upon receipt
* Protection that can be bought from priests or granted by your god only ever grants 1AC per granting; the more protection the player has, the less likely it is to be granted. (K-Mod)
* Greater chance of hostile minions appearing when converting an altar. Especially if the altar is in an occupied temple. (Evil)
* Removed the "temple of the gods" theme room. This themed room contains 3 altars, one of each alignment. It was removed to make the finite altars mechanic more relevant.

#### Altar cracking

* Once the player has received two gifts or has been crowned, altars have a 50% chance to crack with each subsequent gift.
* There are two stages to the cracking. In the first stage the altar becomes partially cracked, which is purely cosmetic and doesn't affect the altar's functionality. However, receiving another gift from a cracked altar will certainly destroy it, losing it forever.
* Being crowned also counts as a gift. If you are crowned on a cracked altar, it will also destroy it in the process.
* Altars on the Astral Plane will never be destroyed. Note that they can still become cracked but are safe from destruction.
* Altars also sometimes generate cracked. One in four altars will generate pre-damaged (doesn't apply for temples or pre-mapped altars).
* Altars are always cracked after level 15.

* Converting an altar will also frequently crack it. This occurs 1 in 3 times the altar is converted or whenever hostile minions are summoned.

The original altar nerf came from SpliceHack, where altars had a 50% chance of being destroyed after 2 artifact gifts had been bestowed.

A new conduct was added to the #conduct menu so that players can track how many altars have been destroyed in their current game.

#### #offer gift odds
* The odds have been adjusted in favor of the player, especially after 2 gifts have been granted.

| Gifts Granted | Old odds | New odds |
|---------------|----------|----------|
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
* Throne wishes have been removed. To compensate, full recursive identify of items can occur if the player has enough luck.
* Artiwishes only care about previous artiwishes; same for gifts (xnh)
* The chance of getting a djinn from a smoky potion has been halved. The actual chances of getting a wish from the djinn have not been changed.

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
* Crowning only grants *up to* 3 intrinsics. In Vanilla, crowning would grant fire, cold, poison, sleep, and shock resistance, as well as see invisible.
* Intrinsic see invisible is no longer granted via crowning
* Intrinsic telepathy is no longer granted via crowning
* In NerfHack, the game will roll three times to pick random intrinsics. On each roll, if the player already possesses that intrinsic, the roll is lost - otherwise the player gains it permanently.
* Crowning gifts are only granted when crowned, never for #offer.

New intrinsics available when crowned:
* Acid resistance
* Disintegration resistance
* Petrification resistance

### AC PENALTIES

#### Dexterity affects AC

* Ported from EvilHack
* Being encumbered negates AC bonuses from dexterity
* Wearing any kind of heavy metallic body armor (not mithril) or other rigid material also negates beneficial AC bonuses

| Dexterity | AC change |
|-----------|-----------|
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
|-------------|-----------|
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

#### Dragon scales and scale mail changes

* The AC of dragon scales has been reduced from 3AC to 1AC 
* The AC of dragon scale mail has been reduced from 9AC to 4AC
* **Dragon scale mail cannot be wished for**
* Any wishes for scale mails will simply be converted to the equivalent dragon scales instead. For example, if you wish for "yellow dragon scale mail", you will receive "yellow dragon scales".
* When wishing for dragon scales, any specified enchantment is nullified to +0 (xnh)
* Green dragon scale mail also grants regeneration.

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


### PARTIAL REFLECTION

* Ported from EvilHack
* Reflection will deflect most, but not all, of the effects of ray attacks.
  * Example: You are hit by a cold ray, it reflects off your amulet of reflection, but you don't yet possess cold resistance.
* If you don't have sleep resistance, but you reflect a sleep ray, you will fall asleep for a maximum of 1d6 turns.
* If you reflect disintegration ray, you still take 6d6 damage unless you possess disintegration resistance.
* If you reflect a death ray, you still take damage and lose max HP. This can be mitigated by magic resistance and half-spell damage, but is impossible to fully prevent.
* Item destruction from elemental effects (like fire or cold) is prevented when rays are reflected.
* Reflection only provides partial protection from **floating eye gazes** - the player will still be subject to d6 turns of paralysis without free action.
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
|--------------|-----------------|-----------|
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
|----------|-------------|
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
* **Hungerless spellcasting nerf:** Total hungerless casting is not possible anymore and the intelligence requirements have been increased. 20+ INT gets you 1/4-hunger and 18+ gets you 1/2 hunger casting (FIQ)
* Healing spell effectiveness is determined by skill (Evil)

### ITEM EROSION AND DESTRUCTION

* Objects can be completely destroyed via rusting/rotting/corroding (Evil)
* Almost all items are erodeable/destroyable (Evil) - amulets, rings, wands, tools, and food are now eligible for erosion. These new erodeable items can be erodeproofed via confused enchant weapon scrolls.
* Silver items can corrode (xnh)
* The iron ball and chain cannot be destroyed from rusting (Evil)
* Poison gas clouds can rot organic armor
* Monsters can wear down and destroy **ANY** armor with the destroy armor spell
* Item erosion can be repaired by dipping into a potion of restore ability (xnh)
* Scrolls also can burn up when hitting hot ground in Gehennom. 3.7 introduced potions being shattered when dropping on hot ground, but we have taken it a step further.
* Potions can shatter when dropped on cold floor (this shows up in Sokoban and in Gehennom)
* Getting hit by potions of acid can corrode armor. Monster acid attacks and spit also corrode armor. Passive acid attacks corrodes armor more often. Thrown potions of acid can corrode items when they hit a monster or the player.
* Water damage may disintegrate scrolls (Dyna).
* Disintegration rays can vaporize boulders

#### Refactor, unify, and nerf item destruction
* Ported from xNetHack
* This patch fixes some problems with item destruction, making it less random and more dependent on the damage dealt in the interaction. Overall, players should expect to get a more fair deal with fewer items destroyed.

### NEW GREASE EFFECTS

Many of these changes were introduced to work in conjunction with the new grease trap.
* Greased items can't be disarmed with a bullwhip
* Greased items are harder to steal
* Glib hands makes applying any item except towels drop them
* Towels can be used to remove grease from specific objects
* Grease can be washed off towels by wetting them
* Greased towels now operate the same way that cursed towels do

## MONSTERS

### New monsters

| Monster              | sym | origin      | changes                                                                                   |
|----------------------|-----|-------------|-------------------------------------------------------------------------------------------| 
| giant praying mantis | a   | SpliceHack  |                                                                                           |
| locust               | a   | EvilHack    |                                                                                           |
| bloodshot eye        | e   | SLASH'EM    |                                                                                           |
| glowing eye          | e   | SLASH'EM    |                                                                                           |
| blinking eye         | e   | SLASH'EM    |                                                                                           |
| kamadan              | f   | SLASH'EM    | recolored to light green<br/>can jump and have infravision<br/>have poisonous snake bites |
| weretiger            | f/@ | SLASH'EM    | can jump as d                                                                             |
| deep one             | h   | SLASH'EM    |                                                                                           |
| deeper one           | h   | SLASH'EM    |                                                                                           |
| deepest one          | h   | SLASH'EM    |                                                                                           |
| alhoon               | h   | EvilHack    | not covetous<br/>now speed 15<br/>can displace monsters                                   |
| redcap               | i   | SpliceHack  |                                                                                           |
| diamond piercer      | p   | SpliceHack  |                                                                                           |
| god piercer          | p   | SpliceHack  |                                                                                           |
| landshark            | q   | SpliceHack  | recolored to bright blue                                                                  |
| jumping spider       | s   | ESplice     |                                                                                           |
| will-o'-the-wisp     | y   | SpliceHack  |                                                                                           |
| zoo bat              | B   | SpliceHack  |                                                                                           |
| athol                | B   | SLASH'EM    | increased size, weight, and nutrition<br/>strong, berserk, flank, and have infravision    |
| byahkee              | B   | SLASH'EM    | recolored to yellow                                                                       |
| nightgaunt           | B   | SLASH'EM    | recolored to purple<br/>tickle attack is unaffected by MC                                 |
| gray fungus          | F   | Evil/THEM   |                                                                                           |
| adherer              | M   | SpliceHack  |                                                                                           |
| ha-naga              | N   | SpliceHack  |                                                                                           |
| alchemist            | Q   | SpliceHack  | can alchemize acid                                                                        |
| troll mummy          | M   | SLASH'EM    |                                                                                           |
| vampire mage         | V   | SLASH'EM    |                                                                                           |
| merfolk              | ;   | Splice/THEM |                                                                                           |
| thing from below     | ;   | SpliceHack  | can see invisible                                                                         |
| grave troll          | T   | SpliceHack  | can spawn in graves/graveyards<br/>                                                       |
| elven cleric         | @   | EvilHack    |                                                                                           |
| like-like            | P   | NerfHack    |                                                                                           |
| ogre mage            | O   | SLASH'EM    |                                                                                           |
| shadow ogre          | O   | SLASH'EM    |                                                                                           |
| ghoul mage           | Z   | SLASH'EM    |                                                                                           |


### New demons lords:
* Kostchtchie from SpliceHack.
* Lolth from EvilHack
* Buer from SpliceHack.
* Baphomet from SpliceHack.
* Malchanthet from SpliceHack.
* Mephistopholes from SpliceHack


## MONSTER CHANGES

### Dangerous piercers
* All piercers are mindless and can grow up
* Much more AC is required to dodge dropping piercers (before -2AC would nullify their drop attacks, now -22AC is required)
* Piercing damage scales with their level (monster level * 6) with a minimum of 4d6 being dealt.
* Piercers actually pierce helmets; if the damage roll is (12 + (helmet enchantment * 6) or greater, any hard helmet blocking the attack is destroyed. If a helmet is destroyed in this fashion, it absorbs some of the damage.
* Piercers and lurkers/trappers always generate hidden if possible. 

### Reviving Zombies
* Zombie corpses may auto-revive similar to trolls (Evil/xnh)
* Cancelled or beheaded zombies and trolls don't revive (Evil)
* If playing as a priest, you'll automatically suppress many zombie revivals solely through your presence
* Wielding Sunsword prevents zombies corpses from appearing (Evil)
* Playing as a priest reduces the chance of zombie revival by 50% (Dyna)
* 
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
* Baby black dragons get a drain life attack.
* Baby gray dragons get a disenchanting bite.
* They get an additional 1d6 claw attack

**Specific tweaks:**

* baby dragon alignments match their adult counterparts (Evil)
* baby red dragons can berserk
* baby blue dragons are slightly faster at speed 12.
* baby green dragons are slightly higher level and difficulty, and regenerate.
* baby yellow dragons also get a passive acid attack.
* baby gray dragons also flank.
* baby white dragons are weaker.
* 
#### Adult dragon changes
* All adult dragons are now level 16 with a slight increase in difficulty from 20 to 21 (SLASHEM)
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

* all quest guardian colors were changed to cyan
* all A monsters are immune to death magic (xnh)
* baluchitherium is now huge; strengthened claw attack from 5d4 to 5d12
* all bats can see invisible
* captains are considered princes (xnh)
* captains and watch captains generate with keys (Evil)
* centaurs will keep their distance from the player naturally (xnh)
* couatls get sleep and shock resistance (Fourk)
* couatls get a stunning gaze and can generate invisible
* all elementals resist sickness
* elf-lords get 9AC, elvenkings get 8AC (K-Mod)
* ettins count as giants and are vulnerable to sling damage
* floating eyes inflict less passive paralysis; wisdom limits duration (Dyna)
* foocubi gain a level when draining one from the player (xnh)
* giant spiders can ensnare monsters in webs (Evil)
* gnome lords and kings always get gnomish suits.
* gnomish wizards always get a gnomish helm.
* gnomes get candles in the mines twice as often as before
* goblins can generate in small groups (Spork)
* green slimes can hide on the ceiling (xnh)
* green slimes are faster, going from 6 to 13 speed)
* green slimes have a passive sliming attack (Grunt)
* gremlins can steal intrinsics no matter the time of day (FIQ)
* hobbits can get flint with their slings (xnh)
* jellyfish get a passive paralyzing attack
* Keystone Kops cannot be genocided (Un)
* Keystone Kops are tougher: they flank and have increased levels, speed, and attack damage; removed their wander flag (K-Mod)
* lizards appear with slightly less frequency
* ki-rin get shock, sleep, cold, and poison resistance (xnh)
* lords and princes never get negative weapons or armor (xnh)
* lieutenants are considered lords (xnh)
* master liches and arch-liches can see invisible (FIQ)
* mastodon is now huge; strengthened butt attacks from 4d8 to 4d16
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
* skeleton/shade slow attack is ineffective vs undead
* soldiers get half as many C-and-K-rations and cannot load both types of rations (K-Mod)
* soldiers and their higher ranks get level, speed, AC, and MR boosts (K-Mod)
* Soldiers can generate with shuriken
* rabid rats cannot be tamed
* rabid rats and sewer rats hide under objects (xnh)
* scorpions are tiny
* shades get 20MR
* shopkeeper base level has been raised to 13 (xnh)
* shopkeepers and priests are colored yellow (xnh)
* titans can see invisible (FIQ)
* titans resist death magic (SLASHEM)
* titans are level 17 (K-Mod)
* tigers are orange (Evil)
* tigers can also jump
* titanothere is now huge; strengthened claw attack from 2d8 to 8d8
* trappers and lurkers above are mindless and speed 6
* troll meat provides temporary intrinsic regeneration (xnh)
* unique monsters cannot be tamed
* all vortices (v) resist shock damage.
* vampire mages can see invisible
* all werefoo in animal form get infravision
* werewolves have a higher level and difficulty, stronger attacks 
* weretigers have a higher level and difficulty, stronger attacks 
* wraiths also no longer "stalk" the player and follow them across levels (Dyna)
* wumpus is now huge; strengthened bite attack from 3d6 to 6d9
* xans can't fly (dnh)
* yellow and black light explosions are directionless (xnh)
* water elementals can now engulf and suffocate (Evil)

### Unique monster changes
* Croesus can move other monsters out of his way (Evil)
* Ixoth can berserk. Like other dragons also has buffs: level raised from 15->18, speed raised from 12 to 20, AC raised from -1 to -4, stronger claw attacks.
* Ixoth gets poison resistance (Evil)
* Lord Surtur can berserk
* The Master Assassin is poison resistant (xnh)
* Yeenoghu's magic missile attack has been buffed to 6d6 (Evil)

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
* Rodney gets a weapon and the ability to use it (Evil)
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

#### Steeds

* Steeds are more aggressive - if your steed has a tameness level of 15 or more, it will actively attack monsters instead of merely reacting to being attacked. (Evil)

#### Monster spellcasting

* Peaceful monsters won't cast make invisible on themselves.
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
* Deals acid damage to its target. The damage output is dependent on the level of the monster casting it.
* The acid from this spell also has a chance of eroding any unprotected weapons or armor in open inventory.
* Ranged, can be cast at the hero up to 13 squares away.
* Only affects a single square; monsters can cast this at close range

**ice bolt (mage spell):**
* Ported from EvilHack
* This spell explodes a small ice storm upon its target.
* Any non-protected objects in open inventory are subject to being frozen.
* This is a low-level spell, so access to this spell is given to every monster spellcaster that has access to mage-based spells.
* Ranged, can be cast at the hero up to 13 squares away.
* Only affects a single square; monsters can cast this at close range

**fire bolt (mage spell):**
* Ported from EvilHack
* This spell explodes a small fireball upon its target.
* Any flammable objects in open inventory are subject to being burned.
* This is a low-level spell, so access to this spell is given to every monster spellcaster that has access to mage-based spells.
* Ranged, can be cast at the hero up to 13 squares away.
* Only affects a single square; monsters can cast this at close range

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

**evil eye (mage spell):**
* Ported from dNetHack
* When successfully cast on the hero, this lowers your Luck by 1 point.
* Evil eye can only be cast by undead and demon spellcasters.
* Because this is implemented as a gaze attack, the player can increase their protection by being invisible or displaced. There is no maximum range to this spell.


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
  
#### Flanking behavior

* Ported from SpliceHack, with enhancements
* Monsters with this property have the M2_FLANK tag.
* Any two monsters can flank a player (or another monster) if they sandwich the target. However, monsters with this property ("outflankers") are more tactical and will actively seek opportunities to flank the player.
* Monsters gain a large bonus to hit when flanking
* Flanking now scales with monster level (it used to be a flat +4 AC penalty in SpliceHack):
  * AC penalty = 4 + (mdifficulty - 4) / 2
* Flanking has been applied to many appropriate monsters in NerfHack.

* Using a pet, you can also take advantage of flanking. Simply place yourself and your pet in such a way as to "sandwich" the monster. You (or your pet) will get a flanking bonus on the victim when attacking.

Flanking restrictions:
* You cannot flank if hallucinating, afraid, confused, punished, fumbling, wounded, unaware, or stunned.
* You must also be able to see the monster you want to flank.
* Monsters cannot flank if eating, sleeping, fleeing, confused, trapped, being stoned, sick, diseased, hiding, or stunned.

#### Berserking behavior

* Ported from EvilHack, with modifications
* Monsters with this property have the M3_BERSERK tag and can be quite dangerous if you take them for granted
* When berserkers are below 50% of their health, they have a high chance to go into berserk mode
* Monsters can also immediately go berserk if they are woken and angered
* When a monster goes berserk it turns hostile and regains a roll of it's max HP, possibly going far above it's normal max HP
* Nearby denizens are also woken up when a monster goes berserk (it screams a battle cry)
* When berserking, monsters totally ignore Elbereth or Scare Monster. If they are usually skittish or trying to keep away, they will instead actively approach
* When a monster is berserking it also gets -2AC
* Berserking monsters also never flee when their HP gets low
* A berserking monster deals double damage rolls when hitting you
* Taming berserking monsters only un-berserks them, it doesn't pacify or tame
* Monsters that can berserk: all dwarves, mordor orcs, uruk-hai, mumaks, zruty, fire giants, frost giants, storm giants, ettin, all ogres, owlbears, sasquatch, and balrog.

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

## ROLE CHANGES

### ARCHEOLOGIST
* An Archeologist wielding a bullwhip will not fall through trap doors (SLASHEM)
* Archeologists get bonus when searching (FIQ)
* Archeologists can reach basic skill in spears.

### CAVEMAN/CAVEWOMAN CHANGES
* They cannot receive spells from their deity (Evil)
* They have an 80% chance of failing to read any spellbook
* They can increase their max-HP at each level-up if they remain illiterate (from SporkHack/SlashTHEM)
* Their special spell has been removed (Evil)
* The caveman quest has been updated and filled with more jungle type monsters: tigers, pythons, and the like. There is also a lot of water added and ; monsters to occupy it (from SlashTHEM)
* Chromatic Dragon: Like other dragons also has buffs: level raised from 15->18, speed raised from 12 to 20, AC raised from -1 to -4, stronger claw attacks.

Cavepeople have also been gifted with more skills in rudimentary tools like rocks and flint:
* They start the game with more flint and no rocks (xnh)
* They can lash flint to arrows, making them do slightly more damage (from SporkHack/SlashTHEM)

* The narrow passageways in their quest have been opened up for convenience (Evil)
* Their quest narration and dialogue is more caveman-like (from xNetHack/Fourk)
* Cavepersons can get an alignment boost via cannibalism (from Sporkhack)
* Cavepersons' gods sometimes don't respond to prayer. There is a 10% chance of being ignored. (from SporkHack/SlashTHEM)

* Skill adjustments for cave dwellers (Evil)
    knife:          Skilled     -> Restricted
    dagger:         Basic       -> Restricted
    polearms:       Skilled     -> Restricted
    morning star:   Basic       -> Restricted
    attack spells:  Basic       -> Restricted
    matter spells:  Skilled     -> Restricted
    riding:         Restricted  -> Basic

* Cave dwellers also cannot have skills in edged or pointy weapons unrestricted. Note that they can still receive these weapons as altar gifts. 


### HEALER
* Add L's Wounds patch: healers can see damage on monsters
* Healers get a bonus when applying unicorn horns
* Cyclops can berserk

### KNIGHT
* Only lawful Knights can dip for Excalibur (from EvilHack/SporkHack)
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

### PRIEST
* Priests start with a +2 small shield (SLASHEM)
* Priests cannot have edged weapon skills unrestricted (Evil)
* Priests don't receive edged/pointy artifact weapons via altar sacrifice (Evil)
* Instead of the standard crowning gift, priests always receive Mjollnir (Evil)
* Priests reduce the chance of zombie revival by 50% (from DynaHack); when a zombie is killed for good, you get a special message
* Priests can reach basic in riding skill.

### RANGER
* Rangers get extended range for seeing object's dknown appearance (this lets them see potions and gems from much further away)
* Rangers get auto-id for launchers when they reach XP level 7
* Rangers get auto-id for ammo enchantment when they reach XP level 10 (xnh)
* Rangers are not stunned from using portals (they are used to quick travel)

### ROGUE
* Rogues start with +1 short sword (from DynaHack)
* Rogue's can inflict backstab damage for the first thrown weapon
* Rogues get bonus backstab damage when using stilettos in melee
* Rogues also get a multishot bonus for knives.
* Rogues start with a +2 stiletto instead of a short sword
* Rogues start with a stack of knives instead of daggers
* Rogues can counterattack with knives and daggers.
  * While wielding a knife or dagger, a rogue has a chance of counter-attacking a humanoid's weapon attack. There are many restrictions:
    * You can't be polymorphed
    * You can't be wearing any heavy metallic armor
    * You cannot be weak (or worse from hunger), and you cannot be encumbered.
    * You cannot be fumbling or unaware (sleeping or paralyzed).
    * You must be able to see the monster.
    * The chance of countering goes up with your skill in the wielded weapon. Your dexterity can either hurt or help your chances.

### SAMURAI
* Samurai start with +3 wakizashi (from DynaHack)
* Samurai can reach expert in spears.

### TOURIST
* Tourists get automatic type identification for shop items (Un)
* Tourists start with more darts to compensate for more training being needed to advance weapon skills (Un)

### VALKYRIE
* More fire traps on valk quest

### WIZARD
* Most of the wizard's combat based skills have been restricted and removed (Evil)
  * knife, axe, short sword, club, mace, polearms, spear, trident, and shuriken skills.

## PLAYER RACE CHANGES

* Removed infravision from dwarves, elves, gnomes, and orcs. No player-race gets infravision.
* Elves can always squeeze between two trees (xnh)
* Elves get see invisible at level 8
* Gnomes are good at slipping free from grabbing attacks because they are small
* Gnomes start with a nightvision radius of 2 (dnh)
* Gnomes start with an interesting tool
* Gnomes get stealth at level 5 (SLASHEM)
* Orcs start with sickness potion (from SporkHack)
* Orcs get an alignment boost for cannibalism (dnh)

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

## ITEM CHANGES

* Reduced weight of land mines to 40 aum (xnh)
* Reduced weight of beartraps to 50 aum (xnh)
* Reduced weight of bullwhips to 7 aum
* Reduced weight of flint stones to 2 aum (xnh/Spork)
* Reduced weight of pick-axe to 75 aum (SLASHEM)
* Reduced weight of most armors by 50 aum (K-Mod)
* Reduced weight of elven gear by about 1/3'rd (Evil)
* Increased weight of dwarvish and elven mithril coats to 200 aum
* Increase weight of dragon scales and scale mail to 80 aum
* Increase the prices of many magical tools
* Raised price of magic marker to 500
* Raised price of magic lamp to 500 (xnh)
* Raised price of wand of nothing to 500 (EvilHack)
* Port FIQHack's ring initial enchantment rules
* Port the Oily Corpses Patch (xnh)
* Rocks can be broken ((a)pplied) to produce flint stones (xnh)
* Flint stones can be struck (applied) against objects made of iron, producing sparks (fire). This can scare certain monsters away who fear fire. (Spork/THEM)
* Buff the effects of the scroll of light (xnh)
* Reverse the name of the HACKEM MUCHE scroll
* Using a cursed unlocking tool has a chance to break (Evil)
* Using eroded unlocking tools also has a chance to break.
* Playing eroded musical instruments can break the instrument or fail to play.
* Applying rusty stethoscope is much less effective.
* Rusty tin openers can break.
* Amulets of magical breathing are immune to water damage
* Food items can get burned.
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

### Weapon changes
* Any slashing or piercing weapons can now be poisoned (SLASHEM)
* All short swords get +1 to-hit (from DynaHack)
* Reduced probability of long swords generating (K-Mod)
* Wielded polearms grant +2AC
* Spears at expert skill can skewer through enemies, allowing you to hit the enemy directly behind the target. Peacefuls are prevents from being hit unless the spear is cursed.
* Spetums can skewer up to 3 monsters when used in melee while riding a steed
* Ranseurs can disarm monsters or the player when pounded or used in melee while riding a steed.
* Bardiches have a 1 in 100 chance of beheading monsters (or the player)
* +4 to-hit bonus for attacking with a scimitar on a steed.
* Wielding and unwielding curved swords takes 0 turns.
* Morning stars and flails can stun monsters (or the player) on critical hits. Player must be skilled or better.

#### Slings
* Projectiles receive a powerful strength bonus when using slings (xnh)
* Gem class projectiles do minimal damage vs thick-skinned monsters
* Launching gem class projectiles from slings has the potential to instakill H
  
### Magic markers
* Appear randomly much less often (1/5'th of the frequency in Vanilla)
* They can still be creating from polypiling

### Wands of wishing
* Always generate pre-charged, meaning they never be charged, otherwise they will explode (many variants incorporate this)
* Wands of wishing only generate with d2 charges
* The maximum possible wishes from any WoW is 3 wishes

### Unicorn horns

* Success depends on their enchantment level (SLASHEM)
* Now one-handed, dealing d6 vs sm/d7 vs large
* Having skill in unicorn horn has a positive impact on your success when applying, having no skill has a negative impact.
* Basic skill grants a 10% bonus to success, skilled 20%s, and expert 40%. This allows roles that can attain proficiency to not have to enchant it so high.

* Successfully applying a unihorn also exercises your skill in it by 5 points. 
* The healer gets a bonus when applying unicorn horns. Instead of the standard 30% success rate when the unihorn is +0, they have a 40% success rate.

### War Hammer
* war hammers have been changed from a one-handed weapon into a competitive two-handed weapon (xnh)
* They now deal 2d6 vs small monsters and 2d8 vs large

### SCROLLS

* Scrolls of genocide only clear a single monster species on the level (uncursed) or globally (blessed) (Un)
* Endgame genocide nerf. Monsters cannot be fully genocided after entering the planes. Any genocides executed in the end game will be uncursed and only have a 1 in 4 chance of destroying each monster of that species. This is a soft counter to the plane of water genocide strategy that most players employ. Players can still genocide ; before entering the planes, but beware, there might be more dangerous replacements waiting for them.
* Enchant armor: Ability to choose worn piece of armor to enchant/repair (Evil)
* Give enchant vibrate warning for all weapons/armor (from DynaHack)
* Blessed scroll of destroy armor asks which armor to destroy (xnh)
* Confused cursed scroll of destroy armor prompts for armor to fix
* Confused scrolls of gold detection no longer detect magic portals
* Confused scroll of identify gives enlightenment (xnh)
  
### POTIONS

* Dipping an eroded item in restore ability repairs the erosion (xnh)
* Acid potions are immune to being destroyed by freezing (xnh)
* Implement behavior for cursed potion of gain ability (xnh)
* More potion breathing effects (xnh)
* Thrown potions of hallucination confuse monsters (Evil)
* Potion of paralysis lasts 3-24 turns on monsters (Evil)

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
* Increase wand to-hit chance for high-dex characters  (from SpliceHack)


## SHOP CHANGES
**Lighting shops:**
* Magic lamps are one notch rarer - down to 11.3% per game now overall. (Spork)
* Potions of oil have been eliminated from appearing.
* Non-candle and non-lamp items have had their probabilities minimized.

## NEW ITEMS

**stomping boots:**
* Instakills any tiny monster you attack or run into. (Splice)
* Small monsters can also get stomped with a 1 in 40 chance.
* Flying monsters, monsters in water, amorphous, and incorporeal monsters are immune to stomping.

**flying boots:** Levitation boots have been removed and replaced with flying boots which simply grant flight. Medusa's Island gets flying boots instead of levitation boots.
** gauntlets of force:** Increase strength bonus, makes forcing locks and opening doors take 1 turn. Chance of stunning. Can break iron bars, boulders.
**anti-magic shield:** Leather shield that provides magic resistance.
**gnomish boots:** Provides 0AC + bonus 2AC for gnomes (THEM)
**gnomish helm:** Provides 0AC + bonus 2AC for gnomes (THEM)
**gnomish suit:** Provides 1AC + bonus 2AC for gnomes (THEM)
**orcish boots:** Provides 1AC + bonus 2AC for orcs (Evil)

**wand of corrosion:** shoots acid rays (Splice)

**wand of poison gas:** shoots poison rays (Splice)

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

## NEW ARTIFACTS

TODO: Break the table into alignment, special dmg, wielded, carried

| Name                | Align     | Type                  | From       | Notes                                                                                                                                                                       |
|---------------------|-----------|-----------------------|------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Disrupter           | neutral   | mace                  | SLASHEM    | deals 1d30 damage and +d5 to-hit vs undead</br>grants warning vs undead                                                                                                     |
| Keolewa             | neutral   | club                  | EvilHack   | deals 1d8 shock damage, +d5 to-hit</br>grants shock resistance while wielded                                                                                                |
| The End             | neutral   | scythe                | SpliceHack | deals 1d20 cold damage, +d3 to-hit</br>grants drain resistance while wielded                                                                                                |
| Serpent's Tongue    | chaotic   | dagger                | SLASHEM    | deals double damage to all monsters<br/>bonus damage vs monsters that don't resist poison                                                                                   |
| Doomblade           | chaotic   | orcish short sword    | SLASHEM    | deals 1d20 damage<br/>25% chance of (1d4 * 5) bonus damage                                                                                                                  |
| Poseidon's trident  | chaotic   | trident               | SpliceHack | deals +d7 damage, +d3 to-hit</br>grants magical breathing while wielded<br/>#invoke for water walking and an earthquake                                                     |
| Origin              | unaligned | quarterstaff          | SpliceHack | deals +d6 damage, +d2 to-hit</br>grants teleport control while wielded<br/>grants spellcasting bonuses while wielded                                                        |
| Hellfire            | chaotic   | crossbow              | SLASHEM    | bolts fired from Hellfire deal +d7 damage and explode in fire<br/>grants fire resistance while wielded                                                                      |
| Plague              | chaotic   | orcish bow            | SLASHEM    | arrows fired from Plague are auto-poisoned and deal +d7 damage<br/>grants sickness resistance while wielded                                                                 |
| Pridwen             | lawful    | large shield          | SpliceHack | grants physical damage reduction while wielded</br>grants steadfastness while wielded                                                                                       |
| Quick Blade         | lawful    | elven short sword     | SLASHEM    | +d9 to-hit, +d2 damage                                                                                                                                                      |
| Carnwennan          | lawful    | knife                 | SpliceHack | deals +d8 damage<br/>+d3 to-hit<br/>grants stealth and searching while wielded                                                                                              |
| Load Brand          | unaligned | heavy sword           | HACKEM     | weights 500aum<br/>deals +d20 damage<br/>Confers steadfastness and MC1 protection<br/>Confers physical damage reduction<br/>Absorbs curses like Magicbane                   |
| Snakeskin           | Neutral   | robe                  | SlashTHEM  | Confers acid resistance<br/>Confers hallucination resistance                                                                                                                |
| Blackshroud         | neutral   | cloak of invisibility | SlashTHEM  | Grants warning and drain resistance                                                                                                                                         |
| Mirrorbright        | neutral   | shield of reflection  | SLASHEM    | Doesn't inhibit spellcasting<br/>Confers hallucination resistance                                                                                                           |
| Deluder             | neutral   | cloak of displacement | SLASHEM    | Confers stealth and MC1 protection                                                                                                                                          |
| Whisperfeet         | neutral   | speed boots           | SLASHEM    | Confers stealth and luck                                                                                                                                                    |
| Mayhem              | chaotic   | stomping boots        | HACKEM     | Confers conflict and warning vs undead                                                                                                                                      |
| The Lenses of Truth | unaligned | lenses                | HACKEM     | Confers see invisible and searching when worn<br/>Confers stun resistance when worn                                                                                         |
| Serenity            | lawful    | silver spear          | HACKEM     | +d5 to-hit, +d10 damage<br/>Confers fire resistance when wielded<br/>Prevents monsters from berserking<br/>Counters 80% of monster spells<br/>Absorbs curses like Magicbane |
| Mouser's Scalpel    | neutral   | rapier                | slashem-up | +d5 to-hit, +1 damage<br/>Capable of multiple bonus hits with no limit                                                                                                      |


## ARTIFACT CHANGES

Artifact weapons can now be dual-wielded (Evil). Lawful and chaotic weapons cannot be two-weaponed.

* The Tsurugi of Muramasa has a 10% chance of bisection (SLASHEM)
* Magicbane is a quarterstaff (FIQ)
* Creating Excalibur will fix any negative enchantment on it (xnh)
* Fire Brand instakills highly flammable monsters and green slimes (xnh)
* Fire Brand: attacking with Fire Brand cures sliming
* Frost Brand instakills water elementals.
* Vorpal blade grants see invisible while wielded
* Vorpal Blade provides warning vs jabberwocks (Evil)
* Vorpal blade gets a 10% chance of beheading (SLASHEM)
* The Heart of Ahriman now grants slotless flying and displacement instead of stealth (FIQ)
* Trollsbane grants regeneration while wielded (many variants)
* The Eyes of the Overworld protect against more gaze attacks (Evil)
* Prevent Cleaver from cleaving peaceful bystanders (xnh)
* Giantslayer is now a spear (Evil)
* Giantslayer conveys 18/** strength while wielded (DynaHack)
* Ogresmasher can also hurtle light-weight monsters (Evil)
* Werebane provides protection from shapechangers when wielded
* The Sceptre of Might gets a flat +3 damage buff
* The Longbow of Diana confers reduced damage when wielded
* Increased Mjollnirs wakeup radius when it strikes monsters with lightning
* Mjollnir can be invoked for a lightning bolt (xnh)

**Bane changes:**
* All banes provide warning vs their bane monster type when wielded (Evil)
* All banes glow red in response to their monster types (Evil)
* All banes can instakill their associated monster types with a 1 in 5 chance (Un)
* Sunsword and Disrupter don't get instakills. 
* Banes can't instakill unique monsters

## DUNGEON CHANGES

* The Rogue level has been disabled (many variants)
* Chickatrices and cockatrice eggs will now appear in cockatrice nests (xnh)

### Art rooms

* Ported from SpliceHack
* These rooms have a one-time event that occurs upon entering a room
* Most of the time it's a fun piece of art depicting something with the denizens of the dungeon. But sometimes it's a special effect.
  * You might see an image of your god, invoking enlightenment
  * You might find a partial map of the level
  * You might encounter a scary image, stunning you for a few turns
* Art rooms help exercise INT and WIS, depending on the room
* To get any effects, you must not be blind when you enter the room

### CASTLE CHANGES

* The castle level is now marked as a graveyard
* Castle barracks may open into courtyard instead of throne room, letting soldiers flood the courtyard more quickly (xnh)
* Added iron bars to the castle perimeter
* Iron bars have been added to the castle towers (Spork)
* The location of the chest containing the wand of wishing has been obfuscated. You will find matching chests and scrolls in each of the towers if you use object detection. The other chests have wands of nothing inside. (Spork)
* The drawbridge passtune range has been expanded by one square. (xnh)
* The drawbridge also does not always close with the passtune, one out of five times it will malfunction when trying to close it. (xnh)
* Castle courtyards are unlit.

### Valley of the Dead

* Player can't regenerate hit points while in the Valley of the Dead (Evil)
* Instead of dart traps, the player will encounter magic traps (Evil)
* Less ghosts are guaranteed in the valley

### DUNGEON LEVELS/ROOMS

#### Streamlined Gehennom

* Gehennom has been dramatically shortened to 5-7 levels.
* All the demon lairs have been removed.
* The fake wizard levels have been removed.
* The wizard's tower levels have been moved out of Gehennom to the main dungeon right below Medusa's Island.
* The portal to the wizard's tower has been moved to a random castle tower and changed to a stair up.
* Some of the maze levels in gehennom have been trimmed out, most of the level generation is cave-like.
* All hell fill levels are either hot or cold.


#### Sokoban

* Sokoban levels ar