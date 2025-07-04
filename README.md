# NerfHack
- [NerfHack](#nerfhack)
  - [QUALITY OF LIFE FEATURES](#quality-of-life-features)
      - [Safer bags of holding:](#safer-bags-of-holding)
    - [Streamlined Identification Features](#streamlined-identification-features)
    - [Interface Changes](#interface-changes)
      - [Farlook enhancements](#farlook-enhancements)
    - [New config options](#new-config-options)
    - [Wizmode features](#wizmode-features)
  - [INTRINSICS AND EXTRINSICS](#intrinsics-and-extrinsics)
    - [Partial Intrinsics](#partial-intrinsics)
    - [Partial Reflection](#partial-reflection)
    - [Magic cancellation (MC) protects items vs cancellation](#magic-cancellation-mc-protects-items-vs-cancellation)
    - [Gaze attack protection](#gaze-attack-protection)
    - [Slow digestion nerf](#slow-digestion-nerf)
    - [Stealth changes](#stealth-changes)
    - [Flying Changes](#flying-changes)
    - [Aggravate Monster changes](#aggravate-monster-changes)
    - [Impaired Actions](#impaired-actions)
  - [MECHANICS CHANGES](#mechanics-changes)
    - [Instakills](#instakills)
    - [Wishing](#wishing)
    - [Genocide has been nerfed and renamed to Exile](#genocide-has-been-nerfed-and-renamed-to-exile)
    - [Slow Luck timeouts (modified)](#slow-luck-timeouts-modified)
    - [Pet behavior](#pet-behavior)
      - [Pet Theft](#pet-theft)
      - [Pets are limited by charisma](#pets-are-limited-by-charisma)
    - [Price Identification Nerf](#price-identification-nerf)
    - [Polymorphing Objects and Polypiling](#polymorphing-objects-and-polypiling)
    - [Poly-Self](#poly-self)
    - [Elbereth and Scare Monster](#elbereth-and-scare-monster)
    - [New Grease Effects](#new-grease-effects)
    - [DEMON AND DEMON LAIR CHANGES](#demon-and-demon-lair-changes)
    - [Endgame Changes](#endgame-changes)
    - [Farming Nerfs](#farming-nerfs)
    - [Underwater mechanics](#underwater-mechanics)
  - [AC nerfs \& buffs](#ac-nerfs--buffs)
    - [Dexterity affects AC](#dexterity-affects-ac)
    - [Encumbrance affects AC](#encumbrance-affects-ac)
  - [SKILLS AND EXPERIENCE](#skills-and-experience)
    - [Skill Changes](#skill-changes)
    - [Shield Skill](#shield-skill)
      - [Effects at different skill levels:](#effects-at-different-skill-levels)
    - [Experience Curve Changes](#experience-curve-changes)
    - [Leveling up bonuses](#leveling-up-bonuses)
    - [To-hit bonuses and penalties](#to-hit-bonuses-and-penalties)
  - [ITEM CHANGES](#item-changes)
    - [Item Erosion and Destruction](#item-erosion-and-destruction)
      - [Fragile items are more vulnerable](#fragile-items-are-more-vulnerable)
      - [Bones files trimming](#bones-files-trimming)
    - [Anti-magical items resist being enchanted (from SpliceHack)](#anti-magical-items-resist-being-enchanted-from-splicehack)
    - [Weapon changes](#weapon-changes)
      - [Higher max weapon enchantment](#higher-max-weapon-enchantment)
      - [Misc weapon changes](#misc-weapon-changes)
      - [Slings](#slings)
    - [Armor changes](#armor-changes)
      - [New armor type: bracers](#new-armor-type-bracers)
      - [New dragon armor system: DSM replaced by scaled armor](#new-dragon-armor-system-dsm-replaced-by-scaled-armor)
    - [Comestibles](#comestibles)
    - [Potions and alchemy](#potions-and-alchemy)
      - [Diluted potion effects](#diluted-potion-effects)
      - [Gem Alchemy](#gem-alchemy)
    - [Scrolls](#scrolls)
    - [Wands](#wands)
      - [Wands of wishing](#wands-of-wishing)
    - [Rings/Amulets](#ringsamulets)
      - [Eating Jewelery \& Accessories](#eating-jewelery--accessories)
    - [Tools](#tools)
      - [Magic markers](#magic-markers)
      - [Unicorn horns](#unicorn-horns)
      - [Mirrors confer reflection while carried](#mirrors-confer-reflection-while-carried)
    - [Gems/Stones/Rocks](#gemsstonesrocks)
  - [NEW ITEMS](#new-items)
    - [potions of blood and vampire blood](#potions-of-blood-and-vampire-blood)
    - [potion of milk](#potion-of-milk)
    - [playing card deck](#playing-card-deck)
    - [scroll of cloning](#scroll-of-cloning)
    - [deck of fate](#deck-of-fate)
    - [healthstone](#healthstone)
    - [whetstone](#whetstone)
    - [foulstone](#foulstone)
  - [ARTIFACT CHANGES](#artifact-changes)
    - [General artifact changes](#general-artifact-changes)
    - [Specific artifact changes](#specific-artifact-changes)
  - [NEW ARTIFACTS](#new-artifacts)
    - [Load Brand](#load-brand)
    - [The Lenses of Truth](#the-lenses-of-truth)
    - [Serenity](#serenity)
    - [Thunderfists](#thunderfists)
    - [Glyph Shard](#glyph-shard)
  - [NEW MONSTERS](#new-monsters)
    - [New monster notes](#new-monster-notes)
  - [MONSTER CHANGES](#monster-changes)
    - [Misc monster changes](#misc-monster-changes)
    - [Delayed stoning for all footrice effects](#delayed-stoning-for-all-footrice-effects)
    - [Dangerous piercers](#dangerous-piercers)
    - [Reviving and Poisonous Zombies](#reviving-and-poisonous-zombies)
    - [Dragon changes](#dragon-changes)
    - [Unique monster changes](#unique-monster-changes)
      - [Warping behavior for demon princes and lords and quest nemeses](#warping-behavior-for-demon-princes-and-lords-and-quest-nemeses)
  - [MONSTER BEHAVIOR](#monster-behavior)
    - [Monster item use](#monster-item-use)
    - [Monster accessory use](#monster-accessory-use)
    - [Misc monster behavior changes](#misc-monster-behavior-changes)
    - [Flanking behavior](#flanking-behavior)
    - [Berserking behavior](#berserking-behavior)
    - [Rabid monsters](#rabid-monsters)
    - [Diseased monsters](#diseased-monsters)
    - [Accurate behavior](#accurate-behavior)
    - [Jumping behavior](#jumping-behavior)
    - [Withering attacks](#withering-attacks)
  - [MONSTER SPELLCASTING](#monster-spellcasting)
    - [Mage Spells](#mage-spells)
    - [Clerical Spells](#clerical-spells)
  - [ROLE CHANGES](#role-changes)
    - [Archeologist](#archeologist)
    - [Barbarian](#barbarian)
    - [Cave Dweller](#cave-dweller)
    - [Healer](#healer)
    - [Knight](#knight)
    - [Monk](#monk)
    - [Priest](#priest)
    - [Rogue](#rogue)
    - [Ranger](#ranger)
    - [Samurai](#samurai)
    - [Tourist](#tourist)
    - [Valkyrie](#valkyrie)
    - [Wizard](#wizard)
  - [NEW ROLES](#new-roles)
    - [Undead Slayer](#undead-slayer)
    - [Cartomancer](#cartomancer)
  - [PLAYER RACE CHANGES](#player-race-changes)
    - [Elves](#elves)
    - [Dwarves](#dwarves)
    - [Gnomes](#gnomes)
    - [Orcs](#orcs)
    - [New race/role combos.](#new-racerole-combos)
    - [Racial item preferences](#racial-item-preferences)
  - [NEW RACES](#new-races)
    - [Dhampir](#dhampir)
      - [NerfHack introduces smarter feeding to regulate vampire bite mechanics:](#nerfhack-introduces-smarter-feeding-to-regulate-vampire-bite-mechanics)
      - [Dhampir's resistances and abilities](#dhampirs-resistances-and-abilities)
    - [Grung](#grung)
      - [Grung's resistances and abilities](#grungs-resistances-and-abilities)
      - [Grung Hydration Mechanics](#grung-hydration-mechanics)
  - [SPELLCASTING CHANGES](#spellcasting-changes)
    - [Spell memory](#spell-memory)
    - [Other spellcasting changes](#other-spellcasting-changes)
    - [New skill-dependent spell ranges](#new-skill-dependent-spell-ranges)
    - [Spell changes and updates](#spell-changes-and-updates)
  - [DUNGEON CHANGES](#dungeon-changes)
    - [New levels](#new-levels)
    - [New themed rooms](#new-themed-rooms)
    - [Shop Changes](#shop-changes)
    - [Castle changes](#castle-changes)
    - [Valley of the Dead](#valley-of-the-dead)
    - [Enhanced Gehennom](#enhanced-gehennom)
    - [The Wizard's Tower Overhaul](#the-wizards-tower-overhaul)
    - [Vlad's Tower revamp](#vlads-tower-revamp)
    - [Sokoban](#sokoban)
    - [Fort Ludios](#fort-ludios)
    - [Minetown/Mines End](#minetownmines-end)
    - [Oracle](#oracle)
    - [Temple to Moloch level](#temple-to-moloch-level)
    - [Lost Tomb level](#lost-tomb-level)
    - [The Wyrm Caves](#the-wyrm-caves)
    - [Big Room](#big-room)
    - [Grass](#grass)
    - [Puddles](#puddles)
    - [Forges](#forges)
      - [Forging and Forging Recipes](#forging-and-forging-recipes)
    - [Toilets](#toilets)
      - [Toilet kicking:](#toilet-kicking)
    - [Bloody tiles](#bloody-tiles)
    - [Traps](#traps)
      - [New container traps](#new-container-traps)
      - [Falling rock traps](#falling-rock-traps)
      - [Spear traps](#spear-traps)
      - [Magic beam traps](#magic-beam-traps)
      - [Grease traps](#grease-traps)
      - [Cold Traps](#cold-traps)
      - [Door traps](#door-traps)
      - [Booby-trapped tins](#booby-trapped-tins)
  - [SPECIAL ROOMS](#special-rooms)
    - [Art rooms](#art-rooms)
    - [Room colors patch](#room-colors-patch)
    - [New room: dragon lair (from SLASH'EM).](#new-room-dragon-lair-from-slashem)
    - [New room: giant courtroom (from SLASH'EM).](#new-room-giant-courtroom-from-slashem)
    - [New room: Real zoo (from SLASH'EM).](#new-room-real-zoo-from-slashem)
    - [New room: Fungus farm (from SLASH'EM).](#new-room-fungus-farm-from-slashem)
    - [New room: Migo hive (from SLASH'EM).](#new-room-migo-hive-from-slashem)
    - [New room: terror halls (from SlashTHEM)](#new-room-terror-halls-from-slashthem)
  - [ALTARS, PRAYER, AND PRIESTS](#altars-prayer-and-priests)
    - [Revised divine protection scheme](#revised-divine-protection-scheme)
    - [Altar cracking](#altar-cracking)
    - [Altar generation](#altar-generation)
    - [#offer GIFT ODDS](#offer-gift-odds)
    - [Crowning](#crowning)
  - [THE QUEST](#the-quest)
  - [MISC CHANGES](#misc-changes)
  - [CREDITS](#credits)
    - [NetHack Ideas Archive credits](#nethack-ideas-archive-credits)
    - [Changes that were later adopted into NetHack 3.7.0](#changes-that-were-later-adopted-into-nethack-370)
    - [Special thanks to:](#special-thanks-to)
    - [Thanks:](#thanks)

This changelog exists to track the changes in NerfHack: https://github.com/elunna/NerfHack.


## QUALITY OF LIFE FEATURES

* Chaotics do not get alignment penalties for angering, attacking, or killing peacefuls (xNetHack)
* Running and traveling no longer pushes boulders (xNetHack)
* When traveling, engravings on graves will not be stopped on or considered 'interesting'
* When traveling, the player will avoid ice and puddles.
* Stop occupations when the hero is caught in a poison gas cloud
* Allow lighting only 1 candle in a stack (GnollHack).
* Inform player when casting healing at monsters with full HP.
* Swapping weapons take 0 turns (dNetHack)
* A welded cursed quarterstaff doesn't block spellcasting (xNetHack)
* Crysknives are never auto-quivered
* Launchers don't count as weapons for the 'hit with a wielded weapon' conduct
* Give enchanting vibrate warning for all weapons and armor when using scrolls of enchant weapon or armor (Dynahack)
* The spellcasting skill bonus no longer applies after you can advance the spell school past basic.

#### Safer bags of holding:
The following safeguards were added to protect players from exploding bags:
* Players cannot put **known** wands of cancellation or magical bags into **identified** bags of holding. Keep in mind, unknown wands and bags are still dangerous and should be handled with care until formally identified (dNetHack)
* Players are prevented from tipping **known** explosive items into **identified** bags of holding
* Empty wands of cancellation may still be placed inside bags of holding (no risk of blowing up)

DISCLAIMER: Bag of holding explosions are not prevented when confused or hallucinating!

* Another subtle but helpful change: bags are not susceptible to burning up when lava walking. In Vanilla this was never the case, but in some variants bags can sometimes burn up unless foo-proofed.

### Streamlined Identification Features
A general design philosophy of NerfHack is to automatically identify items that are unambiguous from various effects. If a quick wiki lookup is all that is needed (ie: sink ring identification) let's save the player from opening up a browser.

* All roles start out knowing potions of water, blank scrolls, and scrolls of identify (one exception is cave dwellers, who don't know scrolls of identify)
* When dropping a container on an altar, the BUC status of all contained items is revealed (NetHack4)
* Your primary wielded weapon is auto-identified after killing enough monsters with it (EvilHack)
* Auto-identify rings of increase damage and accuracy with enough experience killing monsters.
* When you have expert skill in a weapon type, you can wield those weapons to auto-id the enchantment (only for non-missile weapons)
* Auto-ID potions of acid when water explosions result from dipping (xNetHack)
* Auto-ID potions of acid when a lichen corpse is dipped into one
* Auto-ID potions of sickness when they coat a weapon in poison
* Auto-ID potions of sickness and fruit juice when dipping a unihorn in sickness
* Auto-ID potions of see invisible or fruit juice by process of elimination when quaffed.
* Auto-ID potions of restore ability when quaffed
* Auto-ID potions of booze when quaffed
* Auto-ID amethyst, fruit juice, and booze when dipping amethyst into booze (Fourk)
* Auto-ID some potions when inhaling their vapors (xNetHack)
* Auto-ID scrolls of scare monster when they crumble from being picked up (UnNetHack)
* Auto-ID scrolls that have obvious effects when read:
  * scare monster
  * confuse monster
  * food detection
  * remove curse
  * flood
  * scrolls of enchant armor when they erodeproof armor or create dragon scaled armor
* Auto-ID rings dropped into a sink (UnNetHack)
* Auto-ID rings of regeneration upon wearing
* Auto-ID +0 rings of protection (if MC is increased)
* Auto-ID wands of cancellation after they destroy a bag of holding (UnNetHack)
* Auto-ID most wands when engraving (xNetHack)
* Automatically use a process of elimination for auto-identifying wands when available (UnNetHack)
* Auto-id flint stones yielded from applying rocks to each-other
* Auto-ID most musical instruments upon use (UnNetHack)
* Auto-ID magic lamps and oil lamps when #rub is used (UnNetHack)
* Auto-ID dunce caps when one is first put on (UnNetHack)
* Auto-ID jumping boots when they are worn (UnNetHack/Ace)
* Auto-ID water walking boots when they waterwalk (xNetHack)
* Auto-ID kicking boots when you #kick when them
* Auto-ID BUC of products from BUC identified tinning kit or horn of plenty (UnNetHack++)
* Auto-ID BUC of wands when they backfire
* Auto-id bags of holding when items are added or removed
* Blessed stethoscopes can identify eggs (EvilHack/Sporkhack)
* Make rustproof/erodeproof/fixed known by default (Dynahack)
* **Items that are 'lost'** from the players inventory are longer un-identified.

### Interface Changes
* Created a new splash screen for the Windows build.
* A detailed object and monster Pokedex is available in the in-game lookup (xNetHack/UnNetHack/HackEM)
  * Farlook any monster (press '//'), then press ':' to access the pokedex entry
  * You can also search for a monster or item: press '/' then '?', then type the name of the thing you want information on.
  * For item details, open your inventory and press the letter of the item for info.
* Object lookup also works for artifacts (HackEM)
* Peaceful monsters are underlined [TTY and curses] (xNetHack)
* Magic cancellation (MC) value is shown on the bottom line (EvilHack)
* Skill caps and percentage towards next level is available in #enhance
* Show available skill slots in #enhance menu (Dynahack)
* Show if a monster ignores magical scaring or Elbereth in the pokedex info.
* Add inventory weight/carrycap and n/52 items display
* /> or < can be used to autotravel to stairs (autostairtravel option)
* Display AC values for armor in the hero's inventory (SpliceHack)
* Prayer statistics (last prayed, reconciled, received a gift, divine protection) can be viewed in the attributes screen (via Ctrl-X)
* All position prompts may be aborted
* Show warning level 0 for very weak monsters (Dynahack)
* More descriptive combat messages have been added to enhance hits and misses (xNetHack)
* The SLASH'EM style message is used for getting zapped by cancellation
* Show explicit messages for objects that are randomly cursed from monsters cursing your items or wizard harassment (Dynahack)
* Print an explicit message when summon nasties occurs as part of wizard harassment
* Special room and special level walls can have their own unique coloring (SpliceHack/xNetHack)
* Enabled autocomplete for #twoweapon
* Enable **full options** by default
* Disabled **#chronicle** from auto-completing (so #chat will autocomplete as normal)
* Disabled **farlook help**
* Disabled the 3.7 **tutorial**
* Changed the symbol for **sinks** back to #
* The hero's color reflects their race (SLASH'EM)
* Suggest donation amount (relative to XP level) when #chatting to priests
* Use NERFHACKOPTIONS instead of NETHACKOPTIONS so it does't clash with NetHack.
* Added a "Rabid" status for when the player is rabid
* Added a "Phasing" status for when the player is phasing
* Don't livelog events in explore mode

#### Farlook enhancements
* We are able to see more monster conditions on farlook (EvilHack/SpliceHack/xNetHack)
  * You can ascertain monsters that are berserking, rabid, and/or spell-beings which appear as "sparkling".
* Farlook also shows amulets and rings monsters are wearing
* We are able to see what weapon a monster is wielding from farlook (EvilHack)
* We are able to see roughly how much armor a monster is wearing on farlook (EvilHack)

### New config options

* **showdamage:** Displays damage dealt and flanking bonuses/penalties
* **do_not_flip_soko:** Enables player to choose whether they want Sokoban levels to be flipped. If enabled, incurs Sokoban penalty for each level used.
* **invweight:** Show weights of objects in inventory
* **autostairtravel:** Allow fast travel to stairs with < and >
* **hide_old_spells:** This option allows the player to control whether spells with 0% retention show up in the spellcasting menu.

### Wizmode features
* The #wizcrown command has been added for testing crowning (EvilHack)
* The #wizclear (^z) command, clears all monsters on the screen (SpliceHack)
* Wizard mode can override an artifact ignoring you (xNetHack)
* Allow teleportation into unteleportable spots in wizard mode
* Allow wishing (^W) for monsters in wizmode (UnNetHack)
* Changed #debugfuzzer command to just #fuzz
* Allow wishing for specific spell beings
* Show timeouts for sick, rabid, withering, and other afflictions in the wizmode enlightenment menu


## INTRINSICS AND EXTRINSICS


* The new Saving Grace feature introduced in 3.7.0 has been disabled.
* The beginner flag is only set true for tourists. This means that you will usually be able to use-test items more effectively earlier in the game.
* Invisibility and see invisible cannot be permanently gained intrinsically (xNetHack)
* Telepathy cannot be permanently gained intrinsically
* Teleportitis cannot be permanently gained intrinsically.
* Teleport control cannot be permanently gained intrinsically.
* Amnesia can make you forget intrinsic telepathy.
* Intrinsic disintegration resistance doesn't protect items from disintegration.
* Regeneration only causes additional hunger when it's actively healing your HP.
* When regeneration is active, it burns twice as much hunger.
* Free action protects from stoning paralysis.
* The chance of gaining levels from wraiths has been reduced using the SLASH'EM version of edible wraith corpses.
* Strength gain nerfs: giant corpses have less of a chance of conferring strength gain (SLASH'EM)
* Lessen confusing messages for confuse monster effects wearing off.
* Passive fire damage burns away slime.
* Unchanging pauses rather than cancels sliming (xNetHack)
* Phasing allows escape from being engulfed (EvilHack)
* Max carry capacity has been raised to 1250, with strength playing a larger factor in its calculation.
* Warn the player that invisibility is about to time out (xNetHack)
* There is an increased CON penalty for getting lifesaved (xNetHack).
* Extrinsic acid resistance only provides 50% damage reduction.
* Magic resistance and spell damage reduction only halve magic missile damage instead of preventing it (EvilHack)
* Half physical damage only provides one-quarter (25%) physical damage reduction.
* Half spell damage only provides one-quarter (25%) spell damage reduction.
* Having really low intelligence (under 6 INT) prevents you from reading most things (EvilHack).
* Low intelligence players also cannot successfully write Elbereth.

### Partial Intrinsics
* Ported from EvilHack
* Instead of binary resistances where the player either has it or doesn't, the player gradually builds up their resistance from 0% to 100%.
* When eating a corpse, player gains a percentage of certain intrinsics.
* Percentage gained is based on the weight of the corpse; minimum being 2% and maximum at 25% (capped at 100%).
* Tins convey the same percentage from whatever they are made from.
* You will always get a percentage intrinsic from each corpse eaten.
* You receive all intrinsics that the corpse can convey if there are multiple intrinsics it can give (ie: eating a black pudding glob grants a small percentage each of poison, cold, and shock resistance.)
* Damage and effects dealt are adjusted based on the percentage intrinsic currently possessed. Damage reduction is rounded down, requiring slightly more resistance to be effective.
* Gremlins steal (25 + d25)% of your intrinsics
* Cold traps and ice demons also steal (25 + d25)% of your cold resistance.
* Enlightenment always shows the partial percentage acquired for intrinsics. If you have an extrinsic source that will be displayed separately.

### Partial Reflection
* Ported from EvilHack
* Reflection will deflect most, but not all, of the effects of ray attacks.
* Example: You are hit by a cold ray, it reflects off your amulet of reflection, but you don't yet possess cold resistance.
* If you don't have sleep resistance, but you reflect a sleep ray, you will fall asleep for 1d6 turns (which could be lessened by your current level of sleep resistance).
* If you reflect disintegration ray, you still take 12d6 damage (subject to your current level of disintegration resistance).
* If you reflect a death ray, you still take damage and lose max HP. This can be mitigated by magic resistance and spell damage reduction, but is impossible to fully prevent.
* Item destruction from elemental effects (like fire or cold) is prevented when rays are reflected.
* Reflection only provides partial protection from **floating eye gazes** - the player will still be subject to d2 turns of paralysis without free action. This is weighted on Luck, so the higher your Luck the better the chance to avoid the gaze.
* **Medusa's gaze** has no effect on her if reflected back from more than 3 squares away.
  * If she might be affected by her own gaze, Medusa will protect herself 98% of the time.
* Monsters also have partial reflection, making them more vulnerable to various ray attacks.

### Magic cancellation (MC) protects items vs cancellation
* Any level of MC limits the damage if the enchantment on an item is positive.
* If the enchantment is negative, the item's enchantment is cancelled to +0 as usual.
* If it's a potion, scroll, or other item that would be blanked, it also gets an additional save roll.
* With MC0, there is no protection when facing a cancel zap and the standard NetHack 3.7.0 rules apply.

Each level of MC offers a higher minimum that you should expect to maintain. This minimum is not absolute however, there is an additional role (1 in MCx2) to determine if some damage will pass through.
* MC1: Item enchantments will not usually go below +2
* MC2: Item enchantments will not usually go below +4
* MC3: Item enchantments will not usually go below +6

* MC1: Items have a 1 in 2 chance to avoid blanking
* MC2: Items have a 2 in 3 chance to avoid blanking
* MC3: Items have a 5 in 6 chance to avoid blanking

### Gaze attack protection
* Displacement protects from gaze attacks, only letting 1 in 3 gaze attacks find the player
* Invisibility protects from gaze attacks, only letting 1 in 3 gaze attacks find the player
* Darkness offers protection from gaze attacks (as long as the player is on a dark square and the gazer doesn't have infravision and the player is infravisible).
* If a gazer is in melee range, it will bypass invisibility and darkness protection.
* Hallucination always protects against floating eye gaze.
* Hallucination negates all incoming gaze attacks, except Medusa's glare (xNetHack).

### Slow digestion nerf
* Slow digestion now functions in a fashion opposite of the ring of hunger.
* Slow digestion only prevents hunger for 1 in every 2 turns
* The previous Vanilla behavior slowed hunger to only occur 1 in 20 turns

### Stealth changes
* To bring back the feeling of the 3.4.3 **stealth** mechanic, the chance of sleeping monsters waking up and growling has been lowered dramatically and is based on luck.
  * 0 Luck: 12.5% chance of a monster screaming when roused.
  * 2+ Luck: 0.3% chance
  * Negative luck has at least a 30% chance of rousing monsters.

### Flying Changes
* You cannot be Fast or Very Fast while levitating.
* You cannot be Very Fast while flying.
* Stomping boots and Jumping boots block flying.
* Extrinsic fumbling blocks flying (from boots or gloves)
* You cannot jump while flying.
* Items that grant **steadfastness** will do so even if the hero is flying or levitating.

### Aggravate Monster changes
* Cannibalism causes aggravation for 10-15k turns instead of permanently.
* Eating domestic animals causes aggravation for 5000-7500 turns instead of permanently.
* Intrinsic aggravate monster increases monster difficulty by 5 (stacks with extrinsic).
* Aggravate monster spell cast at hero causes intrinsic aggravation for 50-300 turns.
* Aggravate monster causes monsters not to be scared of musical instruments.
* Having the Aggravate Monster property lets monsters track you.
* Ring of aggravate monster causes pets to attack anything without fear.
* Note: The ring of aggravate monster increases the monster generation difficulty by 15 (this was already implemented in NetHack 3.7, but it's worth including here as a recent change)
* Carrying foulstones also confers aggravate monster

### Impaired Actions
* Allow #terrain whilst impaired (xNetHack)
* Falling downstairs does more damage: 10-19 instead of 1d3. (K-Mod with higher damage)
* Falling down a hole or pit whilst fumbling (or low dex) can make you fall on a wielded weapon.
* Going downstairs whilst stunned always results in falling, confusion sometimes does.
* Don't allow stunned jumping. Confused jumping has a 20% chance to fail (EvilHack)
* Many item actions are now forbidden if you have both hands welded.
* If you (or a monster) are stuck in a pit, the range of wand zaps and thrown items is limited to the  squares adjacent to the pit.
* Hallucination affects all item descriptions and appearances in and outside of your inventory (SLASH'EM)
* Auto-pickup is automatically disabled whilst hallucinating.
* You will always hit monsters who are holding you.
* No multishot when **fumbling**

## MECHANICS CHANGES

### Instakills
* It is no longer possible to be insta-petrified by touching footrice or their corpses.
* Bardiches are a new, but rare, source of instadeath. They have a 1 in 100 chance of beheading a monster or you on hit.
* Magic resistance and half-spell damage offers some protection from self-zapped wands of death (or the finger of death spell).

### Wishing
**Wands vs scrolls:**
* Wands of wishing have been replaced by one-use scrolls of wishing. Whenever a WoW would generate, a scroll will instead generate in its place.
* Scrolls of wishing do not generate randomly.
* The wand of wishing in the Castle has been replaced by a scroll of wishing.
* There are now guaranteed scrolls of wishing located at the Castle, Vlad's Tower, The Wizard's Tower, and Moloch's Sanctum.

**Wishing restrictions and effects:**
* Quest artifacts cannot be wished for (dNetHack)
* Attempting to wish for quest artifacts doesn't use up a wish
* Artifact wishes only care about previous **successful** artiwishes.
* Wishes no longer increase prayer timeout (Dynahack)
* Wishing with bad luck causes amnesia.

**The chance of receiving the artifact from a wish is:**

    1 in [number of previous artifact wishes + 1].

  * Artifact wish #1: 1 in 1 chance of success (100%)
  * Artifact wish #2: 1 in 2 chance of success (50%)
  * Artifact wish #3: 1 in 3 chance of success (33%)
  * And so on.

**How wishes have been suppressed:**
* Wishes from thrones are much more rare. The chance of getting a wish from sitting on a throne is now about 1.5%. Whenever a player hits the 1 in 13 chance to get a wish and they don't, they lose 1 point of Luck (this roughly translates to a 6% chance of losing luck anytime you sit on a throne). Once the player is granted a wish from a throne, the throne is guaranteed to disappear (from EvilHack with adjustments).
* Diluted smoky potions no longer can spawn djinnis
* The odds for fountain wishes has been inverted: they are more likely *the deeper* you are instead of the closer you are to the dungeon entry.
* The lighting shops in Minetown no longer can offer magic lamps, instead they offer magic candles (which are not capable of granting wishes)

**There are a few new sources of wishes:**
* Using the Deck of Fate can result in a wish if you draw The World card. The deck is then used up.
* If you zap a wand of wonder and trigger the wishing effect (and pass a 1 in 100 roll), you can get a wish. The odds of getting a wish on any given zap are (1/28) * (1/100) for 1 in 2800 per zap.

### Genocide has been nerfed and renamed to Exile
* A renaming was in order because genocide was heavily nerfed and functions differently from vanilla NetHack.
* Permanent dungeon-wide monster genocides are no longer allowed.
* An uncursed scroll of exile works to wipe out a single species of monster that is in close proximity to the player.
* A blessed scroll of exile wipes out a single species on the level.
* All other effects are identical to the scroll of genocide in vanilla.
* Genocides from thrones have been replaced with a generous gift of gold.

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

### Pet behavior
#### Pet Theft
* Pet theft from shops has been totally nerfed.
* Pets will never pick up objects in shops nor eat unpaid food (Gnoll)
* On the flip side - pets will also never take items from outside shops and drop them inside (like your pick-axe that you always have to leave right outside the door)
* You also cannot #loot items to/from your pet that are unpaid.
* Shopkeepers start with more gold, usually more than double the standard amounts (gnoll)

#### Pets are limited by charisma
* Your maximum number of pets is normally (CHA / 3). If you get more pets than that, they will be untamed starting with the weakest first (EvilHack)

* Ported from EvilHack with modifications
* The number of pets you can have on a level is now capped at Charisma divided by 3.
* For example, if your charisma is only 7, you can keep 2 pets, at 9 charisma you can keep 3 pets.
* However, if you exceed this limit, your weakest pets (based on level) will be the first to become untamed, with ties resolved randomly.
* Untamed pets that were previously mistreated, such as resurrected ones, may even turn hostile.
* Your steed, whilst counting toward your pet limit, will never become untamed.
* Summoned spell beings do not count toward the total pet limit.
* Since the minimum CHA possible is 3, you should always be capable of retaining a pet.

**Misc pet changes:**
* Steeds are more aggressive - if your steed has a tameness level of 15 or more, it will actively attack monsters instead of merely reacting to being attacked (EvilHack)
* Chaotics do not get alignment penalties for casting healing at pets (xNetHack)
* Restrict pets from blowing you up via gas spore, so they won't attack one whilst you are adjacent (xNetHack)
* Pets never displace player from stairs when entering a level (Dynahack).
* Pets' items can be managed with #loot
* We can also see if pets are stunned, confused, or blinded on farlook.
* Pets will use items more intelligently (EvilHack). Many extensions to the pet AI were implemented that help them value armor, weapons, and items so they use the best equipment possible.
* Tame pets will not hide or conceal themselves.
* Pets will hesitate to attack grung unless resistant to the passive.
* Pets can help the player other than fighting under certain circumstances.
* Pets are more likely to nudge you awake if you have treats in open inventory.

### Price Identification Nerf
This change destroys price identification and conforms most potions, scrolls, wands, and rings to the same price (SLEX).

* All rings cost $200
* All potions cost $200
* All wands cost $200
* All scrolls cost $200

Exceptions:
* cursed or blessed potions of water still cost $100
* Potions of blood, milk, and healing cost $100
* Scrolls of identify and knowledge cost $100
* Cards of zapping still cost $50. These only spawn in games for cartomancers.

### Polymorphing Objects and Polypiling
* The number of items you have polymorphed can be viewed in #conduct
* Non-magical potions, scrolls, spellbooks, and wands are much less likely to transform into magical items. These items only have a 1% chance of transforming into something magical. This is now comparable to other non-magical items polymorphing into magical. (dNetHack)
* The chances of getting a golem from polypiling have been increased (K-Mod/Sporkhack)
* The enchantment level or charges can be randomly reduced on polymorphed objects (Sporkhack)
* Golems created from polypiling immediately halt the polypiling process. This effectively nerfs the "one-giant-pile" strategy of polypiling.

### Poly-Self
* Players can use gaze attacks in melee range when polymorphed into monsters with a gaze attack.
* Humanoids are more careful about attacking you when you are a dangerous polyform.
* Mind flayers won't purposely to eat the brains of petrifying monsters (ie: when you are polymorphed into a cockatrice)
* When you polymorph into a 'nolimbs' monster, you are able to slip out of a ball & chain (EvilHack)
* Escape from controlled polymorph prompt no longer causes random poly (xNetHack).
* Polymorphing into a horned monster destroys flimsy or cloth helms.
* Being polymorphed into a wandering form will sometimes make you wander.
* Being polyd into a vampire bat doesn't cause stunning.

### Elbereth and Scare Monster
* Conflict negates Elbereth and scare monster protection (EvilHack)
* Engraving Elbereth no longer exercises wisdom (Fourk).
* You can't dust engrave whilst being held by a monster.
* You can't dust engrave on bloody or grassy tiles.
* You don't waste turns for aborted engrave attempts.

**Reverted 82f0b1e8e**
* The previous behavior implemented in 3.7.0 was "Scared hostile monster which cannot move away will attack."
* This has been reverted so players will be able to stand on scrolls of scare monster or Elbereth without risk of random melee attacks from scared or fleeing monsters.
* The reason for this is that it violates the classic, expected behavior of Elbereth. There are other nerfs to Elbereth and scare-monster that take the place of this.

### New Grease Effects
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
* Greased gloves cause Glib.
* Greased feet/boots cause fumbling.
* If you try to take off greased boots or any boots while you have greasy feet, you become Glib for a short time.
* Greased rings slip off your fingers as if you had greasy fingers.

### DEMON AND DEMON LAIR CHANGES
* Demonic bribes are much more expensive.
* Juiblex buffs.
* Geryon buffs (EvilHack).
* Increase speed of Baalzebub.

### Endgame Changes
* Occasional earthquakes can occur during the ascension run (UnNetHack/EvilHack). These will cease after entering the planes.
* After the invocation (and whilst traversing through Gehennom), monsters will flood from the upstairs (UnNetHack/EvilHack)
* The identity of the Riders hidden via farlook (UnNetHack)
* The correct temple on the Astral Plane will not be revealed due to fleeing monsters (UnNetHack)
* Replaced undead on Astral Plane with random A (xNetHack).
* Wizard harassment (after initially killing the Wizard of Yendor) has been increased by 20-25%
* Some monsters on the Astral Plane spawn with rings of slow digestion or teleport control to thwart "purple rain" and teleportation strategies.
* Level-teleporting (or branchporting) in hell causes major pain. The levelport will still succeed as normal, but costs a large fraction of the hero's HP and energy. It also drains the max of both (up to 1d3 each). To be fair, the player is warned before this happens and can abort the teleport. This also includes the Wizard's Tower and Vlad's Tower. **Teleport pain goes away once you've killed the Wizard of Yendor.**
* Amulet of Yendor needs only be carried to hint of nearby portals (Sporkhack).
* Allow performing the invocation whilst hallucinating.
* If you cause conflict on the astral plane, double the normal quantity of hostile angels can now appear
* Confused scrolls of gold detection no longer detect magic portals - however, the Amulet of Yendor does not require wearing to give hints when portals are nearby.


### Farming Nerfs

A big philosophy of NerfHack is to discourage repetitive and potentially infinite strategies and exploits. These specific nerfs also are aimed at encouraging using "found items" and prodding the player deeper into the dungeon.

* **Vault guard farming:** Vault guards don't get special offensive or defensive items on spawn and don't leave death drops.
* **Temple ghost farming:** All abandoned temples only spawn one ghost and then lose their status as a temple.
* **Quest monster/giant farming:** This is mostly in regard to what is known as "giant farming" in the valkyrie quest. Players could possibly farm giants for strength and gems by subsisting on their corpses. Monster generation in quests is now dramatically less frequent.
* **Werefoo farming:** Werefoo summon temporary spell-beings that don't leave death drops or corpses.
* **Horn of plenty farming:** Historically, horns of plenty could be endlessly recharged using the tourist's quest artifact, the Platinum Yendorian Express Card. However, this exploit has been nerfed to align with the restrictions on recharging tools, similar to the limitations imposed on wands.
* **Trees on special levels are pre-looted.** This doesn't fit into the classic "infinite" farming category, but because many levels have been modified to feature copious amounts of trees, a player could farm them all for bees and fruits.
* **Death drops decrease as games get longer:** For every 5000 turns that has passed, the chance of a death drop does down by 1. This is a nerf to slowly starve players out and to reduce inventory bloat toward the end of a game. It's also a good reason to play fast. The chance of a death drop is traditionally 1 in 6. So, at 5k turns it would decrease to 1 in 7, at 10k turns it goes to 1 in 8 and so on.


### Underwater mechanics
* Prevent kicking monsters out of water while underwater or vice versa.
* The hero and other monsters resist splash, spore, and fire effects while underwater.
* Being underwater provides immunity from explosions and fire damage.


## AC nerfs & buffs


### Dexterity affects AC
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

### Encumbrance affects AC
* Being encumbered has a severe negative effect on your AC and inflicts +4AC for each level of encumbrance.

| Encumbrance | AC change |
| ----------- | --------- |
| Burdened    | +4        |
| Stressed    | +8        |
| Strained    | +12       |
| Overtaxed   | +16       |
| Overloaded  | +20       |

* **The "wounded legs" status** also inflicts a severe AC penalty for bearing weight. You get +1AC for every 100aum you are carrying whilst you are wounded. Many traps can cause this condition, but now the jungle boots can be useful to prevent it.


## SKILLS AND EXPERIENCE


### Skill Changes
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

* 1-damage hits train weapon/unarmed skills (Dynahack)
* Riding skill is exercised more quickly, closer to vanilla (UnNetHack)
* Skill gain for spells is faster than skill gain for weapons (UnNetHack)
* Shield skill gains are also quadrupled to keep pace with the increased skill requirements.
* Training skill in pick-axe affects how fast you can dig (EvilHack)
    * Skilled gives you the same bonus as a dwarf (x2)
    * Expert gives you double the bonus of a dwarf (x4)

### Shield Skill
* Ported from EvilHack with some modifications
* Shield skill can be trained up like any other weapon attack. It is not actively trained, but passively as you block attacks with your shield. Sometimes you will train even if not directly shielding. There's a 2 in 3 chance of training shield skill whilst wearing one and a regular miss event occurs. A further check is rolled against the enchantment of the shield, with a higher enchantment resulting in more chance of training.
* Different roles can reach different levels of shield skill.
* As a player levels up with shield, there is also a small chance of shield bashing when attacking a monster.

#### Effects at different skill levels:
* Unskilled:  No AC bonus
* Basic:      Grants -1AC, 1 in 25 chance of shield bash
* Skilled:    Grants -3AC, 1 in 17 chance of shield bash
* Expert:     Grants -5AC, 1 in 13 chance of shield bash
* Master:     Grants -8AC, 1 in 10 chance of shield bash

* Knights and valkyries start at basic skill.
* Small shields and antimagic shields deal 1-3 damage
* Tower shields deal 2 - 13 damage
* All other shields deal 2 - 7 damage
* If you are expert or greater in shield skill, you deal an extra d4 damage.


### Experience Curve Changes
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

### Leveling up bonuses
Leveling up grants damage bonuses (SlashTHEM)
    * Level 10, +1 damage to attacks.
    * level 20+: +d(x), where x is 1 damage for every additional level gained.
    * For example: At level 25, you would get a combined total of +d6+1 damage (+1 for reaching XP 10 and +6 for levels 20-25).

### To-hit bonuses and penalties
A lot of changes have been introduced to reign back the bonuses for to-hit because in vanilla NetHack, its not uncommon to have nearly a 100% hit rate by the mid or late game.

* Strength doesn't affect to-hit calculations.
* The effect Luck has on to-hit bonuses has been reduced to (Luck / 3) (EvilHack/Sporkhack)
* Luck still has an effect when -1, -2, +1, and +2 (xNetHack)
* Players get an additional +1 to-hit bonus whilst XP1-5.
*Players get a to-hit bonus after reaching level 20 (from EvilHack with adjustments)
    * Level 22: +1 to-hit
    * Level 24: +d2 to-hit
    * Level 26: +d3 to-hit, and so on.
* Weapon enchantments give variable to-hit bonus instead of flat bonus.
* The enchantment based to-hit bonus for projectiles capped at +7.
* All short swords get +1 to-hit (Dynahack)
* You get a +4 to-hit bonus for attacking with a scimitar on a steed.
* **Polearms** get a +4 to-hit bonus vs horses and centaurs.
* fencing gloves provide +2 to-hit when you are attacking with a free off-hand (dNetHack)
* gauntlets of dexterity grant +1 to-hit whilst using bows (EvilHack)
* gauntlets of fumbling grant -9 to-hit penalty whilst using bows (EvilHack)
* combat boots provide 1AC and +1 to-hit (dNetHack)
* You have an increased wand to-hit chance for high-dex characters  (SpliceHack)


## ITEM CHANGES


* Levels of erosion on an item can affect its price (EvilHack).
* orcish equipment usually generates rusty and/or corroded
* dwarvish items sometimes spawn as fixed.
* Towels cannot be worn over the eyes - blindfolds now must be relied upon for blinding.
* Wet towels provide 100% protection from poison gas when worn.
* Scrolls, rings, and wands have a variety of new appearances (UnNetHack/Slice)

### Item Erosion and Destruction
* Objects can be completely destroyed via rusting/rotting/corroding (EvilHack)
* Almost all items are erodible/destroyable (EvilHack) - amulets, rings, wands, and tools are now eligible for erosion and destruction.
* Silver items can also corrode (xNetHack)
* The iron ball and chain cannot be destroyed from rusting (EvilHack)
* Poison gas clouds can rot organic armor
* Extrinsic poison resistance protects items from rotting in poison gas
* Monsters can wear down and destroy any armor with the destroy armor spell except crystal plate mail (EvilHack)
* Scrolls can burn up when hitting hot ground in Gehennom. (3.7 introduced potions being shattered when dropping on hot ground - this just takes it a step further.)
* Getting hit by potions of acid can corrode armor. Monster acid attacks and spit also corrode armor.
* Passive acid attacks corrodes armor more often.
* Thrown potions of acid can corrode items or armor when they hit a monster or the player.
* Water damage may disintegrate scrolls; may occur when dipping (Dynahack)
* Disintegration rays can vaporize boulders
* Items can be erodeproofed via confused enchant weapon scrolls or by dipping into non-diluted potions of reflection.
* Item erosion and negative enchantment can be repaired by dipping into a non-diluted potion of restore ability; the read counters on spellbooks can also be refreshed (xNetHack)

#### Fragile items are more vulnerable
* Beams of force bolt and striking can break fragile items in inventory.
* Knockback attacks can also shatter fragile items in inventories.
* Fragile items can be fixed to avoid destruction (note that although mirrors can be tempered, they are still subject to shattering when reflecting rays)
* Wands of striking and rings of shock resistance are immune from impact damage.
* Extrinsic shock resistance protects fragile items in your inventory from physical damage when worn.

#### Bones files trimming
* When bones files are left, a random selection of items are subject to shuddering.
* Items that grant wishes will be converted to non-magical equivalents.
* Magic markers are converted to athames.
* Quest artifacts cannot be left in bones, they revert to ordinary objects.

### Anti-magical items resist being enchanted (from SpliceHack)
* If an item grants magic resistance, it will resist scrolls of enchant weapon and enchant armor.
* The resistance is not absolute.
* Gray dragon scales can always be converted to dragon scaled armor.

**For enchant armor:**

| Current enchantment | Chance of failure |
| ------------------- | ----------------- |
| +0                  | 0%                |
| +1                  | 14%               |
| +2                  | 29%               |
| +3                  | 43%               |
| +4                  | 57%               |

**For enchant weapon:**

| Current enchantment | Chance of failure |
| ------------------- | ----------------- |
| +0                  | 0%                |
| +1                  | 8%                |
| +2                  | 15%               |
| +3                  | 23%               |
| +4                  | 31%               |
| +5                  | 38%               |
| +6                  | 46%               |
| +7                  | 54%               |
| +8                  | 62%               |
| +9                  | 69%               |
| +10                 | 77%               |
| +11                 | 85%               |
| +12                 | 92%               |


### Weapon changes
#### Higher max weapon enchantment
* Weapons can be enchanted much higher, with a soft limit of +12.
* This means that the new "+5" is "+12", and +13 is easily attainable by reading a blessed scroll of enchant weapon with a +12 weapon.
* After +6, enchant weapon scrolls will only add +1 to a weapon.
* To compensate, weapon enchantment gives variable to-hit bonus instead of flat bonus. This means that instead of a +7 weapon granting +7 to-hit, it grants a random to-hit bonus from +1 to +7, inclusive.
* Random weapons have a small chance to generate with very high enchantment.
* Lords, princes, and uniques will also appear with much higher enchantment on their weapons.
* Beware, over-enchanted weapons that vaporize now explode.
* Your wisdom is abused whenever you over-enchant and destroy weapons.
* Kicking edged weapons with bare feet or non-metal boots is painful.


#### Misc weapon changes

* Cursed launchers always have a chance of misfiring.
* Cursed projectiles can hit yourself in the leg (EvilHack).
* Any slashing or piercing weapons can now be poisoned (SLASH'EM)

* Reduced probability of long swords generating (K-Mod)
* Increased probability of boomerangs
* Increased weight of war hammers to 120.
* Reduced weight of morning star to 50.
* Reduced weight of bullwhips to 7 aum
* Increased weight of shuriken to 2 aum each.
* Wielded polearms grant an AC bonus depending on their weight (for every 30aum, they grant -1AC)
* **Spears** at expert skill can skewer through enemies, allowing you to hit the enemy directly behind the target. Peacefuls are prevented from being hit unless the spear is cursed. We also won't auto-skewer the spot unless it is visible or spottable via ESP. Skewering doesn't trigger most passive attacks unless it's a passive electrifying attack and you attack with a metal spear. Most of the time you won't get a skewer unless the monster is below 20% of it's health, otherwise if it's a kebabable monster or a solid or blobby monster, you'll always be able to skewer.
* **Tridents** at basic can also skewer monsters.
* **Spetums** can skewer up to 3 monsters when used in melee whilst riding a steed
* **Ranseurs** can disarm monsters or the player when pounded or used in melee whilst riding a steed.
* **Bardiches (long poleaxes)** have a 1 in 100 chance of beheading monsters (or the player)
* Wielding and unwielding **curved swords** takes 0 turns.
* **Morning stars and flails** can stun monsters (or the player) on critical hits. Player must be skilled or better.
* Special weapon effects (like rogue backstab, flail stunning, and samurai katana weapon smashing) have been enabled when two-weaponing.
* **Crossbows** no longer grant multishot, instead their damage output is multiplied by your skill (dNetHack). Crossbow bolts have been buffed to deal 1d7+1 versus small and 1d8+1 vs large monsters with a +2 to-hit bonus.
* **Boomerangs** will can pass through enemies on hit.
* **Polearms** can be used to trigger traps (Fourk).
* **Polearms and lances** can be pounded when blind (as long as you can sense the target)
* **Daggers and knives** have a small chance to mulch. If non-cursed, the probability is 1 in 100. If cursed, they go through the same checks as other mulchable projectiles.
* **Bows and crossbows** are two-handed.
* Ported the modified version of L's Bullwhip Patch (xNetHack).
* **All *launchers* can contribute to missile projectile damage** (adapted from SpliceHack); the damage is calculated as d(x/3), where x is the current enchantment of the launcher.
* **war hammers** have been changed from a one-handed weapon into a competitive two-handed weapon (xNetHack). They now deal 2d6 vs small monsters and 2d8 vs large

#### Slings
* Projectiles receive a strength bonus when using slings (xNetHack). However, this bonus is 3/4'th what is normally granted.
* Gem class projectiles do minimal damage vs thick-skinned monsters or unsolid monsters.
* Launching gem class projectiles from slings has the potential to instakill H

### Armor changes
* reduced weight of most armors by 50 aum (K-Mod)
* reduced weight of elvish gear by about 1/3'rd (EvilHack)
* reduced weight of dwarvish shields to 75
* kicking boots supersede thick_skinned monster or burdened status (SpliceHack)
* mud boots provide protection from wrapping attacks
* hiking boots let you avoid pit traps
* hiking boots provide extra carrying capacity (dNetHack)
* old gloves are immune to erosion damage (dNetHack)
* padded gloves provide an extra point of AC (dNetHack)
* leather gloves provide 0AC (NetHack Brass)
* combat boots provide 1AC and +1 to-hit (dNetHack)
* jungle boots provide protection from wounded legs (dNetHack)
* kicking boots allow kicking even when your legs are wounded
* oilskin cloaks let you slip effortlessly out of web traps
* increased weight of dwarvish mithril coats to 200 aum
* dwarvish and elvish mithril coats only grant MC1
* increased weight of dragon scales to 80 aum
* mummy wrappings always generate rotted
* mummy wrappings grant 0MC
* cursed armor weighs more when worn
* **the protective effect of hard helmets** has been reduced when heavy objects fall on the hero's head.
* only elves can safely enchant elvish armor over +3 - other races will get a warning vibration once their armor passes +3.
* worn armor has a 25% weight reduction (xNetHack/FIQ)
* plate mail now grants 8AC
* crystal plate mail now weighs 200, is gemstone, resists destruction, but only grants 5AC
* bronze plate mail now grants 7AC
* leather armor and studded leather armor don't grant any MC but weigh much less
* leather cloaks grant 1AC and 0MC

#### New armor type: bracers

Bracers also occupy the shield slot (EvilHack).

This implementation mostly follows EvilHack's, just adapted to 3.7 and with new types of bracers.

Bracers weigh 15 (half as much as a small shield). They allow the use of weapons while worn and don't impede spellcasting or martial arts. However, to balance them out so that shields are not rendered obsolete, they grant 0AC. They still benefit from shield skill, but the rate is only 1AC per skill. So basic = 1AC, skilled = 2AC, etc.

Elves and centaurs can spawn with bracers.

#### New dragon armor system: DSM replaced by scaled armor

Ported from xNetHack's implementation. The following text was revised from xNetHack
commit 00fec37778:

This proposal, referred to as the "dtsund-DSM" system, developed by dtsund and jonadab, introduces a significant change to how dragon scales are used in the game. Instead of dragon scale mail being its own type of armor, players can now incorporate dragon scales into existing armors—such as leather armor, chain mail, and others. These "scaled" armors provide the same extrinsic benefits as traditional dragon scale mail whilst retaining their original properties.

**Motivation for the Change**
The primary reason for replacing dragon scale mail with this system is to enhance armor strategy. Dragon scale mail was overwhelmingly optimal, rendering other armor choices irrelevant. It was simultaneously:
- **Lightweight**,
- **Higher in base AC** than any other armor,
- **Naturally erodeproof**,
- **Unrestrictive for spellcasting**,
- **Easily obtainable** before the Castle or Quest, often as an early wish, and
- **A source of powerful extrinsics** (e.g., reflection, magic resistance).

Once dragon scale mail became available, there was little incentive to consider other armors. With this new system, players must weigh the pros and cons of different base armors, making armor strategy relevant beyond defeating the first few dragons.

**Benefits of the New System**
This approach aligns with the philosophy of prioritizing found items over wished ones. Previously, even excellent armors like mithril chain mail would only serve as placeholders until dragon scale mail became available. Now, players can find dragon scales, integrate them into their chosen armor, and continue using it throughout the game.

**Key Details**
- Dragon scales provide +3 AC when used as a cloak and add +3 AC to any scaled armor.
- Scaled armor is **not automatically erodeproof**, maintaining the risk of erosion into the mid-game. Players can still erodeproof their armor or attach scales to naturally erodeproof materials.
- Following the system used in NethackFourk, if a player polymorphs and merges with their scaled armor, it will return after unpolymorphing. This is an intentional buff, ensuring that players do not lose enchantments or scales.
- **Potions of phasing** can also be used to graft dragon scales onto armor.

**Other dragon scale notes:**
* Dragon scales now weigh 80.
* Shopkeepers price dragon-scaled armor at a high value (xNetHack).
* When wishing for dragon scales, any specified enchantment is nullified to +0 (xNetHack)
* Dragon scales do not provide secondary intrinsics, they must be enchanted into scale-mail for the secondary effect to kick in.

| Dragon     | Scales confer      | Scaled armor confers       |
| ---------- | ------------------ | -------------------------- |
| gray       | magic resistance   |                            |
| gold       | light source       | hallucination resistance   |
| silver     | reflection         | blinding resistance        |
| shimmering | displacement       | stun resistance            |
| red        | fire resistance    | increase damage            |
| white      | cold resistance    | slow digest/water walk     |
| orange     | sleep resistance   | free action                |
| black      | disintegration res | drain/withering res        |
| blue       | shock resistance   | speed                      |
| green      | poison resistance  | regeneration, sickness res |
| yellow     | acid resistance    | petrification res          |

* Red dragon scaled armor confers increase damage; enchantment works in the same fashion as a ring of increase damage.

### Comestibles
* Port the Oily Corpses Patch (xNetHack)
* Blessed food items are rotten much less often
* Eucalyptus leaves can never be rotten unless cursed
* Zapping eggs with cancellation sterilizes them (HackEM)
* Cursed food items will no longer tame or pacify monsters
* Recolor royal jelly to magenta (EvilHack/xNetHack)
* Nutrition tweaks and messages for lembas and cram (EvilHack)
* Bump up fried tin nutrition and add stale tins (xNetHack)

### Potions and alchemy
* Potions can shatter when dropped on cold floors
* Potions of acid are immune to freezing (xNetHack)
* Potions of restore ability can be alchemized
* Potions of restore ability can be quaffed to cure wounded legs
* Potions of gain energy grant a lot more energy and get an alchemy recipe (xNetHack).
* Potions of holy water can cure withering status.
* Cursed potions of gain ability now subtract 1 point from a random status, adding it to a different status (xNetHack)
* Cursed potions of gain level can be used in Sokoban to bypass a floor (xNetHack)
* Blessed restore ability only restores a few levels (EvilHack)
* Dipping an eroded item in non-diluted restore ability repairs the erosion (xNetHack)
* Dipping worn dragon scales into a potion of phasing works the same as reading a scroll of enchant armor.
* Dipping in non-diluted potions of reflection erodeproofs an item.
* Dipping water into any potion will simply dilute the other potion (SLASH'EM)
* Dipping into a cursed potion always causes an explosion (SLASH'EM).
* Dipping acid into toilets explodes and destroys the toilet.
* Dipping a unicorn horn into a potion of acid will dissolve the horn, alchemizing it into a potion of healing.
* Dipping scrolls of amnesia blanks non-water non-polymorph potions.
* Mixing oil with water always results in diluted oil.
* More potion breathing effects (xNetHack)
* Thrown potions of hallucination confuse monsters (EvilHack)
* Potion of paralysis lasts 3-24 turns on monsters and has less effect when diluted (EvilHack)
* Non-magical alchemy is less likely to result in an alchemical explosion (1 in 20 chance instead of 1 in 10)
* HP gains from healing potions are subject to nurse dancing limits, but the limit is always observed as if the players level is maxed out at 30.
* Fizzy potions and booze can cause loud belches.
* Smoky potions cannot appear in any starting role's inventory.

#### Diluted potion effects
* Potions can sometimes generate diluted in the dungeon or in monster inventory.
* Most potions have a much less potent effect when diluted (EvilHack)
* Shopkeepers only offer 1/2 price for diluted potions.
* Diluted healing potions heal less and grant less max-HP (EvilHack).
* Vampire blood doesn't provide HP gains if diluted.
* Diluted smoky potions will never yield a djinni from a bottle.
* Diluted milky potions never yield ghosts.
* Cursed diluted potions of gain level don't transport you, they levitate you momentarily.
* Diluted potions of gain ability can only achieve uncursed results.

#### Gem Alchemy
* Ported from UnNetHack, originally from SLASH'EM.
* This allows you to dip a gem into a potion of acid, to alchemize a potion with a specific appearance.
* Gem alchemy recipes can be viewed in the object lookup entry for "potion of acid", or even just "acid".
* Other potions and gems should display their respective recipes.
* Gems auto-id after successful gem alchemy.
* Gem alchemy results are usually diluted; achieving pure results improves slightly with high Luck.

### Scrolls
* Reduced probability of enchant weapon scrolls
* Decreased the probability of scrolls of identify, replaced by scrolls of knowledge
* Blank scrolls cost 50
* Buffed the effects of the scroll of light (xNetHack)
* Reversed the name of the "HACKEM MUCHE" scroll
* Cursed scrolls of remove curse will curse items
* Scrolls of "genocide" have been nerfed and renamed to "exile"
* Identified scrolls of enchant armor let you choose worn piece of armor to enchant/repair (EvilHack)
* Blessed scroll of destroy armor asks which armor to destroy (xNetHack)
* Confused cursed scroll of destroy armor prompts for armor to fix
* Confused scroll of identify gives enlightenment (xNetHack)
* Confused cursed scroll of punishment decreases god anger by 1.
* Confused scrolls of gold detection no longer detect magic portals.

### Wands
* Cursed wands have a higher chance of exploding and can backfire.
* Raise odds of a zapped cursed wand exploding to 1 in 30 (UnNetHack)
* Cursed wand backfire patch (EvilHack)
  * If a directional wand is cursed and the player zaps it, there's a 1 in 8 chance it will backfire, hitting the player instead.
* Wands will never explode when engraved with (SLASH'EM)
* Blessed and uncursed wands wrest much more often (EvilHack)
  * blessed wands wrest 1/4 of the time
  * uncursed wrest 1/6 of the time
  * cursed wands still wrest 1/8 of the time
* Wands are used up even if they fail their wresting chance (EvilHack)
* Wand of cancellation extensions
  * Monsters can zap the player with wands of cancellation
  * Being cancelled removes most temporary effects (invisibility, protection, reflection)
* Wand explosions discharge their effects in an explosion (SLASH'EM).
* Monsters zapping cursed wands have double the chance of explosions.
* You must have at least one free hand (that is not welded to a cursed item or shield) to zap a wand.
* Plastic wands can neither be broken (via apply) nor exploded by shock damage. This includes all wands made of plastic material including: "plastic", "pliable", and "green".
* Wands can sometimes generate pre-charged, especially for monsters
* Wands of polymorph appear less often and monsters never spawn with them

#### Wands of wishing
* Wands of wishing have been replaced with scrolls of wishing - please see the section on Wishes.

### Rings/Amulets
* Port FIQHack's ring initial enchantment rules
* Cursed rings burn extra nutrition when worn.
* Cursed rings can slip off your fingers when Glib.
* Rings of sustain ability protect legs from wounding.
* Rings of free action offer protection from grabbing attacks (SLASH'EM).
* Rings of conflict usually generate cursed.
* Wearing the protection from shapechangers ring wakes up shifters when they revert to their normal shape (this also applies to Werebane, since that also confers PfSC now)
* Lower chances of rings exploding during charging (Sporkhack). Rings with enchantment +3 or lower will no longer have a chance to explode when charged, and rings at -5 or lower will only explode from cursed charging

* Amulets of magical breathing are immune to water damage
* Amulets of unchanging can't be polymorphed (UnNetHack)
* Rings of sustain ability cannot be polymorphed
* Amulets of guarding are now chargeable with variable AC protection (positive or negative)
* Reduced the probability for amulets of reflection.
* Amulet of life saving will not work if the player is in nonliving form (EvilHack).
* Cursed amulets of life-saving are ineffective.

#### Eating Jewelery & Accessories
* Eating rings and amulets only confers an intrinsic for a temporary period.
* To compensate for the temporary nature of these intrinsics, the possibility of getting the property is guaranteed.
* Before, the chance of getting an intrinsic from a ring by eating it was 1 in 3. It is now 100%. The chance for an amulet by eating it was 1 in 5. It has been changed to 100%.

**Summary of revised eating effects:**
- Eating a ring now grants 750-1500 turns of it's property intrinsically.
- Eating an amulet now grants 1250-2000 turns of it's property intrinsically.
- Eating the amulet of reflection now gives intrinsic reflection for 1250-2000 turns. Previously it would not grant anything.
- Eating the amulet of flying now gives intrinsic flying for 1250-2000 turns. Previously it had no effect.
- Rings of increase damage and increase accuracy only grant (+x / 2) with a minimum of 1 for positive enchantment. So rings that are +1 through +3 only grant a permanent +1, +4 and +5 will grant a +2 permanent bonus.

### Tools
* Reduced weight of land mines to 40 aum (xNetHack)
* Reduced weight of beartraps to 50 aum (xNetHack)
* Reduced weight of pick-axe to 75 aum (SLASH'EM)
* Reduced weight of potions to 10 aum
* Increased the prices of many magical tools
* Raised price of magic marker to 500
* Raised price of magic lamp to 500 (xNetHack)
* Magic lamps are more rare, wax candles are more common
* Using eroded unlocking tools also has a chance to break
* Playing eroded musical instruments can break the instrument or fail to play
* Applying rusty stethoscopes is much less effective
* Stethoscopes don't work on undead or nonliving monsters
* Rusty tin openers can break
* Applying a cursed horn of plenty causes hunger
* Using a cursed unlocking tool has a chance to break (EvilHack)
* Credit cards may slip through a lock when cursed or hero is fumbling (xNetHack)
* Reduced crystal ball paralysis if player has free action (Dynahack)
* saddles are now twice as common (FIQHack)
* Switched the probabilities of bags of holding and oilskin sacks so bags of holding are more rare.
* Make beartraps stackable (xNetHack).
* Tools have the same recharging limits as wands and have a chance to crumble.

#### Magic markers
* Magic markers do not appear in any role's starting inventory.
* Magic markers don't spawn randomly.
* Magic markers cannot be created from polypiling
* There is a 1 in 4 chance of a magic marker being the Sokoban prize
* One Sokoban ending level has a magic marker guaranteed for a prize
* There is a chance of a magic marker being hidden in the Lost Tomb level.
* A magic marker can also be found in the Boulder Bonanza Mine's End level.

#### Unicorn horns
* Unicorn horns are now one-handed, dealing d6 vs small and d7 vs large monsters
* Cancelled unicorn horns become degraded, unusable for curing. A unihorn only becomes degraded if it's enchantment is +0, otherwise it is drained of 1 enchantment level. However, a degraded horn still has a 1 in 20 chance of success.
* Unicorn horn drops decrease as the number of unicorns killed increases.
* Since unihorns are more scarce, be careful when dipping into random potions as acid will dissolve your unihorn!
* Unicorn horns cannot be poisoned (via toilet dipping)

**Unicorn horns now reduce the timeouts of most afflications instead of outright curing.**
* For troubles that time out (not illness or vomiting), the unihorn has been nerfed so that it only reduces the timeout.
* The amount reduced depends on a few factors:
  * the base fix is 1d3 + 1
  * your skill in unicorn horn (multiplied by 2)
  * the enchantment on your unicorn horn (multiplied by 2.5)
  * if you are a healer or you hit the luck bonus, double the entire above sum
  * the **luck bonus** goes up with your luck. At 0 luck, there is a 4.2% chance, at 11 there is a 20.4% chance.
  * Add all of the following for the time out reduction roll (or "tRoll").
  * For each affliction, we roll d(tRoll) for the amount reduced.
* Regardless of any of the above, there is always a 1 in 20 chance of completely curing a condition.
* Applying a unihorn can also exercise your unihorn skill.

Historical Note: The success rate change from SLASH'EM was experimented with, but ultimately discarded in favor of the timeout nerf.

#### Mirrors confer reflection while carried
* This applies to both the player and monsters.
* While carrying a mirror in open inventory, you will benefit from reflection.
* However, whenever a mirror reflects a ray, there is about a 50% chance the mirror will shatter. If you were the originator of the ray, you will be subject to a -2 luck penalty. If monsters cause the breakage, there is no luck effect.
* Artifact mirrors like the Magic Mirror of Merlin are shatterproof and will resist destruction when reflecting any rays.
* Cracked mirrors always shatter when they reflect a ray.
* Medusa's stoning gaze always shatters mirrors that reflect her gaze.
* Beware of nymphs since they regularly carry mirrors...
* Applying a mirror to Medusa starts slow stoning instead of instapetrification.

### Gems/Stones/Rocks
* Reduced weight of flint stones to 2 aum (xNetHack/Sporkhack)
* Reduced base cost of flint stones to 1.
* Reduced weight of rocks to 4 aum
* Rocks can be broken (via apply) to produce flint stones (xNetHack). When the player breaks rocks, they enter into an occupation which continues until the rocks are used up.
* Flint stones can be struck (applied) against objects made of iron, producing sparks (fire). This can scare certain monsters away who fear fire. (Sporkhack/THEM)
* Boulders deal 1+5d4 damage instead of 1d20.
* Cursed gems count as attacks when thrown at unicorns.
* Significantly lowered the odds of luckstones generating randomly; increased the odds of other gray stones
* Unicorn gems are used up when they yield Luck.


## NEW ITEMS


| Item                          | Class     | cost | aum | Origin             | Notes                                      |
| ----------------------------- | --------- | ---- | --- | ------------------ | ------------------------------------------ |
| razor card                    | weapon    | 5    | 1   | SpliceHack         | weaker shuriken for cartomancers           |
| silver short sword            | weapon    | 50   | 36  | SLASH'EM           |                                            |
| rapier                        | weapon    | 40   | 15  | SLASH'EM           | light metal saber, erodeproof steel        |
| heavy sword                   | weapon    | 50   | 500 | NerfHack           | base item for Load Brand                   |
| scythe                        | weapon    | 10   | 120 | SpliceHack         | polearm that can be used in melee          |
| sling bullet                  | weapon    | 1    | 2   | EvilHack           | 1d6 + 1 damage                             |
| gnomish helm                  | armor     | 8    | 3   | SlashTHEM          | 1AC                                        |
| fire helmet                   | armor     | 50   | 50  | SlashTHEM          | fire res                                   |
| oilskin helm                  | armor     | 50   | 20  | EvilHack           | protection from tentacle/wrap attacks      |
| shimmering dragon scales      | armor     | 700  | 80  | Deferred           | displacement, stun res                     |
| gnomish suit                  | armor     | 40   | 50  | SlashTHEM          | 2AC                                        |
| tower shield                  | armor     | 20   | 150 | SpliceHack         | Heavy, provides 4AC                        |
| anti-magic shield             | armor     | 75   | 25  | NerfHack           | 1AC/2MC, provides MR, counters spells      |
| rogue's gloves                | armor     | 50   | 10  | SpliceHack         | Confers searching, fingerless (!)          |
| bronze gauntlets              | armor     | 30   | 20  | NerfHack           | copper, 2AC                                |
| gauntlets of swimming         | armor     | 50   | 10  | SLASH'EM           | grants swimming, protects items from water |
| gauntlets of force            | armor     | 50   | 10  | NerfHack           | stuns monsters, steadfastness              |
| gnomish boots                 | armor     | 16   | 10  | SlashTHEM          | 1AC                                        |
| orcish boots                  | armor     | 16   | 30  | EvilHack           | 1AC (+ 1AC for orcs)                       |
| dwarvish boots                | armor     | 16   | 50  | EvilHack           | 2AC - replaces iron boots                  |
| stomping boots                | armor     | 50   | 50  | SpliceHack         | Instakills tiny/small monsters, noisy      |
| freedom boots                 | armor     | 50   | 20  | NerfHack           | conveys free action                        |
| leather bracers               | armor     | 10   | 15  | NerfHack           | 0AC                                        |
| bracers of integrity          | armor     | 50   | 15  | NerfHack           | conveys dis/wither res, erodeproof         |
| bracers of sleep resistance   | armor     | 50   | 15  | NerfHack           | confers sleep res                          |
| bracers of cold resistance    | armor     | 50   | 15  | NerfHack           | confers cold res                           |
| bracers vs shapechangers      | armor     | 50   | 15  | NerfHack           | confers protection vs shapechangers        |
| bracers of unchanging         | armor     | 50   | 15  | NerfHack           | confers unchanging                         |
| bracers vs stone              | armor     | 50   | 15  | NerfHack           | confers petrification res                  |
| ring of withering             | ring      | 200  | 3   | NerfHack           | causes withering                           |
| ring of sleeping              | ring      | 200  | 3   | SLASH'EM           | causes restful sleep                       |
| ring of carrying              | ring      | 200  | 3   | xNetHack           | grants expanded carrying capacity          |
| playing card deck             | tool      | 80   | 10  | SpliceHack         | can reveal your current luck               |
| deck of fate                  | tool      | 300  | 10  | SpliceHack         | high risk, high reward!                    |
| potion of milk                | potion    | 100  | 10  | NerfHack           | cancels good and bad statuses              |
| potion of reflection          | potion    | 200  | 10  | SpliceHack         | conveys temporary reflection               |
| potion of phasing             | potion    | 200  | 10  | NerfHack           | conveys temporary phasing                  |
| potion of blood               | potion    | 100  | 10  | SLASH'EM           | nutrition for vampires                     |
| potion of vampire blood       | potion    | 200  | 10  | SLASH'EM           | nutrition/healing for vampires             |
| scroll of cloning             | scroll    | 200  | 5   | SpliceHack         | clones items or monsters                   |
| scroll of knowledge           | scroll    | 100  | 5   | SpliceHack         | learn about a random magic item            |
| scroll of flood               | scroll    | 200  | 5   | UnNetHack/xNetHack | generates water pools                      |
| scroll of zapping             | scroll    | 50   | 5   | NerfHack           | special for cartomancers                   |
| spellbook of repair           | spellbook | 300  | 45  | EvilHack           | repairs any item erosion                   |
| spellbook of fire bolt        | spellbook | 100  | 35  | HackEM             | shoots a beam of fire                      |
| spellbook of flesh-to-stone   | spellbook | 700  | 65  | NerfHack           | stones monsters                            |
| spellbook of waterproofing    | spellbook | 200  | 40  | NerfHack           | protects items from water and rust         |
| spellbook of sacred vision    | spellbook | 200  | 40  | NerfHack           | confers see invisible while active         |
| spellbook of lightning        | spellbook | 500  | 50  | SLASH'EM           |                                            |
| spellbook of poison blast     | spellbook | 500  | 55  | SLASH'EM           |                                            |
| spellbook of divine reckoning | spellbook | 800  | 70  | NerfHack           | Massive damage vs undead and demons        |
| spellbook of flame sphere     | spellbook | 200  | 40  | SLASH'EM           |                                            |
| spellbook of freeze sphere    | spellbook | 200  | 40  | SLASH'EM           |                                            |
| wand of wonder                | wand      | 200  | 7   | SpliceHack         | random wand effect                         |
| wand of identify              | wand      | 200  | 7   | SlashTHEM          | identifies items, spawns with 4-8 charges  |
| wand of poison gas            | wand      | 200  | 7   | SpliceHack         | shoots poison gas                          |
| wand of corrosion             | wand      | 200  | 7   | SpliceHack         | shoots acid rays                           |
| wand of draining              | wand      | 200  | 7   | SLASH'EM           | shoots drain life rays                     |
| healthstone                   | gem       | 60   | 10  | SLASH'EM           | affects regeneration                       |
| whetstone                     | gem       | 45   | 10  | SLASH'EM           | sharpens edged weapons                     |
| foulstone                     | gem       | 0    | 10  | NerfHack           | aggravate monster & misc effects           |
| pineapple                     | food      | 9    | 15  | SpliceHack         | can be thrown for extra damage             |
| mistletoe                     | food      | 10   | 1   | EvilHack           | can cure hallucination                     |
| pinch of catnip               | food      | 7    | 1   | SpliceHack         | can tame felines                           |
| magic candle                  | tool      | 500  | 2   | SLASH'EM           | permanent light source                     |

* Potions of reflection are immune to fire and cold damage.
* Cursed potions of reflection aggravate monster (similar to cursed potions of invisibility)
* Cursed potions of phasing removes any intrinsic phasing and resets your stats (like self polymorph)
* (!) fingerless gloves do not protect against petrification

### potions of blood and vampire blood
* Increased the nutrition for blood potions
* Reduced nutrition for diluted blood.
* Non-vampire players turning into a vampire via potion of vampire blood is not permanent (from EvilHack).

### potion of milk
Non-cursed potions of milk reliably cancel out a lot of good and bad effects:
* hallucination
* confusion
* stunning
* blindness
* protection given by spell
* reflection given by potion
* phasing given by potion
* invisibility
* see invisible
* telepathy
* milk also will un-poly a player or monster back to their original form.

Other effects:
* non-diluted milk heals 1 HP
* Cursed milk is always spoiled and causes nausea without cancelling any effects.
* Blessed milk also increases your max HP by 1.
* Monsters will also drink milk to cure stunning and confusion only.
* Dipping a poisoned item into milk unpoisons it.

### playing card deck
* When applied, gives you a poker hand which correlates to your luck.
* If the deck is blessed (or you are a cartomancer), you get a clear indication of your luck
  by using the kicker.
* If uncursed, you get a rough indication of your luck by the hand strength.
* If cursed, the meanings are reversed.
* Can be #tipped and emptied for a stack of razor cards

### scroll of cloning
* Ported from SpliceHack with modifications
* This can clone an item in your inventory or clone yourself if read whilst confused.
* Attempting to clone unique items or items that are too powerful will result in lesser quality results: magic markers, magic lamps, wands of wishing, scrolls of cloning, artifacts, and any invocation items will produce a lesser type of item.
* To copy the enchantment on an item, the scroll must be blessed.
* If the scroll is cursed, the resulting item will be cursed.
* All other properties on the item should be copied exactly as is. This enables fun tricks like cloning a +13 fixed crysknife, or that blessed figurine of an Archon you've been holding onto.
* When confused, the scroll clones the player. The resulting clone will have no inventory. A blessed scroll creates a tame clone, an uncursed scroll makes a peaceful clone, and a cursed scroll makes a hostile clone. An interesting side-effect of this is that cloning yourself reduces your current HP by half.
* If confused and the scroll is blessed, you can also clone yourself to create a powerful tame pet if you currently hold a strong polyform (ie: master mind flayer, purple worm, etc)
* Scrolls of cloning cannot be created from polypiling nor written.

**Other updates from SpliceHack:**

Unpaid items cloned in shops now become the property of the shopkeeper. Additionally, more item properties are carried over during cloning, including erosion-proofing, container status, and other miscellaneous attributes to ensure that items are genuinely cloned.

Intelligent monsters can also use these scrolls to clone themselves. When monsters read the scrolls, they are always read-as-confused, meaning they can only clone themselves. Whilst this approach might seem odd, it simplifies the system by avoiding the complexities of allowing monsters to clone items.

**Unique monsters can use these scrolls as well**, but the Wizard of Yendor must still follow the Double Trouble routine, ensuring that no more than two Rodneys can oppose you at any time. However, other unique monsters have the potential to clone themselves more than once if the opportunity arises.

### deck of fate
This tarot-based deck is very powerful and was ported from SpliceHack with some major changes. In SpliceHack, you would be prompted for how many cards to draw. This has been changed to be a mandatory draw of 5 cards, eliminating the prompt. After using the deck, it is always destroyed, allowing only one use. Because it is capable of granting wishes, the deck of fate cannot be wished for, cloned, or created from polypiling.

There are 22 different cards in the deck, each having a potentially good or bad effect. About half the cards are "good" and half "bad". There is a nudge factor that occurs if the deck is cursed or blessed.

If cursed, the drawn card's value will be lowered by one notch. This means **The World** is impossible to draw with a cursed deck since it's the highest numbered card at 22. It also doubles the chance of drawing **The Tower** since that card is number 1.

If blessed, the drawn card value is raised by one notch. This effectively doubles your chances of drawing **The World** and prevents **The Tower** from being drawn.

If no effects interfere with drawing or the BUC status of the deck, an uncursed deck has about a 24.3% chance of granting a wish and a blessed deck has a 43.5% chance. However, if you draw **Temperance**, the deck is marked as cursed for the remaining draws.

**Before you start drawing cards, your current alignment is set to -1.** Be wary of any artifacts you may wish for because an artifact blast is guaranteed - both because your alignment is negative and because artifact blasts will always occur if possible. Artifact blasts have also been increased, making early artiwishes much more dangerous.

* Unlike the playing card deck, decks of fate cannot be #tipped for razor cards, making them easy to identify.

| Card                 | Effects                                                                                                                                                                                                                             |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| The Tower            | Explosions of fire and magic blast you for 1d30 each and you are cancelled.                                                                                                                                                         |
| The Wheel of Fortune | Draw two more cards.                                                                                                                                                                                                                |
| The Devil            | If your luck is 0 or less a demon lord is summoned, otherwise a random demon appears;  cease drawing from the deck and lose 7 luck.                                                                                                 |
| The Fool             | INT and WIS are each drained by 1-3 points. Grants aggravate monster for 1500-2245 turns.                                                                                                                                           |
| Death                | If you have 7+ Luck, you may be polymorphed. Otherwise, you are subjected to the touch of death; you cease drawing from the deck in either case.                                                                                    |
| Judgment             | You are punished.                                                                                                                                                                                                                   |
| The Emperor          | Two intrinsics are drained or outright stolen (like the gremlin attack).                                                                                                                                                            |
| The Hermit           | You gain invisibility and teleportitis for 1000-1499 turns.                                                                                                                                                                         |
| The Hanged Man       | A rope golem is summoned and you lose 1 Luck.                                                                                                                                                                                       |
| Justice              | With -13 or less alignment abuse or non-positive luck, you are paralyzed for 20-49 turns and stop drawing cards. Otherwise you are unpunished. You may also receive divine protection if you have retained your original alignment. |
| Temperance           | Two worn pieces of armor are destroyed; the deck becomes cursed for the rest of the draws.                                                                                                                                          |
| The Lovers           | Two peaceful foocubi are summoned.                                                                                                                                                                                                  |
| The Magician         | If the Wizard of Yendor has been killed he is resurrected, otherwise your max energy is increased by 10-29 points.                                                                                                                  |
| Strength             | Your strength is increased.                                                                                                                                                                                                         |
| The High Priestess   | Your charisma is increased by 1 point and you gain intrinsic ESP for 1250-1999 turns                                                                                                                                                |
| The Hierophant       | Creates an altar where you are standing if the terrain is valid.                                                                                                                                                                    |
| The Empress          | Creates a throne where you are standing if the terrain is valid. Summons an Elvenqueen if you have bad Luck.                                                                                                                        |
| The Chariot          | Uncontrolled teleport on the current level.                                                                                                                                                                                         |
| The Sun              | No effect if you have changed alignments, otherwise you are granted some divine protection.                                                                                                                                         |
| The Moon             | You gain 7 luck.                                                                                                                                                                                                                    |
| The World            | Your entire inventory is identified.                                                                                                                                                                                                |
| The Star             | You are granted a wish; cease drawing from the deck.                                                                                                                                                                                |
### healthstone
* Ported from SLASH'EM with updates
* A blessed healthstone now increases your regeneration rate by 10%.
* An uncursed healthstone increases regeneration by 5%.
* A cursed healthstone decreases regeneration by 10%.
* Healthstones usually generate cursed, making them stand out a bit more among gray stones and a little easier to identify.
* Monsters carrying non-cursed healthstones also gain regeneration.

### whetstone
* Ported from SLASH'EM with updates from HackEM.
* Whetstones no longer can add positive enchantment to a weapon, they can only repair it to +0.
* Cursed whetstones either rust or corrode items.
* Blessed whetstones can uncurse a cursed weapon, but lose their blessed state in the process.
* Most of the other small quality-of-life improvements from HackEM remain.

### foulstone
Effects of carrying a foulstone:
* Causes aggravate monster (but without increasing the difficulty of spawned monsters)
* Monsters cannot digest you and you cannot digest monsters carrying one.
* Shopkeepers will not let you into their shops and won't buy it.
* If blessed, has a 1 in 100 chance each turn of emitting a stench that scares monsters for a short while (similar to garlic breath)
* If cursed, has a 1 in 100 chance each turn of emitting a poisonous cloud on your square.
* The effects can stack, so carrying multiple foulstones increases the frequency of the cursed or blessed effects.

Other effects:
* Monsters will never eat this rock and it's inedible if you are polymorphed into a monster that could eat it.
* Pets will try not to step on one (treated as a cursed item).
* If rubbed on another rock, emits a poisonous cloud.
* Foulstones always generate cursed and autocurse when dropped.
* Cursed foulstones cannot be dropped (like loadstones).

## ARTIFACT CHANGES

### General artifact changes
* Artifact weapons can now be dual-wielded (SLASH'EM)
* Intrinsics are granted for both weapons accordingly.
* Lawful and chaotic weapons cannot be two-weaponed (EvilHack)
* Artifacts always blast you if they have the chance (instead of passing a 1 in 4 roll)
* Artifacts blasts inflict much more damage (SLASH'EM)
* Cartomancers take doubled artifact blast damage.

### Specific artifact changes
* Cleaver is prevented from cleaving peaceful bystanders (unless cursed) (xNetHack)
* Excalibur will fix any negative enchantment on it when created from #dipping (xNetHack)
* Eye of the Aethiopica must be worn to grant energy regeneration and half-spell damage.
* Eyes of the Overworld protect against more gaze attacks (EvilHack)
* Eyes of the Overworld's xray-vision range was increased to 8 (from FIQHack).
* Fire Brand instakills highly flammable monsters and green slimes (xNetHack)
* Fire Brand cures sliming whenever you attack with it
* Fire Brand is now a short sword (EvilHack)
* Frost Brand instakills water elementals
* Frost Brand is now a short sword (EvilHack)
* Giantslayer is now a spear (EvilHack)
* Giantslayer conveys 18/\* strength whilst wielded (Dynahack)
* Grayswandir only deals bonus damage versus cross-aligned monsters.
* Grimtooth can inflict disease on its victims (EvilHack)
* Heart of Ahriman is now a ruby that grants slotless flying, displacement, and Luck instead of stealth (FIQHack)
* Heart of Ahriman can be invoked for a blessed remove curse effect (Fourk)
* The Longbow of Diana must be wielded to grant ESP
* Longbow of Diana confers half physical damage when wielded
* Magicbane is a quarterstaff (FIQHack)
* Magic Mirror of Merlin grants reflection and 1/2 spell damage instead of magic resistance (EvilHack).
* Mjollnir's is louder when it strikes monsters with lightning
* Mjollnir can be invoked for a lightning bolt (xNetHack)
* Ogresmasher can also hurtle light-weight monsters (EvilHack)
* Orb of Detection grants clairvoyance whilst carried.
* Sceptre of Might grants steadfastness when wielded
* Sceptre of Might gets a bonus on all monsters (this is to compensate for the difficulty in enchanting it due to its magic resistance)
* Snickersnee grants stun resistance when wielded (EvilHack)
* Staff of Aesculapius can cure withering (xNetHack/EvilHack)
* Sting actually cuts through webs when exiting a web
* Trollsbane grants regeneration whilst wielded (many variants)
* Trollsbane only needs to be carried to suppress troll revival
* Tsurugi of Muramasa has a 10% chance of bisection (SLASH'EM)
* Tsurugi of Muramasa also confers very fast speed when wielded (Fourk)
* Vorpal Blade gets a 10% chance of beheading (SLASH'EM)
* Vorpal Blade grants see invisible whilst wielded
* Vorpal Blade provides warning vs jabberwocks (EvilHack)
* Werebane provides protection from shapechangers when wielded

**Bane changes:**
* All banes provide warning vs their bane monster type when wielded (EvilHack)
* All banes glow red in response to their monster types (EvilHack)
* All banes can instakill their associated monster types with a 1 in 5 chance (UnNetHack)
* Sunsword and Disrupter don't get instakills
* Banes can't instakill unique monsters


## NEW ARTIFACTS


| Name                  | Align      | Type                  | From        | to-hit/dmg                             | Notes                                                                                                          |
| --------------------- | ---------- | --------------------- | ----------- | -------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Acidfall              | chaotic(!) | long sword            | SpliceHack  | +d5 to-hit, 2x acid dmg                | intelligent, confers acid res when wielded                                                                     |
| Amulet of Storms      | chaotic    | amulet of flying      | xNetHack    | n/a                                    | confers shock res when worn, prevents thunderstorm paralysis, pacify stormy monsters via #chat                 |
| Angelslayer           | chaotic(!) | trident               | EvilHack    | +d5 to-hit, +d10 dmg                   | bane vs angels; confers searching and 1/2 spell damage when wielded                                            |
| Blackshroud           | chaotic    | cloak of invisibility | SlashTHEM   | n/a                                    | confers warning and drain res when worn                                                                        |
| Carnwennan            | lawful     | knife                 | SpliceHack  | +d3 to-hit, +d8 dmg                    | confers searching and stealth when wielded                                                                     |
| David's Sling         | neutral    | sling                 | SlashTHEM   | +d5 to-hit, +d6 dmg                    | bane vs giants; confers 1/2 physical damage when wielded                                                       |
| Deluder               | neutral    | cloak of displacement | SLASH'EM    | n/a                                    | confers stealth and protection when worn                                                                       |
| Disrupter             | neutral    | mace                  | SLASH'EM    | +d5 to-hit, +d30 dmg vs undead         | bane vs undead                                                                                                 |
| Doomblade             | chaotic    | short sword           | SLASH'EM    | +d10 dmg, 25% chance of dmg bonus      |                                                                                                                |
| Drowsing Rod          | unaligned  | quarterstaff          | HackEM      | +d5 to-hit, +d5 sleep dmg              | first sacrifice gift for healers; confers sleep res when wielded                                               |
| Glamdring             | chaotic    | long sword            | EvilHack    | +d8 to-hit, +d10 dmg                   | bane vs orcs; confers shock res and protection when worn                                                       |
| Hellfire              | chaotic    | crossbow              | SLASH'EM    | +d5 to-hit, +d7 dmg + explosion        | confers fire res when wielded                                                                                  |
| Holographic Void Lily | chaotic(!) | credit card           | SpliceHack  | n/a                                    | energy regen, 1/2 spell dmg, and reflection when carried. #invoke for card drop boost                          |
| Load Brand            | unaligned  | heavy sword           | NerfHack    | -9 to-hit, double damage               | when wielded, confers half physical damage, steadfastness, and protection; absorbs curses.                     |
| Mayhem                | chaotic    | stomping boots        | NerfHack    | n/a                                    | confers conflict and warning against undead when worn.                                                         |
| Mirrorbright          | neutral    | shield of reflection  | SLASH'EM    | n/a                                    | confers hallucination res when worn; light source; does not impede spellcasting.                               |
| Mortality Dial        | lawful     | morning star          | SpliceHack  | +d5 to-hit, +d12 dmg                   | confers warning and regeneration when wielded; prevents monster regeneration.                                  |
| Mouser's Scalpel      | neutral    | rapier                | SLASH'EM-up | +d5 to-hit, +1 dmg; multihit bonus     | if not confused or stunned, chance of delivering extra strikes                                                 |
| Origin                | unaligned  | quarterstaff          | SpliceHack  | +d3 to-hit, +d8 dmg                    | confers telepathy and teleport control when wielded; boosts spellcasting                                       |
| Plague                | chaotic    | bow                   | SLASH'EM    | +d5 to-hit, +d7 poison dmg             | confers sickness res when wielded, poison res when carried.                                                    |
| Poseidon's trident    | chaotic    | trident               | SpliceHack  | +d3 to-hit, +d14                       | confers magical breathing when wielded; #invoke for water walking                                              |
| Pridwen               | lawful     | large shield          | SpliceHack  | n/a                                    | confers half physical damage and steadfastness when worn                                                       |
| Quick Blade           | lawful     | silver short sword    | SLASH'EM    | +d9 to-hit, +d2                        | confers speed when wielded                                                                                     |
| Serenity              | lawful(!)  | silver spear          | NerfHack    | +d3 to-hit, +d10                       | counters 80% of monster spells and blocks spellcasting; suppresses aggravate monster, berserking, and conflict |
| Serpent's Tongue      | chaotic    | dagger                | SLASH'EM    | +d2 to-hit, 2x damage + poison bonuses | always poisoned, #invoke to fling poison                                                                       |
| Skullcrusher          | lawful     | aklys                 | SLASH'EM    | +d3 to-hit, +d10 dmg                   | first sacrifice gift for cavemen                                                                               |
| Snakeskin             | Neutral    | robe                  | SlashTHEM   | n/a                                    | confers acid res and hallucination res when worn.                                                              |
| The End               | neutral    | scythe                | SpliceHack  | +d3 to-hit, +d10 dmg                   | confers drain res when wielded                                                                                 |
| The Lenses of Truth   | unaligned  | lenses                | NerfHack    | n/a                                    | confers see invisible and stun res when worn                                                                   |
| Thunderfists          | neutral    | gauntlets of force    | NerfHack    | +3 to-hit, +1d8 shock damage           | first sacrifice gift for monks; confers shock res and protection when worn                                     |
| Whisperfeet           | neutral    | speed boots           | SLASH'EM    | n/a                                    | confers stealth and luck when worn                                                                             |
| Oathfire              | lawful(!)  | leather bracers       | NerfHack    | n/a                                    | confers fire resistance and protection, protects fragile items, passive fire damage and explosions             |
| The Argent Cross      | lawful(!)  | amulet of reflection  | NerfHack    | n/a                                    | light source, half spell damage, disintegration/withering res, passive turn undead                             |
| The Glyph Shard       | unaligned  | obsidian stone        | NerfHack    | n/a                                    | #invoke to levelport to a level keyed into the stone                                                           |

(!) - Means the artifact is intelligent
Misc changes:
* Plague was changed from an orcish bow to a standard bow.
* Quick Blade is a silver short sword instead of an elvish short sword
* Blackshroud was a neutral cloak in SlashTHEM - it was changed to chaotic.
* Skullcrusher was a club in SLASH'EM, but it has been changed to an aklys.
* Wielding Origin protects from amnesia.
* Snakeskin provided a point of protection in SlashTHEM but that was removed and provides MC2 as a robe.
* Scythes are a type of polearm that can be used in melee but they have a -2 to-hit penalty.
* Mortality Dial was an executioner's mace in SpliceHack but it was changed to a morning star with higher damage. It also now grants warning.
* In NetHack 3.7.0, Grimtooth can be invoked to fling poison. However, since it was already buffed with a disease attack, this ability was moved to Serpent's Tongue.

### Load Brand
* This heavy sword was forged from load stones and weighs in at a hefty 500aum!
* Deals 3d6 vs small monsters and 3d8 vs large monsters
* -9 to-hit penalty
* Double damage
* It also confers half physical damage, steadfastness, and MC1 protection
* Similar to Magicbane, it also absorbs curses

### The Lenses of Truth
* Confers see invisible and stun resistance when worn.

### Serenity
* +d10 damage
* counters 80% of monster spells whilst wielded
* whenever it successfully counters, the caster briefly requires more time to recover and cast another spell
* blocks you from casting spells when wielded
* blocks aggravate monster and conflict
* blocks barbarian blood rage from activating if wielded
* prevents monsters from berserking

### Thunderfists
* gauntlets of force
* Grants shock resistance when worn
* Deals shock damage when used bare-handed
* When monks don these, they occasionally release a chain lightning blast
* Grants MC1

### Glyph Shard
* This powerful gem allows the player to open a portal to a specific level.
* To bind a level to the shard, simply (a)pply it on the desired level. This can only be performed once per game, so choose carefully—only one level can ever be linked.
* Rumors say a Glyph Shard lies hidden deep within the Wyrm Caves...


## NEW MONSTERS


The following summarizes the new monsters, advanced info can be found in the monster pokedex in NerfHack or on the NetHack Wiki.

| Monster                | Sym | Origin               |
| ---------------------- | --- | -------------------- |
| giant fly              | a   | SpliceHack           |
| giant cockroach        | a   | EvilHack             |
| giant praying mantis   | a   | SpliceHack           |
| bullet ant             | a   | SpliceHack           |
| locust                 | a   | EvilHack             |
| queen ant              | a   | EvilHack             |
| assassin bug           | a   | SLASH'EM             |
| migo drone             | a   | SLASH'EM             |
| migo warrior           | a   | SLASH'EM             |
| migo queen             | a   | SLASH'EM             |
| jiggling blob          | b   | SLASH'EM             |
| lava blob              | b   | SLASH'EM             |
| static blob            | b   | SLASH'EM             |
| burbling blob          | b   | SLASH'EM             |
| basilisk               | c   | EvilHack             |
| barghest               | d   | SpliceHack           |
| Cerberus               | d   | EvilHack/xNetHack    |
| revenant hound         | d   | NerfHack             |
| warg pup               | d   | NerfHack             |
| vulpenferno            | d   | SpliceHack           |
| glowing eye            | e   | SLASH'EM             |
| stinking sphere        | e   | Fourk                |
| acid sphere            | e   | SpliceHack/EvilHack  |
| third eye              | e   | SLASH'EM/YANI        |
| blinking eye           | e   | SLASH'EM             |
| kamadan                | f   | SLASH'EM             |
| weretiger              | f/@ | SLASH'EM             |
| deep one               | h   | SLASH'EM             |
| deeper one             | h   | SLASH'EM             |
| deepest one            | h   | SLASH'EM             |
| alhoon                 | h   | EvilHack             |
| dretch                 | i   | SLASH'EM             |
| rutterkin              | i   | SLASH'EM             |
| blood imp              | i   | SLASH'EM             |
| nupperibo              | i   | SLASH'EM             |
| redcap                 | i   | SpliceHack           |
| clear jelly            | j   | SLASH'EM             |
| yellow jelly           | j   | SLASH'EM             |
| orange jelly           | j   | SLASH'EM             |
| rancid jelly           | j   | SLASH'EM             |
| leper                  | l   | NerfHack             |
| killer mimic           | m   | SpliceHack           |
| pixie                  | n   | SLASH'EM             |
| spiked orc             | o   | NerfHack             |
| diamond piercer        | p   | SpliceHack           |
| god piercer            | p   | SpliceHack           |
| landshark              | q   | SpliceHack           |
| pack rat               | r   | SLASH'EM             |
| hedgehog               | r   | SpliceHack           |
| nickelpede             | s   | SLASH'EM             |
| recluse spider         | s   | SLASH'EM             |
| phase spider           | s   | SLASH'EM             |
| werespider             | s   | SLASH'EM             |
| monstrous spider       | s   | SpliceHack           |
| giant centipede        | s   | EvilHack             |
| maggot                 | w   | SLASH'EM/SpliceHack  |
| acid worm              | w   | SLASH'EM             |
| bloodworm              | w   | SLASH'EM             |
| tunnel worm            | w   | SLASH'EM             |
| rot worm               | w   | SLASH'EM             |
| spark bug              | x   | SLASH'EM             |
| arc bug                | x   | SLASH'EM             |
| lightning bug          | x   | SLASH'EM             |
| will-o'-the-wisp       | y   | SpliceHack           |
| koala                  | z   | SLASH'EM             |
| compsognathus          | z   | NerfHack             |
| velociraptor           | z   | SpliceHack           |
| t-rex                  | z   | SpliceHack           |
| dark Angel             | A   | UnNetHack            |
| movanic deva           | A   | SLASH'EM             |
| monadic deva           | A   | SLASH'EM             |
| astral deva            | A   | SLASH'EM             |
| zoo bat                | B   | SpliceHack           |
| athol                  | B   | SLASH'EM             |
| phoenix                | B   | SpliceHack           |
| byahkee                | B   | SLASH'EM             |
| nightgaunt             | B   | SLASH'EM             |
| fell beast             | D   | EvilHack             |
| baby shimmering dragon | D   | Deferred             |
| shimmering dragon      | D   | Deferred             |
| Wintercloak            | D   | NerfHack             |
| volatile mushroom      | F   | SpliceHack           |
| gray fungus            | F   | EvilHack/SlashTHEM   |
| elder minotaur         | H   | EvilHack             |
| arch-vile              | L   | NerfHack             |
| eye of fear and flame  | L   | SpliceHack           |
| worm that walks        | L   | SpliceHack           |
| adherer                | M   | SpliceHack           |
| troll mummy            | M   | SLASH'EM             |
| ha-naga                | N   | SpliceHack           |
| ogre mage              | O   | SLASH'EM             |
| shadow ogre            | O   | SLASH'EM             |
| like-like              | P   | NerfHack             |
| shoggoth               | P   | SLASH'EM             |
| orb weaver             | Q   | NerfHack             |
| alchemist              | Q   | SpliceHack           |
| cerastes               | S   | SpliceHack           |
| asphynx                | S   | SLASH'EM             |
| weresnake              | S   | SLASH'EM             |
| giant anaconda         | S   | EvilHack             |
| grave troll            | T   | SpliceHack           |
| hunger hulk            | U   | SpliceHack           |
| slumber hulk           | U   | SpliceHack           |
| umbral hulk            | U   | SlashTHEM/SpliceHack |
| water hulk             | U   | SLASH'EM             |
| gorgon hulk            | U   | NerfHack             |
| fire vampire           | U   | SLASH'EM             |
| star vampire           | U   | SLASH'EM/dnh         |
| dhampir                | V   | NerfHack             |
| vampire mage           | V   | SLASH'EM             |
| vampire king           | V   | EvilHack             |
| bodak                  | W   | SpliceHack           |
| slaughter wight        | W   | HackEM               |
| shadow                 | X   | SLASH'EM             |
| The First Evil         | X   | NerfHack             |
| ghoul mage             | Z   | SLASH'EM             |
| revenant               | Z   | EvilHack             |
| gug                    | Z   | SLASH'EM             |
| ghoul queen            | Z   | SLASH'EM             |
| elven cleric           | @   | EvilHack             |
| familiar               | @   | NerfHack             |
| lava demon             | &   | Convict Patch        |
| spined devil           | &   | SLASH'EM             |
| Cthulhu                | &   | SLASH'EM/UnNetHack   |
| weredemon              | &/d | EvilHack             |
| merfolk                | ;   | SpliceHack/SlashTHEM |
| thing from below       | ;   | SpliceHack           |
| cartomancer            | @   | SpliceHack           |
| King of Games          | @   | SpliceHack           |
| Del Zethire            | @   | SpliceHack           |
| duelist                | @   | SpliceHack           |
| undead slayer          | @   | SLASH'EM             |
| exterminator           | @   | SLASH'EM             |
| Van Helsing            | @   | SLASH'EM             |
| The Executioner        | @   | UnNetHack            |
| wax golem              | '   | SLASH'EM             |
| plastic golem          | '   | SLASH'EM             |
| grung                  | 6   | NerfHack             |
| green grung            | 6   | NerfHack             |
| blue grung             | 6   | NerfHack             |
| purple grung           | 6   | NerfHack             |
| red grung              | 6   | NerfHack             |
| orange grung           | 6   | NerfHack             |
| gold grung             | 6   | NerfHack             |
| gnoll                  | 9   | SLASH'EM             |
| gnoll warrior          | 9   | SLASH'EM             |
| gnoll chieftain        | 9   | SLASH'EM             |
| gnoll shaman           | 9   | SLASH'EM             |


### New monster notes
* all devas resist poison, fire, and shock damage
* monadic devas are breathless and accurate
* astral devas are accurate
* adherer AC was buffed from it's original AC in SpliceHack
* alhoons were covetous in EvilHack, now they move normally but faster
* alhoons can now displace monsters
* arch-viles are fast and lethal L class monsters that can cast fire pillar from a distance and revive monsters. They can also cast other clerical spells.
* assassin bugs are stronger than SLASH'EM
* athols have increased size, weight, and nutrition
* athols are now strong, berserk, flank, and have infravision
* barghests now have fire, cold, poison, drain, death resistance, and can swim.
* barghests are now vulnerable to silver
* barghests difficulty increased from 9 to 12
* barghests get an additional 1d8 fiery claw attack; their existing 2d6 bite attack now drains life.
* blinking eyes also get a passive blink that teleports attackers
* bloodworms get a drain life bite instead of poison bite
* bullet ants get an additional 2d4 cold bite.
* byahkees were recolored to yellow
* cerastes buffs: 2 poison bites, poison res, higher difficulty.
* rats are the same as Vanilla's rabid rats. They always spawn rabid.
* some deepest ones are guaranteed on the plane of water
* deep ones, deeper ones, and deepest ones have all received major buffs.
* deep/er/est ones all get regeneration, faster speed in water, are non-tameable, and not infravisible anymore.
* deeper ones resist sleep and shock.
* deepest ones resist sleep, shock, acid, and magic. They also have 100 MR.
* deeper and deepest ones get an additional hug attack.
* deeper ones and deepest ones take extra damage from blessed weapons.
* elven clerics were known as elven wizards in EvilHack
* ghoul mages are now clairvoyance
* ghoul queens can generate randomly in the dungeon
* ghoul queens are now bright magenta
* ghoul queens have -5 AC, level 16, and difficulty 21
* giant praying mantis now ignores all magical scaring
* giant praying mantis has a higher level
* glowing eyes get a passive stunning gaze
* gnolls now have '9' symbol instead of 'G' (SpliceHack)
* all gnolls get berserking instead of traitorous (EvilHack)
* all gnolls get flanking (SpliceHack)
* all gnolls resist poison, fire, sleep, draining, and sickness. They no longer hide.
* gnoll shamans gets teleport control.
* gnoll warriors get the lord tag.
* gnoll chieftains get the prince tag.
* grave trolls can spawn in graves/graveyards
* grave troll corpses cause sickness when eaten
* grave trolls are huge and have thick hides
* gugs are now orange
* jiggling blobs can jump
* kamadan are recolored to light green, can now jump, have infravision, and get some poisonous snake bites
* koalas cannot calm berserking monsters.
* rabid koalas are not capable of calming anything
* landsharks were recolored to bright blue
* lepers are generate sleeping and are fairly slow, but have a nasty disease touch.
* lepers can spawn with bells and will ring them incessantly.
* like likes can eat organic shields and cloaks when engulfing you (note: dragonhide scales are not edible for them)
* merfolk were recolored to bright green
* merfolk no longer steal items, they get more attacks and spawn with rustproof tridents or spears.
* migos explode into poison gas clouds on death and don't leave any corpses
* migos are immune to poison gas.
* migo drones and warriors are slightly lower level than in SLASH'EM.
* monstrous spiders get a stunning gaze
* nightgaunts were recolored to purple
* pack rats can generate randomly in the dungeon
* phase spiders may appear in small groups
* phase spiders can't move diagonally
* phase spiders have shock resistance
* revenants can now shoot fireballs and have fire resistance (inspired by DOOM 2)
* revenants count as zombies, so they also revive and ignore magical scaring.
* shadows have higher level, better AC, stronger attacks, are unsolid, resist shock, and can now stalk the player
* shadows have the same defense as shades (must be hit with silver or blessed weapons)
* shadow ogres spawn invisible and have a drain life attack
* spiked orcs cannot wear anything in the armor slot
* spined devils now have a passive spike attack
* star vampires are telepathic
* things from below can see invisible
* third eyes inflict a passive hallucination gaze.
* troll mummies get a withering attack
* t-rex can berserk and emit a scary roar
* velociraptors are much stronger than in SpliceHack (roughly the same strength as SLASH'EM's kangaroos)
* weretigers are recolored to red and can jump
* zoo bats now cause confusion when eaten
* rot worms are now tiny
* tunnel worms are now huge, get an armor rending attack, and a butt attack
* vampire kings get two drain life bites, a stronger weapon attack, 75MR, and cold resistance
* vampire kings can displace monsters to get to you and cannot be tamed.
* werespiders can summon giant spiders, phase spiders, and monstrous spiders
* weresnakes can summon snakes, pit vipers, and asphynxes
* weresnakes are now red
* monstrous spiders were buffed from level 8 to 12, difficulty 10 to 15, have berserk, infravision, infravisible, and MR 20
* worms that walk get an additional hug/grapple attack

**New hulk changes**:
* water hulks are also amphibious

**Passive spiking monsters:**
* This mechanic was ported over from SpliceHack and applies to hedgehogs and spiked orcs.

**Phoenix:**
* Very strong lawful monster that explodes on death
* When it dies it leaves behind a phoenix egg, which will hatch when exposed to fire or lava
* It will also hatch when attempts are made to eat it, bury it, or put it in a container
* When zapped with polymorph, a phoenix will self-explode in resistance to the change
* To prevent a phoenix from exploding or leaving an egg, you must cancel it or stone it
* To prevent a phoenix egg from hatching, you can also cancel it
* Couple of other ways permanently kill them: disintegration rays (from a black dragon) and withering away
* Lowered their MC protection from 40 to 20
* Phoenixes now resist cold
* Phoenixes have a fierce hatred toward undead and grudge them.

**Orb Weaver:**
* A brand new monster debuting in NerfHack
* This pesky spellcaster will relentlessly summon spheres of all types
* Although they can cast clerical spells, they only can cast 'summon orbs', healing spells, and protection.
* Currently, uses the transmuter's tile from SpliceHack.

## MONSTER CHANGES


### Misc monster changes
* all quest guardian colors were changed to cyan
* all A class monsters are immune to death magic (xNetHack)
* All A class monsters resist sickness.
* air elementals get shock resistance.
* Aleax difficulty raised to 16 (SLASH'EM)
* Aleax weapon attacks raised to 2d6 (Sporkhack)
* baluchitherium are now huge; have -5 AC, strengthened claw attack from 5d4 to 5d12; increased difficulty
* all bats can see invisible
* captains are considered princes (xNetHack)
* captains and watch captains generate with keys (EvilHack)
* centaurs will keep their distance from the player naturally (xNetHack)
* couatls get sleep and shock resistance (Fourk)
* couatls get a stunning gaze and can generate invisible
* deep ones and deeper ones have thick skin, matching deepest ones
* many major demons have been given flight (xNetHack)
* dingos have been replaced with warg pups - very similar to dingos but slight adjustments so they can grow into wargs.
* disenchanters can appear in the main dungeon
* dragons, nagas, and golems don't balk at approaching as much
* dwarves sometimes start with potions of booze (xNetHack)
* all elementals resist sickness
* arch-liches resist acid
* elf-lords get 9AC, Elvenkings get 8AC (K-Mod)
* erinys can generate up to 13 times (previously only 3 could be birthed in the entire game)
* ettins count as giants and are vulnerable to sling damage
* fell beasts can shriek, inflicting stun damage (xNetHack/EvilHack)
* floating eyes inflict less passive paralysis; wisdom limits duration (Dynahack)
* all footrice can fly
* all footrice have more potent hissing attacks - the stoning process is twice as likely
* foocubi gain a level when draining one from the player (xNetHack)
* gas spores and volatile mushrooms start with exactly 1 HP
* genetic engineers grudge all other monsters, and their difficulty has been increased.
* all ghost class monsters get acid resistance
* giant mimics get an engulf-digest attack
* giant spiders can ensnare monsters in webs (EvilHack)
* gnome lords and kings always get gnomish suits
* gnomish wizards always get a gnomish helm
* gnomes get candles in the mines twice as often as before
* goblins can generate in small groups (Sporkhack)
* green slimes can hide on the ceiling (xNetHack)
* green slimes can appear in the main dungeon, are faster (going from 6 to 13 speed), higher difficulty
* green slimes have a passive sliming attack (Grunt)
* gremlins can steal intrinsics no matter the time of day (FIQHack)
* peaceful gremlins don't use fountains/pools/etc to split themselves (Fourk)
* hobbits can get flint with their slings (xNetHack)
* horned devils get a butt attack
* all hulks resist poison
* ice and bone devils are now lawful (xNetHack)
* ice devils have speed 8 (K-Mod)
* ice devils' cold sting and claw attacks have been buffed, they have the power to strip cold resistance from the player or monsters (xNetHack)
* iron golems get a passive disenchant attack (from SLASH'EM steel golems)
* jellyfish get a passive paralyzing attack
* Keystone Kops are tougher (K-Mod)
* Keystone Kops no longer wander, but instead can flank
* lava demons are huge
* leprechauns do not stash gold in the ground after stealing it (reverted from 3.7)
* lizards appear with slightly less frequency
* ki-rin get shock, sleep, cold, and poison resistance (xNetHack)
* long worms have thick skin, 7 speed, -5AC, a 2d10 bite attack, and accurate behavior
* long worm segments have lower chance to be cut
* lords and princes never get negative weapons or armor (xNetHack)
* lieutenants are considered lords (xNetHack)
* master liches and arch-liches can see invisible (FIQHack)
* mastodon is now huge; has -8 AC, strengthened butt attacks from 4d8 to 4d16; increased difficulty
* mastodon gets a hug attack and can berserk (EvilHack)
* giant mimics, large mimics, and killer mimics are higher level and difficulty
* mimics take the form of strange objects much less often
* mind flayers are bright magenta
* mind flayer attacks can make hero forget skills (EvilHack) - however the frequency and impact of these attacks has been weakened
* mind flayer psychic blasts do more damage; if the victim is telepathic they can also be stunned
* minotaurs resist death magic (SLASH'EM)
* minotaurs have a thick hide, have flanking, and berserk
* minotaurs carry wands of digging less often
* molds can generate in small groups
* molds and fungus can grow on corpses (SLASH'EM/xNetHack)
* monkeys get a small head start after they steal an item (xNetHack)
* Mordor orcs can spawn with orcish boots
* mumakil get butts or kicks instead of bites
* mummies get a nasty withering attack (xNetHack/EvilHack)
* all mummies get an additional -1AC to compensate for their ragged wrappings
* Nazgul always spawn accompanied by a fell beast (EvilHack)
* Nazgul have increased level, difficulty, AC, attack strength, infravision, and MR (EvilHack)
* Nazgul get an additional weapon/drain attack, can flank, and resist stoning
* nurses won't heal you if you are undead
* nurses can also cure rabid status
* nurses cannot flank or assist flanking
* nurses grant max-hp at a much higher rate, for quicker "nurse dancing"
* nymphs spawn with mirrors half as often (25% chance instead of 50%)
* olog hai get poison resistance, are huge, have thick skin, higher level and speed, with raised difficulty.
* all orcs can stalk the player
* orc captains now are lords and have speed 9 (xNetHack)
* orc shamans and kobold shamans are skittish (FIQHack)
* paper golems leave special cards for cartomancers
* pit fiends have speed 8 (K-Mod)
* priests of Moloch are always generated hostile (SLASH'EM)
* purple worms have thick skin
* pyrolisks have negative alignment
* quasit buffs: faster, stronger attacks, see invisible, can appear in small groups (xNetHack)
* queen bees can displace monsters
* quest leaders resist death magic (EvilHack)
* quest nemeses can break boulders after getting frustrated enough.
* rock moles can actually eat rocks (xNetHack)
* rock trolls are stoning resistant (xNetHack)
* shriekers can shriek from any distance whenever they see you.
* all spheres explode on death (unless cancelled)
* all spheres have speed 15 and 0 AC.
* skeleton and shade slow attacks are ineffective vs undead
* soldiers get half as many C-and-K-rations (K-Mod)
* soldiers and their higher ranks get level, speed, AC, and MR boosts (K-Mod)
* soldiers can generate with shuriken
* seducing monsters will introduce themselves before stealing items (SpliceHack/xNetHack)
* sewer rats hide under objects (xNetHack)
* scorpions are tiny
* shades get 20MR
* shapechangers turn back to their base form when killed with 50-75% of their health (SLASH'EM)
* shapechangers hold level-appropriate form longer, out-of-depth forms for less time (Fourk)
* cancelled shapeshifters cannot change form
* shopkeepers' base level raised to 24, AC to -6 (SLASH'EM)
* shopkeepers get extra defensive items (SLASH'EM)
* shopkeepers get a wand of sleep instead of striking (EvilHack)
* shopkeepers and priests are colored yellow (xNetHack)
* shopkeepers resist sleep and poison
* tame spiders will not spin webs
* telepathic monsters convey a short amount of intrinsic telepathy when eaten.
* titans can see invisible (FIQHack)
* titans resist death magic (SLASH'EM)
* titans are level 17 (K-Mod)
* tigers are orange (EvilHack)
* tigers can also jump
* titanothere is now huge; has -2 AC, strengthened claw attack from 2d8 to 8d8; increased difficulty
* trappers and lurkers above are mindless and speed 6
* troll meat provides temporary intrinsic regeneration (xNetHack)
* violet fungi puff out hallucination-inducing spores when hit
* all vortices (v) resist shock damage
* vampire mages can see invisible
* vampires (any V) are not afraid of cracked or Molochian altars
* vampires attack with their bite attacks first
* vampires can use weapons (EvilHack)
* all werefoo in animal form get infravision
* wargs have a thick hide
* werefoo revert back to their base form when killed (SLASH'EM)
* werefoo can occasionally summon rabid brethren
* werefoo can disguise themselves in both animal and humanoid forms (Crecelle)
* werewolves and weretigers have a higher level and difficulty, stronger attacks
* wraiths also no longer "stalk" the player and follow them across levels (Dynahack)
* the wumpus is now unique to the ranger quest and much scarier; it also now appears in a random room in the Ranger's locate level
* wumpus is now huge with a thick hide; strengthened bite attack from 3d6 to 6d9; increased difficulty
* xans can't fly (dNetHack)
* xorns have flanking
* yellow and black light explosions are directionless (xNetHack)
* yellow molds puff out stunning spores when hit
* wood nymphs are slightly slower than average, lower difficulty (xNetHack)
* Wood nymphs leave grass instead of corpses (CrecelleHack).
* water nymphs are slightly higher level and difficulty (xNetHack)
* mountain nymphs are higher level, faster, and higher difficulty (xNetHack)
* hill giants are lower level and difficulty (xNetHack)
* stone giants are slightly stronger and can wrest boulders out of the ground (xNetHack)
* fire giants get an active fire attack (xNetHack)
* frost giants get an active frost attack (xNetHack)
* storm giants get an active ranged lightning attack (xNetHack)

### Delayed stoning for all footrice effects
* This was ported from EvilHack with extensions.
* Instant petrification has been removed both for the player and for monsters (keep in mind this only applies for footrice, NOT for Medusa's gaze!)
* Instead, wherever a monster or player would have been instakilled, a stoning timer is started for 5 turns.
* This applies for every instapetrification effect: touching a footrice corpse, being knocked into a footrice
* Footrice only inflict slow stoning for the player and for monsters

### Dangerous piercers
* All piercers are mindless and can grow up
* Much more AC is required to dodge dropping piercers (previously, -2AC would nullify their drop attacks, now -22AC is required)
* Piercing damage scales with their level (monster level * 6) with a minimum of 4d6 being dealt.
* Piercers and lurkers/trappers always generate hidden if possible.
* Hidden piercers (and other ceiling clingers) can surprise attack you from adjacent squares.

**Piercers can actually pierce hard helmets:** Piercers can penetrate even the toughest helmets, but the level of enchantment on your helmet determines its resistance to piercer damage and destruction:

**Helmet Resistance:**
* Only hard and metal helmets are affected, cloth and leather helms are safe from this specific damage.
* If a piercer strikes a helmet with a negative enchantment, the helmet is instantly destroyed.
* For helmets with positive enchantments, a successful hit reduces the enchantment level by -1. With bad luck, the penalty may range from -1 to -3.
* Glass and Crystal Helmets: Glass helmets (e.g., crystal helms) don’t lose enchantments. Instead, they crack over time, following erosion rules rather than enchantment degradation.
* Enchanting your helmet can be both protective and risky. A higher enchantment level defends against weaker piercers but may still leave you vulnerable to stronger ones.
* Special Case – God Piercers: God piercers deal extremely high damage. Your best defense is achieving an AC of -22 or better, as even the most enchanted helmets provide limited protection against their attacks.

**Enchantment Levels and Piercer Resistance:**
* +1 enchantment: Generally protects against rock piercers.
* +2 enchantment: Generally protects against iron piercers.
* +3 enchantment: Generally protects against glass piercers.
* +4 enchantment: Generally protects against diamond piercers.

### Reviving and Poisonous Zombies
* Zombie corpses may auto-revive similar to trolls (EvilHack/xNetHack)
* Cancelled or beheaded zombies/trolls don't revive (EvilHack)
* Wielding Sunsword prevents zombies corpses from appearing (EvilHack)
* Playing as a priest reduces the chance of zombie revival by 50% (Dynahack)
* All zombies get an additional poisonous bite attack that can drain constitution.
* Sometimes zombies will try to bite the players legs, inflicting wounded legs for a short time.
* Zombies are immune to being scared by Elbereth

### Dragon changes
* Dragons have been overhauled to more closely resemble the versions in SLASH'EM and FIQHack.
* An attempt has been made to make each dragon have a special quality or perk.
* Part of the challenge in SLASH'EM was that adult dragons (and therefore dragon scales) were more difficult to come by. Baby dragons are plentiful and can potentially be tamed and grown up into adults, but with the large gap in levels the process is long and difficult. It's possible they might not be guaranteed in Ludios or the Castle anymore either, but the increased frequency means they should show up in Gehennom much more often.
* Dragons are always generated awake and pissed for Knights (from EvilHack).

**Baby dragon changes**
* Most baby dragons are level 4 and difficulty 6 (SLASH'EM)
* Their size has been reduced from HUGE to LARGE (eliminates possible knockback on the player)
* Reduced their weight from 1500 to 1000.
* They can generate randomly in the dungeon with a frequency of 1, but not in Gehennom
* Baby dragons get a special 1d6 bite attack instead of a 2d6 physical bite (K-Mod).
* For most dragons, their bite matches their adult breath attack (red = fire bite, blue = shock bite, etc).
* All baby dragons get an additional 1d6 claw attack
* baby dragon alignments match their adult counterparts (EvilHack)
* baby red dragons can berserk
* baby blue dragons are slightly faster at speed 12
* baby green dragons regenerate, and are slightly higher level and difficulty
* baby yellow dragons get a passive acid attack
* baby gray dragons flank
* baby white dragons are weaker
* baby gray dragons get a disenchanting bite
* baby black dragons get a drain life attack (and level 7 difficulty)

**Adult dragon changes**
* They get a 3d8 bite and 2d4 claw attacks, and are frequency 2.
* Their speed has been increased from 12 to 20, and have a small buff to their claw attacks (FIQHack)
* all dragons stalk/follow the player (FIQHack)
* red dragons can berserk
* blue dragons are faster (speed 24)
* green dragons regenerate and are slightly higher level
* orange dragons get an engulf digestion attack
* black dragons get a terrifying roar
* yellow dragons get a passive acid splash attack
* white dragons are weaker than other dragons
* gray dragons can flank
* shimmering dragons have displacement and resist stunning
* Not all dragons can see invisible. Only highly intelligent and/or magical dragons get this ability. Removed see invisible from red, green, white, orange, and yellow dragons.

### Unique monster changes
* unique monsters cannot be tamed
* Croesus can move other monsters out of his way (EvilHack)
* Ixoth can berserk. Speed raised to 20, AC raised from -1 to -4, stronger claw attacks.
* Ixoth gets poison resistance (EvilHack)
* Lord Surtur can berserk, jump, and cast mage spells.
* Lord
* Cyclops can berserk
* The Master Assassin is poison resistant (xNetHack)
* The Master Assassin is stronger, faster, sees invisible, resists sleep, and gets one additional attack.
* Yeenoghu's magic missile attack has been buffed to 6d6 (EvilHack)
* Vlad gets stoning resistance.
* King Arthur gets a full suite of resistances.
* Give Baalzebub some combat buffs (xNetHack).
* Master Kaen and the Grand Master receive the same intrinsics that high level monks have.
* Dispater drops a deck of fate.
* Dispater can walk through walls

#### Warping behavior for demon princes and lords and quest nemeses
* These covetous monsters will now only perform one initial warp to get to the player. After their introduction, they will revert to standard AI and movement.
* This makes most lords and nemeses a little less dangerous to handle and allows the player to create different strategies to deal with them.
* Cthulhu is a unique threat - because he resurrects he will be able to regain the warp each time he revives.

**Medusa**
Inspired by EvilHack, Medusa gets an overall difficulty boost:
* She goes from level 20 to 24
* She gets -8AC (a big buff from 2AC)
* Her weapon attack goes from 2d4 to 4d4
* Instead of a single poisonous bite, she gets two poisonous snake bite attacks.
* Medusa also gets a stoning bite (EvilHack).
* Medusa gets infravision

**Wizard of Yendor**
* Rodney is bright magenta (EvilHack)
* Rodney will never steal the quest artifact of the current role (UnNetHack)
* Rodney gets a strong weapon and the ability to use it (EvilHack)
* Rodney is now telepathic

**The riders**
* Each rider gets an additional 100 HP (EvilHack)

**Cthulhu:**
* NerfHack's Cthulhu is a blend of his counterparts in SLASH'EM and UnNetHack with some new enhancements to make him a fearsome component of the endgame:
* Speed of 18 matches SLASH'EM.
* AC was lowered from -15 to -8 to match UnNetHack.
* Cthulhu's inventory os prevented from being shown when probed (UnNetHack)
* Cthulhu now has flying and is telepathic
* Cthulhu can displace monsters, pass through iron bars, break boulders and bust down doors to get to you.
* Cthulhu will always track you down and chase you.
* Converted the drain intelligence attack to drain energy instead.
* Cthulhu is placed right in the middle of Moloch's Sanctum as a guardian but does not receive the Amulet of Yendor.
* Allow Cthulhu to return via wizard harassment if the player is carrying the Amulet of Yendor.
* **Note: Cthulhu is covetous and will perform a single warp to reach the player.** After that, he will revert to standard non-covetous movement - however, when he dies and resurrects, he will always get the initial warp back.

## MONSTER BEHAVIOR


### Monster item use
* Monsters can use figurines and magic flutes (EvilHack)
* Monsters can use cameras to blind you (SpliceHack)
* Monsters can read scrolls of remove curse (EvilHack)
* Monsters can read scrolls of stinking cloud and target the player (EvilHack)
* Monsters can read scrolls of fire and target the player (deferred in vanilla)
* Monsters can read scrolls of flood (defensively)
* Monsters can throw (lit) potions of oil at you (xNetHack)
* Monsters can throw potions of polymorph (EvilHack)
* Monsters can throw potions of hallucination at you (xNetHack)
* Non-lawful monsters can dip weapons into potions of sickness.
* Monsters can zap wands of cancellation at the player (EvilHack)
* Monsters can zap wands of slow monster at the player (EvilHack)
* Monsters can zap wands of wonder at the player
* Hostile monsters wielding a digging tool can break boulders (EvilHack)
* Monsters can quaff potions of restore ability to un-cancel themselves (EvilHack)
* Monster will quaff potions of reflection if you have a reflectable attack available.
* Vampire monsters can quaff vampire blood to heal (SLASH'EM)
* When playing as a cartomancer, monsters can use monster summon cards and zappable cards against you.
* Some monsters will not throw weapons that are usable for melee.
* Monsters won't try to use wands of digging on hardfloor levels.
* Monsters will not be tricked into picking up projectiles endlessly while in combat.
* Monster will attempt to wrest wands if there are no charges left.

### Monster accessory use
* Adapted from EvilHack with modifications
* Monsters can wear most rings and amulets.
* Your pets can also wear the same items, but you need to #loot them and manually give them the gear you want them to equip.
* The range of usable items has been expanded upon, notably:
  * All resistance rings
  * rings of teleportation and teleport control
  * amulets of flying and boots of levitation
  * stomping boots
  * amulets versus poison
  * amulets of ESP
  * rings of polymorph (turns any monster into a shapeshifter!)

### Misc monster behavior changes
* Monsters with a negative AC get damage reduction from melee attacks (EvilHack)
* Monsters will switch to their melee attack intelligently (Sporkhack)
* When a monster spawns with a weapon, it wields it immediately (xNetHack)
* Intelligent monsters pick up keys and lock picks (UnNetHack)
* Magic-liking monsters will pick up magical tools (xNetHack)
* Covetous monsters will equip wearable items that they target (xNetHack)
* Monsters will use ranged combat in melee as a fallback option (Grunt)
* Monster stunning now works similarly to player stunning (xNetHack)
* Add more spears in monster starting inventory (Fourk)
* Hallucination protects against skeleton bone rattling (xNetHack)
* Headless and breathless monsters don't cough in poison gas clouds
* Monster knockback is noisy.
* Monsters may be woken up by eating carrots, reading dusty books, or rolling boulders.
* Monsters that hatch in water drown unless amphibious or natural swimmers.
* Monsters can use breath/spit attacks in melee range (FIQHack).
* Cancelled monsters can't explode (in death or as an attack).
* Displacing monsters (like the displacer beast) cannot displace you if helpless or trapped.
* Cancelled displacers are incapable of displacement.
* Force-fighting displaced monster can also result in displacement.
* Because see invisible cannot be gained intrinsically - peaceful monsters will not make themselves invisible by means of potions, wands, or spells.
* Monsters can hide under other dungeon furniture (xNetHack)
* Player monsters can steal the amulet from the player (EvilHack) - however they will not attempt to sacrifice it.
* Monsters carrying the Amulet of Yendor are incapable of teleportation.
* Player monsters or any covetous monsters will grudge any monster that has the Amulet of Yendor (EvilHack).

### Flanking behavior
* Ported from SpliceHack, with enhancements
* Monsters with this property have the M2_FLANK tag.
* Any two monsters can flank a player (or another monster) if they sandwich the target. However, monsters with this property ("outflankers") are more tactical and will actively seek opportunities to flank you.
* Monsters gain a large to-hit bonus when flanking
* Flanking now scales with monster level (it used to be a flat +4 AC penalty in SpliceHack):
* Monsters that are natural outflankers get a much higher bonus than other monsters.
* Flanking has been applied to many monsters in NerfHack.

* Using a pet, you can also take advantage of flanking. Simply place yourself and your pet in such a way as to "sandwich" the monster. You (or your pet) will get a flanking bonus on the victim when attacking.

Flanking restrictions:
* You cannot flank if hallucinating, afraid, confused, punished, fumbling, wounded, unaware, stunned, or standing on an Elbereth engraving.
* You must be able to see the monster you want to flank.
* Monsters cannot flank if eating, sleeping, fleeing, confused, stunned, trapped, petrified, sick, diseased, stationary, or hiding.

Certain roles also count as natural flankers and will get higher bonuses than other roles:
  - Knights
  - Monks
  - Rangers
  - Rogues
  - Samurai
  - Valkyries

### Berserking behavior
* Ported from EvilHack, with modifications
* Monsters with this property have the M3_BERSERK tag and can be quite dangerous if you take them for granted
* When berserkers are below 50% of their health, they have a high chance to go into berserk mode
* Monsters can also immediately go berserk if they are woken and angered
* When a monster goes berserk it turns hostile and regains a roll of it's max HP, possibly
  recovering all of its HP.
* Nearby denizens are also woken up when a monster goes berserk (it screams in anger)
* When berserking, monsters totally ignore Elbereth or Scare Monster. If they are usually skittish or trying to keep away, they will instead actively approach
* Berserking monsters also never flee when their HP gets low
* A berserking monster deals double damage rolls when hitting you
* Taming berserking monsters only un-berserks them, it doesn't pacify or tame
* Monsters that can berserk: all dwarves, mordor orcs, uruk-hai, mumaks, zrutys, fire giants, frost giants, storm giants, ettins, all ogres, owlbears, sasquatches, gnolls, and balrogs.
* Berserkers get angry when stuck in traps.

### Rabid monsters
This is a brand new mechanic, debuting in NerfHack!

* There is a fairly small probability of a monster spawning rabid, but bats and coyotes always have a 1 in 10 chance of spawning infected.
* Rabid is mostly limited to living mammals. Insects, birds, and lizards cannot contract it.
* For special rooms (zoos, throne rooms, etc), rabid monsters are prevented from spawning.

Effects of the rabid status on monsters:
* Rabid monsters get an additional bite that can cause the player to become rabid. This bite attack is also poisonous (damaging CON), similar to the rabid rat.
* Rabid monsters don't regenerate
* They grudge all non-rabid monsters (that are capable of catching rabies).
* They occasionally move erratically
* They will never flee or become scared and will actively approach.
* Rabid monsters cannot quaff potions.
* Rabid monsters cannot be tamed.
* If a tame pet becomes rabid, it immediately loses its tameness and becomes hostile.
* Rabid monsters grant a little extra XP when killed.
* Rabid humanoids will growl when #chatted with.

Effect of being rabid on the player:
* You cannot regenerate
* You become bloodthirsty in your attacks (similar to wielding Stormbringer).
* You occasionally move erratically - 1 in 10 moves is confused.
* When the player is infected a timer starts from 100 + d(CON*2) turns.
  * At 40 turns, you develop a fear of water and cannot quaff potions.
  * At 10 turns, you become confused.
  * At 0 turns, you die.

Curing rabid:
* Generally the same guidelines for illness apply, but there are a couple important differences to know about.
* **You cannot use a unicorn horn to heal rabid status!**
* You can drink healing potions (before the fear of water sets in)
* You can cast cure illness
* You can pray (counts as a major trouble)
* You can eat a eucalyptus leaf or a clove of garlic
* You can eat the corpse of a dog (tinned or otherwise)
* You can be healed and cured by a nurse
* You can rub a non-cursed foulstone.  When the foulstone is used this way, it autocurses and becomes a dangerous item again.
* Rabid monsters that poly can stop being rabid if the new form is immune - the same goes for the player.

### Diseased monsters
* Ported from EvilHack
* Monsters can become infected with terminal illness, with a short countdown to death.
* Monsters can cure themselves if they have the means, and the player can use cure sickness or eucalyptus leaves to heal sick pets.
* Currently, the only weapon that causes disease is Grimtooth.

### Accurate behavior
* Ported from EvilHack, with modifications
* Monsters with this property have the M3_ACCURATE tag
* Makes monsters more accurate in melee and with projectiles
* These monsters get a large to-hit bonus of +5 or more
* Players are the elven starting race or polymorphed into elves also enjoy a to-hit bonus that scales with your level.

### Jumping behavior
* Ported from EvilHack/SpliceHack
* Lets monsters jump at you from a few squares away, quickly bridging the gap between you
* They can also cross short barriers like water and lava and even jump over other monsters

### Withering attacks
* Ported from xNetHack and EvilHack
* Withering is a nasty new attack that will give the player the "wither" status temporarily. Whilst withering you will lost 1HP per turn.
* If you are already withering and the new wither attack is strong enough, it will also drain some of your maximum HP, making this threat quite insidious.
* Withering can be cured by quaffing holy water, praying, or invoking the Staff of Aesculapius.
* Any item that grants extrinsic disintegration res also grants withering resistance (black dragon scales, bracers of integrity)
* When playing as a vampire, you will also enjoy withering resistance by virtue of being undead.
* All mummies possess wither attacks.
* Powerful clerics can also cast the Blight spell at range which can cause withering.


## MONSTER SPELLCASTING


* Monsters can target and cast spells at other monsters (EvilHack).
* Peaceful monsters won't cast make invisible on themselves. They also won't drink potions
  of invisibility or zap themselves with wands of make invisible.
* Monster spellcasters will prioritize healing when wounded.
* Monster spellcasters can cast stone-to-flesh in response to getting stoned (EvilHack).
* Don't let monster cleric stunning reset stun counter to 1 when stunned.
* Displacement, invisibility, and darkness offer limited protection from spellcasters.
* Telepathic spellcasters can usually bypass invisibility and displacement protections.

### Mage Spells

**psi bolt**
* Now a ranged spell.
* Does an extra 1d6 if you have telepathy.
* Damage scales down the further away the caster is.

**reflection (EvilHack)**
* A spell that creates a shimmering globe around the caster, granting them reflection for several turns.
* Can be dissipated with a blast of cancellation.

**acid blast (EvilHack)**
* Explodes an acid blast on its target and the surrounding squares. The damage output is dependent on the level of the monster casting it.
* The acid from this spell also has a chance of eroding any unprotected weapons or armor in open inventory.
* Ranged, can be cast at the hero up to 13 squares away.

**ice bolt (EvilHack)**
* This spell explodes a small ice storm upon its target (and surrounding squares)
* Any non-protected objects in open inventory are subject to being frozen.
* This is a low-level spell, so access to this spell is given to every monster spellcaster that has access to mage-based spells.
* Ranged, can be cast at the hero up to 13 squares away.

**fire bolt (EvilHack)**
* This spell explodes a small fireball upon its target  (and surrounding squares)
* Any flammable objects in open inventory are subject to being burned.
* This is a low-level spell, so access to this spell is given to every monster spellcaster that has access to mage-based spells.
* Ranged, can be cast at the hero up to 13 squares away.

**destroy armor**
* Altered from Vanilla NetHack, ported from EvilHack
* Having magic resistance is no longer full protection against this spell. Any piece of armor being worn can have its fixed status removed, and then can be deteriorated to the point that it's completely destroyed. Even armor that is normally erodeproof (dragonhide and dragon scales, etc) is affected. Having MR keeps the erosion level at one per cast, otherwise the erosion level is of one to three levels per cast. Blessed pieces of armor have a small chance of resisting. Armor-based quest artifacts are immune to this spell, as is crystal plate mail.

**entomb (xNetHack)**
* Used by a monster when they are low on health or fleeing. It is primarily for escape and when cast surrounds the player with boulders.
* Any mage-spellcaster can use it when desperate.
* In xNetHack there was also a chance to create solid walls to block the player in, this effect was removed so it only drops boulders.

**call undead**
* Ported from SLASH'EM
* Call Undead can only be cast by undead and demon spellcasters
* Ranged, can be cast at the hero from up to 13 squares away.
* All wraith class monsters (W) are eligible, depending on difficulty
* Mummy class monsters (M) are also eligible (SLEX)
* Excessive chain-summoner spawns are prevented; a caster can only summon a spellcaster of lower difficulty so a demilich could summon a lich, but not another demilich. Ghoul mages and liches are both difficulty 14 so neither can summon the other.

**evil eye (dNetHack)**
* When successfully cast on the hero it lowers your Luck by 1 point.
* Evil eye can only be cast by undead and demon spellcasters.
* Because this is implemented as a gaze attack, the player can increase their protection by being invisible or displaced. There is no maximum range to this spell.

**cure self**
* Spellcasters can use this to cure illness, blindness, withering, and rabid statuses.

**teleport**
* High level spellcasters are able to warp to the hero when further than 7 square away.


### Clerical Spells

**open wounds:**
* Now a ranged spell.
* Damage scales down the further away the caster is.

**lightning:**
* Now a ranged spell.

**protection (EvilHack)**
* This is the monster version of the protection spell already available to the player.
* Provides a temporary magical shield that increases the monster's AC protection.
* Can be dissipated with a blast of cancellation.

**geyser spell**
* The core spell is unchanged from Vanilla NetHack, however now the geyser also rusts armor and instakills iron golems (EvilHack)

**hobble**
* This clerical spell smashes the hero's legs with a magical force and inflicts you with wounded legs for a brief period
* Ranged, can be cast at the hero from up to 13 squares away.
* Damage scales down the further away the caster is.

**blight (xNetHack)**
* In xNetHack, this spell was reserved for 'dark speech' - a nasty group of curses that Asmodeus and Demogorgon can use. But it was extracted out and used as a new clerical spell which inflicts withering on the player.
* The duration of the withering lasts 20-60 turns. It can also be cast up to 8 squares away.

**flesh to stone**
* This is the highest level clerical spell
* When cast it can start the stoning process on the hero.


## ROLE CHANGES


### Archeologist
* An Archeologist wielding a bullwhip will not fall through trap doors (SLASH'EM)
* Archeologists get bonus when searching (FIQHack)
* Archeologists start out knowing dwarvish mattocks and any race can use them.
* Archeologists always get an extra id when reading scrolls of identify.
* Archeologists start with an extra scroll and spellbook (SLASH'EM).
* Archeologists sometimes crack their whip at animals, scaring them.
* Archeologists count as primary spellcasters, so they benefit from spell memory bonuses when casting spells.
* Archeologists can highly enchant fedoras (xNetHack)
* Add boomerangs, spare tinning kit, grappling hook to Arc home (xNetHack).

**Archeologists vs snakes!**
* Archeologists get a -1 to-hit penalty when fighting snakes (any S class monsters).
* Snakes get a +1 to-hit bonus on archeologists
* All snakes have the potential to paralyze archeologists in fear when they successfully connect a hit. Free action only protects the hero 75% of the time vs these paralyzing attacks.
* Some giant anacondas have a chance of appearing in the arc quest now.
* Archeologists are not afraid of snakes when hallucinating.

**Skill adjustments for archeologists:**

| skill  | NetHack    | ->  | NerfHack |
| ------ | ---------- | --- | -------- |
| axe    | restricted | ->  | basic    |
| spear  | restricted | ->  | basic    |
| shield | n/a        | ->  | skilled  |

### Barbarian
* Barbarians start with a little more food (SLASH'EM).
* Barbarians get a **blood rage bonus** for low health.
  * Only occurs when barbarians reach level 4 and higher.
  * When under 40% of their max HP, they get a damage bonus that scales with their level.
  * When under 25%, this bonus is doubled.
  * Each rage attack uses up 1d5 energy, so at least 3 energy is required to trigger a rage attack.
  * This feature was adapted from the SpliceHack skill system.
* The barbarian quest gets a lot more trees in the beginning (these can be chopped down now)
* More random O and T spawn in the quest.

**Skill adjustments for barbarians:**

| skill  | NetHack | ->  | NerfHack |
| ------ | ------- | --- | -------- |
| riding | basic   | ->  | skilled  |
| shield | n/a     | ->  | skilled  |

### Cave Dweller
* Cavemen start with a random set of dragon scales.
* When reading scrolls of identify, cavemen will never be able to identify all items, they will be instead identify 1 instead.
* Cavemen have also been gifted with more skills in rudimentary tools like rocks and flint:
  * They start the game with more flint and no rocks (xNetHack)
  * Cavemen can lash flint to arrows, making them do slightly more damage (Sporkhack/THEM). When arrows are flinted, their enchantment is also revealed.
* Cavepersons can get an alignment boost via cannibalism (Sporkhack)
* Cavepersons' gods sometimes don't respond to prayer. If you have abused your alignment, there is a 10% chance of being ignored (Sporkhack/SlashTHEM/EvilHack)
* Unlike other roles, cavemen do not start out knowing scrolls of identify.
* Cave dwellers start with really low intelligence. As a result, they are incapable of reading scrolls, spellbooks, or other legible items until reaching 6 INT.
* Instead of the standard crowning gift, cavemen always receive Giantslayer (EvilHack)

**Caveman quest updates:**
* The cavewoman quest has been updated and filled with more jungle type monsters: tigers, pythons, and the like. There is also a lot of water added and ; monsters to occupy it (SlashTHEM)
* The Chromatic Dragon has some buffs: Speed raised to 20, AC raised from -1 to -4, stronger claw attacks.
* The Chromatic Dragon can now berserk.
* Their quest narration and dialogue is more caveman-like (xNetHack/Fourk)

**Illiterate bonuses:**
* They can increase their max-HP at each level-up if they remain illiterate (Sporkhack/THEM)
* Updated XP boosts are from EvilHack:
  * Experience levels 1-2: 2-4 HP boost per level.
  * Experience levels 3-9: 3-6 hp boost per level.
  * Experience levels 10-17: 3-8 hp boost per level.
  * Experience levels 18 and up: 5-12 hp boost per level.

**Spellcasting nerfs**
* They cannot receive spells from their deity (EvilHack)
* They have an 80% chance of failing to read any spellbook
* Their special spell has been removed (EvilHack)
* They cannot read spellbooks until their INT is 6 or greater (this is a general nerf for all roles, but cavemen in particular start with 3-4 INT)

**Skill adjustments for cave dwellers:**

| skill         | NetHack    | ->  | NerfHack   |
| ------------- | ---------- | --- | ---------- |
| dagger        | Basic      | ->  | Restricted |
| knife         | Skilled    | ->  | Restricted |
| morning star  | Basic      | ->  | Restricted |
| polearms      | Skilled    | ->  | Restricted |
| attack spells | Basic      | ->  | Restricted |
| matter spells | Skilled    | ->  | Restricted |
| riding        | Restricted | ->  | Basic      |
| shield        | n/a        | ->  | Basic      |

* Cave dwellers cannot have skills in edged or pointy weapons unrestricted. Note that they can still receive these weapons as altar gifts. The exception is unicorn horns, which the cave dwellers can reach skilled in.
* Cavemen get Skullcrusher as their first sacrifice gift.

### Healer
* Added L's Wounds patch: healers can see damage on monsters
* Healers start with a +1 scalpel
* Healers start with 2 eucalyptus leaves.
* Healers get a bonus when applying unicorn horns
* Healers can use an uncursed unicorn horn as if it is blessed.
* Healers know blood potions (SpliceHack).
* Healers start out knowing potions of restore ability, sickness, paralysis, and sleeping (HackEM).

### Knight
* Only lawful Knights can dip for Excalibur (EvilHack/Sporkhack)
* Knights start with a +0 studded leather armor instead of a +1 ring mail (K-Mod)
* The knight's quest has been infested with a swarm of merfolk

**Skill adjustments for knights:**

| skill       | NetHack | ->  | NerfHack   |
| ----------- | ------- | --- | ---------- |
| dagger      | Basic   | ->  | Restricted |
| knife       | Basic   | ->  | Restricted |
| axe         | Skilled | ->  | Restricted |
| pick-axe    | Basic   | ->  | Restricted |
| broad sword | skilled | ->  | Expert     |
| club        | Basic   | ->  | Restricted |
| polearms    | skilled | ->  | Expert     |
| spear       | skilled | ->  | Expert     |
| trident     | Basic   | ->  | Restricted |
| shield      | n/a     | ->  | Expert     |

### Monk
* Monks can start with the spell of sleep (in addition to confuse monster, light, and protection).
* Monks start with a potion of reflection.
* Monks gain acid resistance at level 19 (dNetHack).
* Dramatically increased the monk's body armor penalty (EvilHack)
* Give explicit feedback for monks and cartomancers wearing/removing body armor
* Stop giving "You feel guilty message" eventually after breaking vegetarian conduct enough times (xNetHack)
* Monks get a **fully charged magic marker** as a crowning gift.
* Add trees and two ponds to monk quest start.
* Monk starting spell competency depends on the spellbook.
* Martial arts users are immune to leg damage from bad kicks (xNetHack).
* Whilst wearing the gauntlets of force, monks can break boulders and iron bars whilst bare-handed.
* Monks that have reached grand master in martial arts and level 21 start getting a 1 in 20 chance for critical hits when fighting bare-handed. On critical hits, you inflict double damage.

  **Skill adjustments for monks:**

| skill              | NetHack | ->  | NerfHack   |
| ------------------ | ------- | --- | ---------- |
| crossbow           | basic   | ->  | restricted |
| quarterstaff       | basic   | ->  | expert     |
| enchantment spells | basic   | ->  | skilled    |
| divination spells  | basic   | ->  | restricted |
| escape spells      | skilled | ->  | restricted |
| matter spells      | basic   | ->  | restricted |

### Priest
* Priests start with a +2 small shield (SLASH'EM)
* Priests cannot have edged weapon skills unrestricted (EvilHack)
* Priests don't receive edged/pointy artifact weapons via altar sacrifice (EvilHack)
* Instead of the standard crowning gift, priests always receive Mjollnir (EvilHack)
* Priests reduce the chance of zombie revival by 50% (Dynahack); when a zombie is destroyed for good, you get a special message
* Priests start with more garlic and wolfsbane (similar to the undead slayer in SLASH'EM)
* Vampire priests don't start with any food items. Instead they get potions of vampire blood.

**Skill adjustments for priests:**

| skill    | NetHack    | ->  | NerfHack   |
| -------- | ---------- | --- | ---------- |
| flail    | expert     | ->  | skilled    |
| trident  | skilled    | ->  | basic      |
| lance    | basic      | ->  | restricted |
| shuriken | basic      | ->  | restricted |
| riding   | restricted | ->  | basic      |
| shield   | n/a        | ->  | basic      |

### Rogue
* Rogues also get a multishot bonus for knives.
* Rogues start with a +2 stiletto instead of a short sword
* Rogues start with a stack of knives instead of daggers
* Rogues start with a leather jacket instead of armor.
* Rogues start with scrolls of gold detection and teleport (SLASH'EM).

**Return of Backstab Damage:**
* Rogue's can inflict **backstab damage** for the first thrown weapon. In 3.4.3 this was a very powerful mechanic that was nerfed in 3.6. We are bringing it back in a limited form as a callback to 3.4.3 but also because it strongly fits the theme of the role.
* Rogues get bonus backstab damage when using stilettos in melee

**Rogue counterattacks:**
* Whilst wielding a knife or dagger, a rogue has a chance of counter-attacking an opponent when hit.
* There are many restrictions:
  * The incoming attack must be a weapon, bite, claw, or kick attack.
  * You cannot be polymorphed
  * You cannot be wearing any heavy metallic armor (excludes mithril) or wielding a bulky shield.
  * You cannot be weak (or worse from hunger) and you cannot be encumbered.
  * You cannot be fumbling or unaware.
  * You must be able to see the monster.
* The chance of countering goes up with your skill in the wielded weapon.
* Each counterattack uses up 10 energy (at least 10 energy required to execute)

**Skill adjustments for rogues:**

| skill            | NetHack | ->  | NerfHack   |
| ---------------- | ------- | --- | ---------- |
| broad sword      | skilled | ->  | Restricted |
| long sword       | skilled | ->  | Restricted |
| two-handed sword | basic   | ->  | Restricted |
| club             | skilled | ->  | basic      |
| mace             | skilled | ->  | Restricted |
| morning star     | basic   | ->  | Restricted |
| polearms         | basic   | ->  | Restricted |
| spear            | basic   | ->  | Restricted |
| crossbow         | expert  | ->  | basic      |
| divination       | skilled | ->  | basic      |
| matter spells    | skilled | ->  | Restricted |

### Ranger
* Rangers get extended range for seeing object's appearance (this lets them see potions and gems from much further away)
* Rangers get auto-id for launchers when they reach XP level 7
* Rangers get auto-id for ammo enchantment when they reach XP level 10 (xNetHack)
* Rangers are not stunned from using portals (they are used to quick travel)
* Rangers can chop down the trees in the quest entry level.
* The ranger quest levels get a bunch of bear traps.
* Rangers start the game with 2 beartraps (xNetHack).

**Skill adjustments for rangers:**

| skill        | NetHack | ->  | NerfHack   |
| ------------ | ------- | --- | ---------- |
| dagger       | expert  | ->  | skilled    |
| knife        | skilled | ->  | Restricted |
| axe          | skilled | ->  | basic      |
| pick-axe     | basic   | ->  | Restricted |
| short sword  | skilled | ->  | Restricted |
| morning star | skilled | ->  | Restricted |
| hammer       | skilled | ->  | Restricted |
| quarterstaff | skilled | ->  | Restricted |
| polearms     | skilled | ->  | restricted |
| spear        | skilled | ->  | Restricted |
| trident      | skilled | ->  | Restricted |
| sling        | expert  | ->  | restricted |
| dart         | expert  | ->  | skilled    |
| shuriken     | skilled | ->  | restricted |
| boomerang    | expert  | ->  | restricted |
| divination   | expert  | ->  | basic      |
| shield       | n/a     | ->  | skilled    |

### Samurai
* Samurai start with +3 wakizashi (Dynahack)
* Samurai get to-hit and damage bonuses for two-weaponing a katana with a wakizashi.
* The samurai quest was updated to have more water and monsters (jellyfish, more ninjas, some nagas).
* Being satiated abuses wisdom for Samurai.
* Samurai are also are immune to leg damage from bad kicks (xNetHack).

**Skill adjustments for samurai:**

| skill | NetHack | ->  | NerfHack |
| ----- | ------- | --- | -------- |
| spear | skilled | ->  | expert   |

### Tourist
* Tourists get automatic type identification for shop items (UnNetHack). This means that all items for sale are identified for you in shops. You can instantly identify anything by selling it.
* Tourists start with more darts (UnNetHack)
* Tourists gain experience by discovering new special rooms.
* Tourists start with a pair of walking shoes.

**Skill adjustments for tourists:**

| skill              | NetHack    | ->  | NerfHack |
| ------------------ | ---------- | --- | -------- |
| club               | restricted | ->d | basic    |
| dagger             | expert     | ->  | basic    |
| knife              | skilled    | ->  | basic    |
| short sword        | expert     | ->  | basic    |
| saber              | skilled    | ->  | basic    |
| unicorn horn       | skilled    | ->  | basic    |
| escape spells      | skilled    | ->  | basic    |
| enchantment spells | basic      | ->  | skilled  |
| two-weapon combat  | skilled    | ->  | basic    |
| base-handed combat | skilled    | ->  | basic    |
| shield             | n/a        | ->  | basic    |

### Valkyrie
* Valkyries can also start with a +1 war hammer and cloak instead of spear and shield (SpliceHack)
* Valkyries can pacify and tame winter wolves/cubs with food as if they were a domestic animal.
* Note: because of a change with war hammers, Mjollnir is now a stronger two-handed weapon
* More fire traps on quest

**Skill adjustments for valkyries:**

| skill  | NetHack | ->  | NerfHack |
| ------ | ------- | --- | -------- |
| shield | n/a     | ->  | master   |

### Wizard
* Wizards start with a cloak of protection instead of magic resistance.
* Wizards never receive magic missile in their starting inventory.
* Wizards can start with a spellbook of fire bolt instead of force bolt.
* Wizards are able to sense magic fountains.
* Wizards can always sense how many charges are left in wands.
* The Dark One gets a cloak of magic resistances and staff (xNetHack)

**Skill adjustments for wizards:**
* Most of the wizard's combat based skills have been restricted and removed (EvilHack)

| skill       | NetHack | ->  | NerfHack   |
| ----------- | ------- | --- | ---------- |
| knife       | skilled | ->  | restricted |
| axe         | skilled | ->  | restricted |
| short sword | basic   | ->  | restricted |
| club        | skilled | ->  | restricted |
| mace        | basic   | ->  | restricted |
| polearms    | skilled | ->  | restricted |
| spear       | basic   | ->  | restricted |
| trident     | basic   | ->  | restricted |
| shuriken    | basic   | ->  | restricted |

## NEW ROLES

### Undead Slayer

The **Undead Slayer** has been implemented as a new role, distinct from the Priest. This rework includes a fresh quest storyline in which the player must reclaim *The Argent Cross* from *The First Evil*. Custom quest levels include the desecrated monastery, haunted catacombs, and The Abyssal Vaults. Unlike the divine spellcasting Priest, the Undead Slayer is a dedicated warrior whose sole mission is to purge the undead.

This version of the Undead Slayer blends old and new mechanics, making it a more challenging role early on but highly rewarding in the endgame. Undead Slayers begin with **drain resistance, sickness resistance, and warning against undead.** They start with **slow movement (speed 10)** as they did in SLASH'EM, but they gain to-hit and damage bonuses against undead and demons. One unique trait is their ability to **completely obliterate zombies, preventing them from leaving corpses.** However, they receive significant alignment and Luck penalties for consuming wraith corpses. Their special spell is *protection*. They can be of any alignment and may choose from **human, gnome, elf, or dhampir** as their starting race.

**Intrinsics:**

| XL  | Intrinsic              |
| --- | ---------------------- |
| 1   | Slow (speed 10)        |
| 1   | Drain resistance       |
| 1   | Sickness resistance    |
| 1   | Warning against undead |
| 1   | Stealth                |
| 10  | Speed                  |
| 15  | Poison resistance      |

Undead Slayers also start with a **revenant pup**, a new undead canine with numerous resistances and the ability to phase through walls. These creatures do not eat, so they are tamed via `#chat` rather than food. Chatting with your pet also increases apport. If you take are of your pup it will grow into the powerful revenant hound, a beast comparable in strength to the hell hound. In terms of weapon skills, Undead Slayers can now reach **skilled in riding.**

However, there are a couple differences from SLASH'EM. They get fast speed and poison resistance at much later levels. They do not receive a guaranteed sacrifice gift or any special techniques. Unlike Priests and Knights, they **cannot turn undead.** Additionally, they do not start with a silver pistol or silver bullets, but a new fourth starting kit has been substituted which features a silver short sword and leather cloak. While they can reach **expert** in Daggers, they are still **ineffective at multi-throwing.**

Undead Slayers also face additional challenges, as **undead and demons always spawn hostile.** To support this, wooden stakes and holy wafers have been ported from SLASH'EM. The wooden stake has been enhanced with **staking mechanics from xNetHack**, allowing for **instakills on vampires**. Holy wafers now have the ability to **stop withering.** The quest levels have also been redesigned, drawing inspiration from dNetHack's Binder quest.

The **new quest artifact** is *The Argent Cross*, an **artifact amulet of reflection** that grants **spell damage reduction, disintegration resistance, and withering resistance** when worn. It also acts as an **artifact light source**. When blessed, it will periodically activate the `#turn undead` effect without requiring the player to stand still. However, if cursed, if your god is angry, or if you are non-chaotic and polymorphed into an evil form, it will instead **aggravate monsters.** The cross follows the same activation timer as clairvoyance, triggering every **15-45 turns** after the last activation.

The **new quest nemesis** is *The First Evil*, who guards *The Argent Cross* and the *Bell of Opening*. This is a **high-level evil shade** with an arsenal of powerful abilities. It can cast mage spells and possesses **nasty touch attacks** that can paralyze, slow, freeze, and shock its foes. Additionally, it is highly resistant to various forms of damage, including cold, disintegration, stoning, sleep, poison, acid, and electricity.

**Other notes:**
* The HP growth for undead slayers has been buffed from their SLASH'EM version to make them more durable.
* Undead slayers take an alignment penalty for drinking vampire blood.
* **Undead slayers' max skills vary dynamically based on their starting kits.**
  * Crossbow, spear, long sword, short sword, and whip all default to a max of basic
  * Starting the crossbow unlocks expert skill in crossbow
  * Starting the silver short sword unlocks expert skill in short sword and skilled for long sword
  * Starting the whip unlocks expert skill in whip and master skill in martial arts
  * Starting the silver spear unlocks expert skill in spear
* If you start with the crossbow, you start with more bolts than in SLASH'EM and the crossbow is now +3.


**Skill adjustments for undead slayers (from SLASH'EM):**

| skill              | SLASH'EM     | ->  | NerfHack   |
| ------------------ | ------------ | --- | ---------- |
| boomerang          | basic        | ->  | restricted |
| bow                | basic        | ->  | restricted |
| club               | skilled      | ->  | restricted |
| crossbow           | expert       | ->  | basic**    |
| dagger             | expert       | ->  | expert     |
| dart               | basic        | ->  | restricted |
| firearm            | expert       | ->  | n/a        |
| flail              | skilled      | ->  | expert     |
| hammer             | skilled      | ->  | skilled    |
| javelin            | skilled      | ->  | n/a        |
| long sword         | skilled      | ->  | basic**    |
| mace               | skilled      | ->  | skilled    |
| morning star       | skilled      | ->  | expert     |
| paddle             | skilled      | ->  | n/a        |
| polearms           | skilled      | ->  | skilled    |
| quarterstaff       | skilled      | ->  | restricted |
| short sword        | skilled      | ->  | basic**    |
| shuriken           | basic        | ->  | restricted |
| sling              | basic        | ->  | restricted |
| spear              | expert       | ->  | basic*     |
| unicorn horn       | skilled      | ->  | skilled    |
| whip               | expert       | ->  | basic**    |
| body spell         | skilled      | ->  | n/a        |
| cleric spell       | n/a          | ->  | basic      |
| escape spell       | n/a          | ->  | basic      |
| matter spell       | basic        | ->  | skilled    |
| protection spell   | skilled      | ->  | n/a        |
| bare handed combat | grand master | ->  | skilled**  |
| shield             | n/a          | ->  | skilled    |
| riding             | restricted   | ->  | skilled    |

** These skills have their max capability increased if the Undead Slayer starts with a related item in their inventory.


### Cartomancer
* The cartomancer is a unique role ported over from SpliceHack. Cartomancers are spellcasters with a focus on using cards and summoning temporary minions to do their bidding. Many parts of the role are inspired by or pay homage to various trading card games. The cartomancer has undergone some dramatic transformations from its original implementation in SpliceHack, becoming a more focused and surprising role to play.

**Starting inventory:**
    * graphic tee
    * 40 blessed +2 razor cards
    * ~4 meat sticks
    * ~4 candy bars
    * 7 blessed summon raven cards
    * 1 random rulebook
    * 4 potions of phasing
    * sack
    * a playing card deck

**Intrinsics:**

| XL  | Intrinsic                                        |
| --- | ------------------------------------------------ |
| 1   | Slow (speed 10)                                  |
| 1   | Searching                                        |
| 7   | Warning                                          |
| 7   | Can ascertain razor card enchantments            |
| 15  | Fast                                             |
| 15  | Can ascertain razor card and all scroll/card BUC |

**Skill adjustments for cartomancers (from SpliceHack):**

| skill              | SpliceHack | ->  | NerfHack   |
| ------------------ | ---------- | --- | ---------- |
| bare handed combat | skilled    | ->  | basic      |
| boomerang          | restricted | ->  | skilled    |
| sling              | skilled    | ->  | skilled    |
| dart               | expert     | ->  | skilled    |
| shuriken           | expert     | ->  | master     |
| unicorn horn       | restricted | ->  | expert     |
| dagger             | expert     | ->  | restricted |
| knife              | skilled    | ->  | restricted |
| axe                | basic      | ->  | restricted |
| short sword        | basic      | ->  | restricted |
| club               | basic      | ->  | restricted |
| mace               | basic      | ->  | restricted |
| quarterstaff       | basic      | ->  | restricted |
| polearms           | basic      | ->  | restricted |
| spear              | basic      | ->  | restricted |
| trident            | basic      | ->  | restricted |
| attack spell       | basic      | ->  | restricted |
| healing spell      | basic      | ->  | restricted |
| divination spell   | expert     | ->  | restricted |
| enchantment spell  | skilled    | ->  | restricted |
| cleric spell       | skilled    | ->  | restricted |
| escape spell       | skilled    | ->  | restricted |
| matter spell       | skilled    | ->  | restricted |
| riding             | expert     | ->  | restricted |
| wild magic         | expert     | ->  | n/a        |

**Quest artifact**
The **Holographic Void Lily** is a quest artifact that functions as a chaotic credit card. When carried, it grants energy regeneration, half spell damage and reflection. Additionally, it can be invoked to provide a temporary boost in card drops, during which the Void Lily will shine brightly for 25-50 turns. This invocation effect replaces the original #invoke ability from SpliceHack, where it previously summoned a large group of random monsters.

**Cartomancer terminology**
Whilst playing as a cartomancer, much of the standard NetHack terminology is revised:

| item               | renamed as          |
| ------------------ | ------------------- |
| scrolls            | "cards"             |
| spellbooks         | "rulebooks"         |
| credit cards       | "banned cards"      |
| boomerangs         | "bent cards"        |
| expensive cameras  | "holographic cards" |
| hawaiian shirts    | "graphic tees"      |
| lock picks         | "worthless cards"   |
| scrolls under $100 | "common"            |
| scrolls for $100   | "uncommon"          |
| scrolls for $200   | "rare"              |
| scrolls for $300   | "legendary"         |
* Whenever you or a monster reads a scroll, they instead "play" that card.

**Cartomancer rarity descriptions**
Scrolls are also labeled according to their rarity. In the original SpliceHack implementation, this reflected the price. So a $100 card would be "uncommon", a $200 card would be rare, and so on. With the nerfing of price identification, this system has been revised so that the actual probability of cards is reflected. The following chart describes how this works.

| Card            | Rarity | Description |
| --------------- | ------ | ----------- |
| cloning         | 10     | legendary   |
| charging        | 15     | legendary   |
| exile           | 15     | legendary   |
| taming          | 15     | legendary   |
| punishment      | 15     | legendary   |
| stinking cloud  | 15     | legendary   |
| earth           | 18     | rare        |
| food detection  | 25     | rare        |
| fire            | 30     | rare        |
| gold detection  | 33     | rare        |
| amnesia         | 35     | rare        |
| flood           | 35     | rare        |
| scare monster   | 35     | rare        |
| identify        | 40     | uncommon    |
| magic mapping   | 45     | uncommon    |
| destroy armor   | 45     | uncommon    |
| create monster  | 45     | uncommon    |
| confuse monster | 53     | uncommon    |
| teleportation   | 55     | uncommon    |
| enchant armor   | 63     | common      |
| remove curse    | 65     | common      |
| enchant weapon  | 80     | common      |
| light           | 90     | common      |
| knowledge       | 140    | common      |

**Card abuse penalties**
* Cartomancers receive severe alignment penalties for forging or defacing cards.
  - writing cards: -20 alignment, -5 luck
  - cloning cards: -20 alignment, -5 luck
  - polymorphing cards: -10 alignment, -2 luck

**Play mechanics**
* Cards (scrolls) only weigh 1 for cartomancers.
* Rulebooks (spellbooks) only weigh 5 for cartomancers.
* The camera is played as a holographic card for cartomancers, doesn't break when thrown.
* When applying a deck of cards, cartomancers will always be able to use them as if they
  were blessed.
  - For playing card decks, this enables you to easily evaluate your current luck.
  - For decks of fate, you will have a bonus toward a better result.
* Cartomancers don't break illiterate conduct when playing cards.

**No perma-pets**
Cartomancers do not receive a starting pet and are unable to tame monsters in the usual way. When food is thrown at domestic animals, it only pacifies them rather than taming them. Any figurines that generate are automatically converted into summon cards, and the rulebook of create familiar also produces summon cards instead of familiars. All standard methods of creating permanent pets have been nullified for Cartomancers. On the Astral Plane, they receive an archon card in place of a guardian angel. When reading a confused scroll of cloning, they will simply receive a summon card instead of a possible tame pet.

**Melee combat nerfs**
* Cartomancers are not great melee fighters - they prefer ranged weapons or fighting behind their summoned help. They have some severe penalties for melee combat.
* There is a flat -5 to-hit penalty for all melee combat.
* If wearing armor, they receive an additional -20 to-hit penalty
* If wearing a shield, they receive an additional -10 to-hit penalty
* If attacking with a wielded weapon, they receive an additional -10 to-hit penalty.
* Cartomancers get messages (similar to monks) for cumbersome armor and shields.

**Card drops**
When playing as a cartomancer, there is a chance that a monster will leave a card instead of a corpse upon death. Initially, this chance is 50%, but as you level up and progress deeper into the dungeon, the chance gradually decreases. When a monster dies and is eligible for a drop, one of three outcomes can occur: a razor card (with any BUC status or enchantment) may be dropped, a zap card may appear, or a summon card might be left behind. Summon drops are the most complex, as they can vary depending on RNG. The drop could be the same card as the monster that was killed, a higher difficulty monster, a random monster, or a sphere. If the monster is low level (below 3), it often doesn't leave any card. However, nasty monsters always drop their own summon cards.

* Some monsters are restricted from dropping cards:
  * spell beings
  * revived monsters (zombies and trolls that have been killed once and come back)
  * cancelled monsters
  * phoenixes (they always leave an egg)
  * cloned monsters (gremlins, blue jellies, etc.)
  * Keystone Kops (they can be farmed)
* Cartomancers don't get card drops whilst polymorphed.

**Spell beings**
Spell beings originally came from SLASH'EM. Whenever the flame sphere or freeze sphere spells were cast, they would summon a temporary sphere, which counted as a spell being. These beings are tame and act like pets, but they have a limited lifespan. (In SLASH'EM, there was no lifespan unless you left them on a level, causing them to become untame.) Here, when the cartomancer plays a summon card, it will summon a spell being with a predetermined lifespan that will fight aggressively for you, ignoring any hesitation a regular pet might exhibit and never stopping to eat or hide. If you receive credit for killing a spell being, they only grant 1 XP. Spell beings never leave corpses and spawn with no inventory. Spell-beings also don't count toward vanquished or special logged monsters.

Spell beings have a "sparkling" description in farlook, so you can distinguish them from permanent monsters.

**Lifetime of spell-beings:**

| XPLev | Turns |
| ----- | ----- |
| 1     | 19    |
| 5     | 35    |
| 10    | 55    |
| 15    | 75    |
| 20    | 95    |
| 25    | 115   |
| 30    | 135   |

**Summon cards**
For cartomancers, cards of create monster are twice as common as for other roles, and when these cards spawn, they are keyed to a specific summon monster card. Cartomancers begin the game with seven summon raven cards and have opportunities to expand their collection as they slay monsters. Whilst low-level monsters rarely drop their own summon cards, there is always a small chance that any death drop will leave a higher-level monster card. As the cartomancer's level increases, so does the strength of these rare drops.

The price of summon cards scales according to the difficulty of the monster they summon. In addition to reading summon cards, cartomancers can also throw them to activate the effect, which allows them to summon monsters at a distance, directly next to a threat.

Monsters can also read summon cards, so it’s important for cartomancers to collect them before they are used against them. Cursed summon cards will always create hostile monsters.

Activating summon cards costs 5 energy per card. If the cartomancer lacks enough energy, the card will have no effect and will not be consumed. Unique monsters can drop summon cards, with a few exceptions, such as the Wizard of Yendor and the Riders, due to their ability to revive. Additionally, cartomancers can receive summon cards by offering corpses. Although these cards do not count as artifact gifts they will still increase the prayer timeout.

**Explosive summon cards**
Summon "sphere" cards are special because they instantly explode when thrown at a monster. However, if cursed, they will not explode and instead summon a hostile sphere, which includes gas spores and volatile mushrooms. Exploding sphere monster cards are more likely to drop for cartomancers, providing them with useful ranged explosive options.

These monster cards are eligible for this mechanic:
* freezing spheres
* flaming spheres
* acid spheres
* shocking spheres
* stinking spheres
* volatile mushrooms
* gas spores

**Razor cards**
In **NerfHack**, razor cards have been properly implemented as their own weapon type, using the shuriken skill, unlike in **SpliceHack**, where they were simply renamed shuriken. Razor cards deal 1d6 damage to both small and large creatures, have a +2 to-hit bonus, and weigh 1. Cartomancers can multishot with shuriken-skill projectiles, such as shuriken and razor cards, and they gain multishot bonuses up to expert skill. However, they do not receive additional multishot bonuses at master skill level, though they still benefit from increased damage and to-hit bonuses.

Razor cards will occasionally appear as part of a cartomancer’s regular death drops, sometimes replacing summon or zap cards. These follow the same rules as stacked weapons, so they may appear in stacks of 6-11 and could be blessed, cursed, unblessed, or possibly even poisoned. The strength damage bonus applies exclusively to thrown razor cards, and no other projectile qualifies for this bonus.

If a player comes across a deck of cards that they have no use for, they can #tip the deck to empty it, yielding a potentially large stack of razor cards.

**Zappable cards**
Zap cards, which function as one-use wands, can drop when cartomancers kill monsters. These cards have a 0% generation chance for other roles, meaning only cartomancers will encounter them. Cursed zap cards have a chance to backfire like wands, but they cannot explode. Playing zap cards requires 5 energy per card.

Cartomancers will never see wands generate. Anytime a wand would spawn it is instead replaced with its equivalent zap card. It's important to note that monsters can and will use both zap and summon cards against the player, so it's crucial to collect them as soon as they drop.

**Spellcasting overhaul**
Cartomancers do not learn spells in the traditional way, meaning they cannot acquire spells from starting books, reading spellbooks, or receiving gifts from gods. Instead, they cast spells instantaneously by reading rulebooks. These rulebooks generate with 4-5 charges, and each reading consumes one charge. Once all charges are used, the rulebook is consumed and disappears.

Cartomancers begin the game knowing the identities of all rulebooks, as the title and purpose of a rulebook are typically clear from the cover. They always cast spells at expert level, ensuring high proficiency. Whilst rulebooks can still be written using magic markers without penalties (unlike when forging cards), they cannot be recharged with scrolls of charging. Additionally, cartomancers are fortunate enough to know braille, allowing them to invoke their rulebooks even while blind.

**Card combos:**
* The 'Z' spellcasting command is instead is used for card combos that the cartomancer gets access to as they level up.
* Card combos do not become available until level 5. You gain the ability to cast more cards as you level up:
  * level 5: 3 cards
  * level 10: 4 cards
  * level 15+: 5 cards
* Starting the combo costs 5 energy. Further cards cost 5 energy per card to play as normal.

**Cartomancers get special bonuses for wielding crystal balls:**
Whilst wielding a crystal ball, a cartomancer will enjoy:
  * max charisma
  * telepathy
  * see invisible
  * astral vision

**Changes to the cartomancer quest:**
* Created a unique duelist monster to take the place of students in the cartomancer quest.
* The cartomancer quest levels have received some updates and detailing.
* Buffed the King of Games and Dal Zethire.


## PLAYER RACE CHANGES


* Removed infravision from dwarves, elves, gnomes, and orcs.

### Elves
* Elves can always squeeze between two trees (xNetHack)
* Elves get see invisible at level 8
* Elves can always reach Basic in enchantment spells (xNetHack)

### Dwarves
* Dwarves can always reach Skilled in pick-axe (xNetHack)

### Gnomes
* Gnomes are good at slipping free from grabbing attacks
* Gnomes start with a nightvision radius of 2 (dNetHack)
* Gnomes start with an interesting tool
* Gnomes get stealth at level 5 (SLASH'EM)
* Gnomes get a damage bonus for shooting crossbows
* Gnomes can always reach Skilled in crossbow
* Gnomes can always reach Basic in club (xNetHack)

### Orcs
* Orcs cannot successfully engrave Elbereth.
* Orcs start with sickness potion (Sporkhack)
* Orcs get an alignment boost for cannibalism (dNetHack)
* Orcs can always reach Skilled in saber (xNetHack)
* Orcs start with -20 alignment
* Orcs don't get penalties for attacking and murdering peacefuls, even quest guardians or leaders.
* Orcs get alignment bonuses for attacking peaceful, helpless, or fleeing monsters.
* No extra monsters generate peaceful than necessary.
* Shopkeepers generate peaceful, but watch guards and watch captains will immediately pursue orcs on sight.
* Cross-aligned priests will generate hostile - however, priests of Moloch will generate peaceful.
* Orcs and watch guards have a grudge vs each-other.
* Orcs love drinking blood and get an alignment bonus and exercise constitution when doing so.
* Orcs cannot pacify or tame most monsters because they are just too evil. However, they do have the ability to pacify and tame a few monsters with food: goblins, wargs, trolls, ogres, and barghests.
* The range of monsters they can tame magically is reduced to these monster types: o O T D U
* Orcs get significant STR, CON, and DEX bonuses for leveling up.
* Orcs can saddle and ride wargs
* Orcs always start with a warg pup
* Orcs never get help on Astral and always receive an angry pack of Angels.
* Orcs also hate items made of mithril (this isn't the same mechanic as other variants where mithril does extra damage or prevents damage, they just find it uncomfortable to wear or wield)


### New race/role combos.

* Elven archeologist
* Orcish archeologist
* Elvish healer
* Dwarvish knight
* Dwarvish priest
* Orcish priest
* Elvish rogue
* Gnomish rogue
* Elvish tourist
* Gnomish tourist
* Dwarvish barbarian

### Racial item preferences

* Dwarves, elves, orcs, and gnomes get a -1AC bonus for each piece of racially aligned armor they wear (Evil/THEM).
* While wielding a racially aligned weapon, you get a +1 to-hit bonus (ie: a dwarf wielding a dwarvish spear).
* Wielding a racially aligned off-hand weapon also adds a +1 to-hit bonus.

* Monsters of certain races will usually prefer their own equipment and find other racial equipment awkward or uncomfortable to use.
  * Elves hate dwarvish, gnomish, and orcish objects
  * Orcs hate dwarvish, gnomish, and elven objects
  * Dwarves hate orcish, gnomish, and elven objects
  * Gnomes hate dwarvish, orcish, and elven objects
  * Humans and dhampirs hate gnomish objects - but otherwise they are free to use all other racial equipment

The effects of wearing armor or wielding weapons you hate:
* +3AC penalty for each piece
* -d5 to-hit penalty for each piece
* You receive an explicit message when wearing or wielding any hated object.
* You'll also receive periodic messages when fighting to remind you your to-hit is suffering.
* When throwing items your race dislikes, they have a 1 in 7 chance of slipping - the same as a cursed or greased projectile.

This mechanic also applies to monsters, but they will simply avoid using items they don't like.


## NEW RACES


### Dhampir

Vampires have a rich history in NetHack, first appearing in SLASH'EM and later in UnNetHack, dNetHack, SpliceHack, and Hack'EM, with each variant implementing them slightly differently. However, in NerfHack, vampires take a U-turn from the traditional design due to their overwhelming power. As a playable race, they allowed players to bypass too many core mechanics and obstacles, including newly introduced features.

For instance, their **immunity to withering** made mummies and priests trivial threats, while **immunity to rabid attacks** negated an entirely new mechanic. **Poison resistance** let them fight deadly monsters like orcs or team a without fear, and **sleep resistance** nullified sleep rays. Beyond resistances, their innate abilities made the game even easier: their hardcoded vampire-bat and fog cloud polyforms rendered polytraps meaningless, **flying** allowed them to **bypass ground traps, water, and icy floors**, and **regeneration** gave them an immense edge in combat. All of these factors stripped away much of the game's intended challenge, particularly in the early stages.

**A Balanced Alternative: The Dhampir**

To address these issues, a **lesser type of vampire—the Dhampir (or demi-vampire)**—was introduced. This new race retains some of the vampire's strengths but is far more balanced, fitting alongside other vanilla races. The Dhampir preserves the appeal of playing as a vampire while maintaining the integrity of NerfHack's mechanics and difficulty.

Dhampirs start with **resistance to draining and death magic**, and being **breathless**, they are immune to gas, spores, choking, and drowning. They also resist **lycanthropy** and possess **infravision**. However, **all partial intrinsics are capped at 50%**, even when granted through crowning, ensuring they rely more on extrinsic protections.

Dhampirs **excel at climbing** and can easily escape pits. Their standout ability is a **1d6 draining bite**, which **heals HP** when feeding on blood — replacing the vampire's intrinsic regeneration. As an added bonus, they can **absorb partial intrinsics from drained monsters**, such as **fire, cold, and sleep resistance**.

To prevent frustrating deaths, **bite attacks are automatically prevented** when facing dangerous foes such as **cockatrices, Medusa, or green slimes** — even if the player is only polymorphed into a vampire. However, **stunned, confused, or hallucinating dhampirs and vampires will bite indiscriminately**, making careful gameplay crucial when impaired.

Dhampirs also come with a major weakness — **innate hunger**. This forces players to stay aggressive, attack often, and keep draining blood for nutrition. The corpse draining mechanic from SLASH'EM was never ported due to bugs in the nutrition code and tedious corpse draining mechanics. Instead, SpliceHack's approach was adopted, where **life blood feeding in combat now provides more nutrition**. The tradeoff is that **Dhampirs can no longer eat nor gain benefits from eating corpses**.

#### NerfHack introduces smarter feeding to regulate vampire bite mechanics:
- Low-level dhampir can only use either a bite attack or weapon attack, but not both in the same round.
- If the vampire is hungry (or close to hungry), they will always bite and attempt to feed first.
- Otherwise, there is a 50/50 chance of either biting or attacking with a weapon.
- The ability to combine a bite with a weapon attack is locked until Level 10.
- After **Level 9**, dhampir can perform **both biting and weapon attacks in the same round**.
- If a player **wants to avoid biting**, they can forcefight using `"F"` to **only use their weapon attack**.
- Dhampir also feed more efficiently when their victims are confused, incapacitated, or trapped.

**The Dazzle Technique:** Dhampir also inherit the vampire's dazzle tech from SLASH'EM. This is available from level 1 and allows the dhampir to attempt a paralyzing gaze on an adjacent monster. At low levels this will be quite weak, but as you gain levels and attempt it on weaker monsters it will become more effective. For the player's convenience, a rough estimate of success is accessible in the monster pokedex for each monster. Since monsters can spawn with a range of levels or gain levels in gameplay, the lookup only uses a monster's base level.

#### Dhampir's resistances and abilities

| XL  | Intrinsic                   |
| --- | --------------------------- |
| 1   | Infravision                 |
| 1   | Warning vs humans and elves |
| 1   | Breathless                  |
| 1   | Drain resistance            |
| 1   | Immune to death magic       |
| 1   | Immune to lycanthropy       |

Although dhampir have drain level resistance, they remain **vulnerable to blood-draining bite attacks** from other vampirics and blood-suckers. Intrinsic drain resistance does not protect against these attacks, but an extrinsic source, such as the Stormbringer, will.

In terms of food, **most rations and fruit juice potions are replaced with blood potions** when playing as a dhampir. This avoids creating junk items throughout the game and helps the player survive longer. Some vampires receive an opera cloak, though it is rarer than in SLASH'EM, and **wearing an opera cloak grants a charisma bonus**, as in UnNetHack. Potions of blood and vampire blood offer vampires a drinkable food source. Dhampir can use any racial items, except for gnomish items, which are too small for them.

**Silver weapons also generate more frequently** when playing as a dhampir. After difficulty level 8 kicks in, 10% of all eligible weapons will be converted to silver. Dhampir can handle silver items, but if they come into direct contact (ie: wielding a silver saber without gloves), they will take some damage and be unable to regenerate further HP.


### Grung

**Grung** are a nasty little race of frog-like people known for their toxic skin, sharp teeth, vibrant colors, and lack of long tongues. The featured race here is the green grung. Their **skin naturally secretes poison**, giving them a **passive poison attack**. In combat, they can **poison enemies when striking barehanded**. Although their poison is only about half as strong as a standard poisoned weapon attack, it is still very efficient at wiping out enemies that don't resist poison. Additionally, they can **poison their weapons using their toxic skin** to coat them with venom for extra lethality.

Grung possess several natural abilities. They have **resistance to poison** and are adept at **searching**. Their natural agility allows them to **swim effortlessly**, and as they gain experience, they achieve **jumping ability (XP5)** and **speed (XP7)**.

#### Grung's resistances and abilities

| XL  | Intrinsic         |
| --- | ----------------- |
| 1   | Poison resistance |
| 1   | Searching         |
| 1   | Swimming          |
| 5   | Jumping           |
| 7   | Fast speed        |


One of the grung's **biggest concerns is hydration**.

#### Grung Hydration Mechanics

- **Hydration Requirement:** Grung **must stay wet to survive**
- **Hydration Timer:** Starts at **6000** and counts down every turn
- **Penalties for Low Hydration:**
  - Below **1000** → **Speed and combat penalties**
  - At **0** → **Instant death**
- **Dehydration Accelerators:**
  - **Fire, heat, and dry environments** speed up dehydration
  - **Fire resistance** can **reduce some effects**
- **Methods of Rehydration:**
  - **Drinking water**  (+100-199)
  - **Sitting in water sources**  (+100-199)
  - **Being splashed with water**  (+100-199)
  - **Submerging in water** restores **1000 hydration per turn**
- **Scrolls of Flood:**
  - Can be used for **rapid hydration**  (+4500-6000)
  - If **read while confused**, they cause **severe dehydration** instead
- **Environmental Effects:**
  - Faster dehydration in Gehennom & the Plane of Fire
  - Easy rehydration in the Plane of Water
- **Prayer for Hydration:**
  - If hydration drops to **250 or below**, it counts as **major trouble**
  - **Praying** may grant **1000 hydration**, if your **god blesses you**


Grung have several strengths in combat. Their **DEX-based armor class (AC) bonus** is **slightly increased and doubled** compared to other races. They also gain a **to-hit bonus against kamadan** and can **always reach skilled proficiency in darts**. However, they also have notable weaknesses. They **cannot wear boots** and strongly **dislike heavy or bulky armor**, though they are comfortable wearing racial armor as long as it isn’t cumbersome — mithril is a good choice. Additionally, their **passive poison ability does not function** while wearing **bulky armor**. Grung are particularly vulnerable to **dust vortices**, which accelerate their dehydration process.

**Playable Roles & Alignments**
Grung can be played as **neutral** or **chaotic** characters. They can take on these roles:
- **Archeologist**
- **Barbarian**
- **Monk**
- **Priest/Priestess**
- **Rogue**
- **Ranger**
- **Wizard**

Beyond the green grung, there are other members of the grung clan, each with slightly different abilities and strengths. Grung come in **six colors**:
- **Green grung** possess passive and active poison that drains strength.
- **Blue grung** drain constitution with their poison and can cast mage spells.
- **Purple grung** have a stunning poison and can cast clerical spells.
- **Red grung** poison their enemies by draining dexterity and wield a 2d6 weapon attack.
- **Orange grung** cause hallucinations with their poison and have a 1d6 weapon attack.
- **Gold grung** induce sleep with their poison and wield a powerful 2d6 weapon attack.


## SPELLCASTING CHANGES


Most of these changes are to strengthen natural spellcasters abilities and to dull roles
that don't specialize (like fighters). Non-specialists can still attempt to utilize spells
but they will have to work harder to maintain their spells. Cavemen will have a very
difficult time with spellcasting.

### Spell memory
* The base memory retention ("KEEN") for spells is now 20000 turns for primary spellcasters and 10000 for all other roles.
* When reading or re-reading a spellbook, you will bring the retention back up to your role's KEEN value.
* Reading restricted spellbooks only grants **half** of your role's KEEN value.
* Primary spellcasters (healers, priests, monks, wizards, archeologists) get a memory boost of 500 turns when they cast spells (SLASH'EM).
* Casting your **special spell** also grants a retention bonus of 500 turns no matter what role you are

### Other spellcasting changes
* Removed the spellbook of identify (xNetHack)
* Wielding a quarterstaff provides a small bonus to spellcasting (about a 1/3rd of the bonus a robe confers) (Fourk)
* Hungerless casting ignores too hungry to cast penalty (xNetHack)
* Spellbooks' weight is directly related to their level (xNetHack)
* When casting a SKILLED attack spell, you can choose to cast basic fireball or cone of cold (xNetHack/dnh)
* You get a 100 turn reminder for spells that are close to fading away
* Spellcasting no longer exercises wisdom (FIQHack)
* Total hungerless casting is not possible anymore and the intelligence requirements have been increased. (FIQHack)
* Only primary spellcasters can receive divine spellbook gifts
* Spellbooks can generate pre-read
* Display a single accurate spellcasting retention percentage in the spellbook list
* Hide spells that are at 0% retention in the casting menu.

### New skill-dependent spell ranges
* Your skill in a spell directly affects how far its ray or beam will travel:

| Spellbook       | Unskilled | Basic | Skilled | Expert |
| --------------- | --------- | ----- | ------- | ------ |
| cancellation    | 2-8       | 7-13  | 9-13    | 11-13  |
| charm monster   | 1-4       | 2-8   | 7-13    | 7-13   |
| cone of cold    | 2-8       | 7-13  | 9-13    | 11-13  |
| dig             | 1-4       | 2-8   | 7-13    | 7-13   |
| drain life      | 1-4       | 2-8   | 7-13    | 7-13   |
| finger of death | 2-8       | 7-13  | 9-13    | 11-13  |
| fire bolt       | 1-4       | 2-8   | 7-13    | 7-13   |
| fireball        | 2-8       | 7-13  | 9-13    | 11-13  |
| force bolt      | 1-4       | 2-8   | 7-13    | 7-13   |
| knock           | 1-4       | 2-8   | 7-13    | 7-13   |
| polymorph       | 2-8       | 7-13  | 9-13    | 11-13  |
| sleep           | 1-4       | 2-8   | 7-13    | 7-13   |
| slow monster    | 1-4       | 2-8   | 7-13    | 7-13   |
| wizard lock     | 1-4       | 2-8   | 7-13    | 7-13   |


### Spell changes and updates

| Spellbook      | Notes                                                                                                                                                                                              |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| charm monster  | now a directional level 3 spell; <br/>only works on the first monster hit. <br/>At unskilled, the spell can only pacify monsters. <br/>At expert, you get 2 chances to tame each affected monster. |
| clairvoyance   | At skilled, the effect will persist for a while                                                                                                                                                    |
| cone of cold   | Moved to the Matter school (SLASH'EM)                                                                                                                                                              |
| create monster | Increased from level 2 to level 4<br/>Only creates spell beings at unskilled and basic levels.                                                                                                     |
| cure sickness  | Cure sickness is now directional and can be used to cure pets or other monsters (EvilHack)                                                                                                         |
| dig            | Lowered from a level 5 spell to level 3                                                                                                                                                            |
| drain life     | Increased from level 2 to level 3 (xNetHack)<br/>Now shoots a ray instead of a beam<br/>At expert, there is a 10% chance of firing an explosive ball of necrotic energy on each cast.              |
| fireball       | Moved to the Matter school (SLASH'EM)                                                                                                                                                              |
| food detection | Dhampir always detect potions with food detection spells and scrolls.                                                                                                                              |
| haste self     | At unskilled, same effect as a diluted potion of speed                                                                                                                                             |
| invisibility   | unskilled = diluted potion of invisibility                                                                                                                                                         |
| knock          | Cannot be used to escape from an engulfer (this ability is retained for the wand of opening)                                                                                                       |
| levitation     | unskilled = diluted potion of levitation                                                                                                                                                           |
| magic missile  | damage scales with skill                                                                                                                                                                           |
| sleep          | Lowered to level 2                                                                                                                                                                                 |
| poison blast   | Was level 4 in SLASH'EM, raised to level 5                                                                                                                                                         |
| lighting       | Was level 4 in SLASH'EM, raised to level 5                                                                                                                                                         |
| fire bolt      | Moved to the Attack school<br/>stops after the first monster hit<br/>Updated damage bonuses                                                                                                        |
| healing        | Healing spell effectiveness is determined by skill (EvilHack)                                                                                                                                      |
| extra healing  | Healing spell effectiveness is determined by skill (EvilHack)                                                                                                                                      |

**spellbook of fire bolt**
The damage calculations have been revamped from HackEM:
* Base damage is 1d10 fire damage
* At skilled it deals 2d10 fire damage
* At expert it deals 3d10 fire damage
* At level 5 it deals an additional +1d4 damage
* At level 11 it deals an additional +1d4 damage
* At level 17 it deals an additional +1d4 damage
* If the target resists cold a bonus +7 damage is applied.

This means if the player has maxed out their attack spell skill and leveled up to XP21, they could be dealing 3d10+3d4 with a level 1 spell.


**spellbooks of healing and extra healing**
* Healing power scales with skill level

| spell         | Unskilled | Basic | Skilled | Expert |
| ------------- | --------- | ----- | ------- | ------ |
| healing       | 4d4       | 6d4   | 8d4     | 10d4   |
| extra healing | 4d8       | 6d8   | 8d8     | 10d8   |


**spellbook of light**
* Spell of light's diameter of effect scales with spellcasting ability.
* For reference, the uncursed scroll of light always illuminates a radius of 11.

|       | Unskilled | Basic | Skilled | Expert |
| ----- | --------- | ----- | ------- | ------ |
| range | 1         | 3     | 5       | 7      |

**spellbook of magic mapping**

* The effectiveness of magic mapping depends on your spellcasting ability. The spell will never fully map a level, only the scroll can be depended upon for that.
* Lowered from level 5 to level 4
* Unskilled acts like a confused magic mapping (1 in 7 squares successfully mapped)
* Basic maps 1 in 5 squares
* Skilled maps 1 in 3 squares
* Expert maps all squares

**spellbook of magic missile**

Damage scales with level. Unskilled now deals half the damage expert can.

|       | Unskilled    | Basic        | Skilled      | Expert       |
| ----- | ------------ | ------------ | ------------ | ------------ |
| range | ((XL/2)+1)d3 | ((XL/2)+1)d4 | ((XL/2)+1)d5 | ((XL/2)+1)d6 |

## DUNGEON CHANGES


* Extended the main dungeon by 5 levels.
* Removed the **mysterious force** from the game (xNetHack)
* **Branchport** always brings you to the entry level of a branch
* The Rogue level has been disabled (many variants)
* Chickatrices and cockatrice eggs will now appear in cockatrice nests (xNetHack)
* Shops cannot have themed rooms with unusual floor textures (xNetHack)
* Random scroll shops cannot be big rooms
* Allow delis to buy and sell tin openers.
* No special **themed rooms** generate until level 3
* Random rivers were added to many of the quest filler levels
* Trees can generate in dungeon rooms (xNetHack)
* Trees on special levels are generate pre-looted (they cannot be kicked for killer bees or fruits)
* Trees can be destroyed by fire, cold, and disintegration rays. If a tree is destroyed by fire or cold, it has a 1 in 3 chance of exploding - possibly creating a chain reaction
* Random secret doors are secret less of the time (xNetHack)
* Random secret corridors have been removed (xNetHack)
* Removed the "temple of the gods" theme room. This room contains 3 altars, one of each alignment. It was removed to make the finite altars mechanic more relevant.
* There is a guaranteed thing from below guarding Rodney and chance of a vampire mage as well.
* Thrones can grant knowledge of magical items.
* Throne can summon much larger audiences when that #sit effect is hit.
* Guaranteed pit trap just outside of wizard's zoo.
* Courtrooms generated after level 20 can be filled with vampires (dNetHack).
* Gnomish mines fill levels sometimes have varied lighting; rarely they get ice patches.
* Fake "Closed for inventory" shop engravings can appear in random places.
* Pits can appear in morgues (from xNetHack)

### New levels

* All original Vanilla Sokoban levels have been removed and replaced.

| Level                 | Version                              | Source             |
| --------------------- | ------------------------------------ | ------------------ |
| Asmodeus' lair #2     | river/lava                           | SpliceHack         |
| Baalzebub's lair #2   | marsh                                | SpliceHack         |
| Baalzebub's lair #3   | variation on #1 with lava            | UnNetHack/NerfHack |
| Bridge of Khazad-Dum  | directly after the VotD              | UnNetHack          |
| Orcus Town #2         | river runs through                   | Lethe patch        |
| Castle #2             | lake surrounds castle                | UnNetHack/EvilHack |
| Castle #3             | lava river                           | UnNetHack/EvilHack |
| Demogorgon's lair #1  | enclosed in hell-maze                | SLASH'EM           |
| Demogorgon's lair #2  | two towers                           | Lethe patch        |
| Demogorgon's lair #3  | fortress with river                  | Grunt/EvilHack     |
| Dispater's lair #1    | enclosed in hell-maze                | SLASH'EM           |
| Dispater's lair #2    | the city of dis                      | Lethe patch        |
| Dispater's lair #3    | fortress with river                  | Grunt              |
| Geryon's lair #1      | enclosed in hell-maze                | SLASH'EM           |
| Geryon's lair #2      | the isle of Erytheia                 | Grunt              |
| Mephistopheles' lair  | fortress with river                  | SpliceHack         |
| Moloch's Sanctum #2   | lava islands                         | UnNetHack/EvilHack |
| The Lost Tomb #1      | tomb.des from SLASH'EM (**)          | SLASH'EM           |
| The Lost Tomb #2      | demogorgon's lair from xNetHack (**) | xNetHack           |
| Mine end #4           | the gnomish sewer                    | xNetHack           |
| Mine end #5           | orc temple                           | EvilHack           |
| Mine end #6           | gnome king's apiary                  | SlashTHEM          |
| Mine end #7           | boulder bonanza                      | SlashTHEM          |
| Minetown #8           | zoo town                             | Sporkhack/EvilHack |
| Minetown #9           | lavender town                        | SpliceHack         |
| Minetown #10          | mini-castle town                     | SlashTHEM          |
| Minetown #11          | creek town                           | SlashTHEM          |
| Minetown #12          | forge town                           | NerfHack           |
| Moloch's Temple #1    |                                      | SLASH'EM           |
| Moloch's Temple #2    | variation on #1                      | NerfHack           |
| Sokoban 1-1           | 1-4 from SLASH'EM                    | SLASH'EM           |
| Sokoban 1-2           | 1-3 from SLASH'EM                    | SLASH'EM           |
| Sokoban 1-3           | Dragon_of_Bactria                    | NetHack Fourk      |
| Sokoban 1-4           | 1-7 from Fourk                       | NetHack Fourk      |
| Sokoban 1-5           | 1-4 from Fourk                       | NetHack Fourk      |
| Sokoban 1-6           | 1-5 from Fourk                       | NetHack Fourk      |
| Sokoban 1-7           | 1-6 from Fourk                       | NetHack Fourk      |
| Sokoban 1-8           |                                      | GruntHack          |
| Sokoban 1-9           |                                      | GruntHack          |
| Sokoban 2-1           | 2-5 from SLASH'EM                    | SLASH'EM           |
| Sokoban 2-2           | 2-7 from SLASH'EM                    | SLASH'EM           |
| Sokoban 2-3           | 2-3 from SLASH'EM                    | SLASH'EM           |
| Sokoban 2-4           | 2-4 from SLASH'EM                    | SLASH'EM           |
| Sokoban 2-5           | 2-6 from SLASH'EM                    | SLASH'EM           |
| Sokoban 2-6           | 3-9 from Fourk                       | NetHack Fourk      |
| Sokoban 3-1           | 3-5 from SLASH'EM                    | SLASH'EM           |
| Sokoban 3-2           | 3-3 from SLASH'EM                    | SLASH'EM           |
| Sokoban 3-3           | 3-4 from SLASH'EM                    | SLASH'EM           |
| Sokoban 3-4           | 3-6 from SLASH'EM                    | SLASH'EM           |
| Sokoban 3-5           | 3-7 from SLASH'EM                    | SLASH'EM           |
| Sokoban 3-6           |                                      | GruntHack          |
| Sokoban 3-7           |                                      | GruntHack          |
| Sokoban 3-8           | 2-8 from Fourk                       |                    |
| Sokoban 4-1           | 4-3 from SLASH'EM                    | SLASH'EM           |
| Sokoban 4-2           | 4-4 from SLASH'EM                    | SLASH'EM           |
| Sokoban 4-3           | 4-5 from SLASH'EM                    | SLASH'EM           |
| Sokoban 4-4           | 3-6 from SLASH'EM                    | SLASH'EM           |
| Sokoban 4-5           | 3-7 from SLASH'EM                    | SLASH'EM           |
| Sokoban 4-6           | 3-15 from UnNetHack                  | UnNetHack          |
| Sokoban 4-7           |                                      | GruntHack          |
| Sokoban 4-8           | 3-2 from NetHack Fourk               | NetHack Fourk      |
| Sokoban 5-1           | 4-3                                  | SLASH'EM           |
| Sokoban 5-2           | 4-4                                  | SLASH'EM           |
| Sokoban 5-3           | 4-5                                  | SLASH'EM           |
| Sokoban 5-4           | 3-4                                  | UnNetHack          |
| Sokoban 5-5           | 3-5                                  | UnNetHack          |
| Sokoban 5-6           | 4-3                                  | NetHack Fourk      |
| Sokoban 5-7           | 4-7                                  | NetHack Fourk      |
| Sokoban 5-8           | 4-10                                 | NetHack Fourk      |
| Valley of the Dead #2 | river runs through                   | UnNetHack/Lethe    |
| Yeenoghu's lair #1    | enclosed in hell-maze                | SLASH'EM           |
| Yeenoghu's lair #2    | fortress in marsh                    | Lethe patch        |
| Yeenoghu's lair #3    | fortress with river                  | Grunt              |
| Oracle #2             |                                      | xNetHack           |
| Oracle #3             |                                      | xNetHack           |
| wizard1               | wizard1 from Evil (**)               | EvilHack           |
| wizard2               | soko1-1 or soko1-2 (**)              | NetHack            |
| wizard3               | wizard1 from xNetHack                | xNetHack           |
| wizard4               | wizard2 from xNetHack (**)           | xNetHack           |
| wizard5               | wizard2 from Evil (**)               | EvilHack           |
| wizard6               | wizard3 from Evil (**)               | EvilHack           |
| wizard7               | palace_e from UnNetHack (**)         | UnNetHack          |
| tower1                | tower1 from EvilHack (**)            | EvilHack           |
| tower2                | tower2 from EvilHack (**)            | EvilHack           |
| tower3                | tower3 from EvilHack (**)            | EvilHack           |

(**) - With light-to-extensive modifications from it's original version

### New themed rooms
* Ported kitchen themed room from SpliceHack/xNetHack
* Ported most of the new themed rooms from xNetHack
  * Four connected rooms
  * Barbell-shaped room, horizontal
  * Barbell-shaped room, vertical
  * Graffiti room
  * Boomerang-shaped, rot 1
  * Boomerang-shaped, rot 2
  * Rectangular walled corridor
  * Storeroom vault
  * Crossed X of water (now lava)
  * Mini maze
  * Bunch of closets
  * Beehives
  * Super Honeycomb
  * Swimming pool
  * Anti swimming pool
  * Thin long horizontal room
  * Scummy moldy room
  * Ozymandias' Tomb
  * Gas spore den
  * Four-way circle-and-cross room
  * Four 3x3 rooms, directly adjacent
  * Prison cell
  * Mirrored obstacles
  * Triple rhombus
  * Spiral
  * Abandoned shop
  * Irregular anthole
  * Water temple
  * Tiny cage, big monster
  * Room with small pillars
  * Dragon hall

New themed rooms introduced in NerfHack:
  * piercer room
  * room with random lava

### Shop Changes
* Shopkeeper's real name may be used in cursing shoplifters message (xNetHack).
* Improved the chances of some of the minetown shops appearing.

**Lighting shops:**
* Magic lamps will never appear in lighting shops. Instead, magic candles take their place.

**New shop: Junk Shop**
* Ported from SpliceHack
* This counts as a general store that is usually pre-populated with a bunch of junky items.

**New shop: Collectible Card Game Company**
* Brand new debuting in NerfHack!
* This shop only spawns for cartomancers and features a large variety of summon cards, with the occasional deck box or backpack. Takes the place of most food and weapon shops.

### Castle changes

* The castle level is now marked as a graveyard
* Castle barracks may open into courtyard instead of throne room, letting soldiers flood the courtyard more quickly (xNetHack)
* Added iron bars to the castle perimeter
* Iron bars have been added to the castle towers (Sporkhack)
* The location of the chest containing the scroll of wishing has been obfuscated. You will find matching chests and scrolls in each of the towers if you use object detection. The other chests have wands of nothing inside (Sporkhack)
* The drawbridge passtune range has been expanded by one square (xNetHack)
* The drawbridge also does not always close with the passtune, one out of five times it will malfunction when trying to close it (xNetHack)
* Castle courtyards are unlit
* The castle gets a guaranteed forge.
* Added a dragon lair to castle-3.

### Valley of the Dead

* Players can't regenerate hit points whilst in the Valley of the Dead (EvilHack)
* Instead of dart traps, the player will encounter magic traps (EvilHack)
* Less ghosts spawn to clog up the valley


### Enhanced Gehennom

* The second fake wizard level has been removed.
* The portal to the Wizard's Tower can appear in Gehennom levels 10-17.
* The wizard's tower has been extracted to its own branch (xNetHack/EvilHack)
* Marked the Asmodeus levels as cold and added cold traps
* Juiblex's lair gets some puddles and a shoggoth
* Random item generation has roughly cut in half for Gehennom fill levels.
* The structure of Gehennom now follows the SLASH'EM template.
  * Gehennom spans 19-21 levels
  * All demon lairs are guaranteed to appear with their demons
  * Level 1: The Valley of the Dead
  * Level 2: The Bridge
  * Levels 3-9: Stairs to Vlad's Tower
  * Levels 3-7: Juiblex's lair
  * Levels 3-7: Yeenoghu's lair
  * Levels 3-7: Orcustown
  * Levels 3-7: Demogorgon's lair
  * Level 9: Portal to the wizards tower
  * Levels 10-15: Dispater's lair
  * Levels 10-15: Geryon's lair
  * Levels 10-15: Asmodeus' lair
  * Level 16: Vibrating Square - now has it's own dedicated level.
  * Level 17: Moloch's Sanctum

### The Wizard's Tower Overhaul
* NerfHack borrows from other great variants to create the biggest and baddest tower that Rodney could ever reside in.
* The Wizard's Tower has been expanded to a staggering 7 levels high to provide a highly challenging penultimate test.
* Level 7: wizard1 from EvilHack and where the Wizard of Yendor awaits.
* Level 6: Return of Sokoban: it's an evil version of Sokoban from vanilla NetHack - the Wizard is certainly cruel isn't he... and no prizes either :(.
* Level 5: wizard1 from xNetHack - fight your way through a honeycomb of randomly generated chambers.
* Level 4: wizard2 from xNetHack - the teleportation maze, now scaled back a bit.
* Level 3: wizard2 from EvilHack - now featuring a nest of nasty petrifying monsters.
* Level 2: wizard3 from EvilHack - can you withstand a storm of fire, ice, and explosive migos?
* Level 1: This is the entry to the wizard's tower. It was previously the bottom level of UnNetHack's Sheol branch and features the Executioner who will kindly Cleave (I mean greet) you.

### Vlad's Tower revamp
* This ports the updated and enlarged levels for Vlad's from EvilHack (except for the caverns which will come later).
* Some flair was added to the levels to further torture players.
* To make this a strategic nightmare, lots of iron bars and small niches were added that act as prisons. In these prisons are placed the most annoying gazing and ranged monsters to distract the player while vampires flank them from all sides.
* All levels of Vlad's Tower are fully lit.

### Sokoban

* Sokoban levels are cold and icy - legend has it a white dragon named Wintercloak took the tower over, leaving a trail of frost in its wake. In addition to the level being colored blue with splashes of icy cyan, you will see random patches of ice form in the level. Because they are cold, if potions land on the floor, they have a chance of freezing and shattering.
* Note: A recent change from NetHack 3.7 also makes ice occasionally slide the player in a random direction.
* Sokoban now has two additional levels - an entry level with river obstacles (adapted from the town filler level from UnNetHack) and another puzzle level to solve.
* Monsters are never generated peaceful in Sokoban (FIQHack)
* Zombies don't revive in Sokoban and they won't dig out of the ground.
* Monsters won't break boulders in Sokoban with pick-axes or mattocks, or spellcasting.
* All the vanilla sokoban levels have been replaced with the SLASH'EM puzzles.
* The Dragon of Bactria level was added from NetHack Fourk; the green dragon was replaced with a white dragon
* All Sokoban zoos have the white dragon guarding the treasure.
* The zoos in Sokoban have been expanded slightly.
* Flavored most Sokoban levels with more iron bars.
* Decorated the levels with white dragon statues in honor of the new steward.
* In addition to the amulet and bag, the Sokoban prize can also be a cloak of magic resistance or a magic marker.
* Sokoban prizes are always erodeproofed.
* Stop Sokoban guilt after acquiring the prize.
* The iron bars in some of the Sokoban levels can be phased through, but it now incurs a Luck penalty.
* You will now receive a message when incurring a Sokoban Luck penalty.
* Sokoban maps above puzzle #2 get 2 mimics.
* Almost all Sokoban levels ensure a spare boulder in case of mistakes or misfortune.

### Fort Ludios
* The portal to Fort Ludios is placed in the first eligible vault generated (xNetHack/UnNetHack).
* Ported two Fort Ludios variants (EvilHack/UnNetHack)
* Some mermaids were added to patrol the moats.

### Minetown/Mines End
* Ported zoo town and lavender town (SpliceHack)
* Ported Creek Town and Mini-Castle town (THEM)
* Imported the Gnomish Sewer (xNetHack)
* Imported 3 mines end variants (THEM)
* Created a new minetown called "forge town"

### Oracle
* The Oracle level now appears from levels 8-11.
* Ported Oracle variations 2 and 3 (SpliceHack)
* Allow dungeon features to generate in the Oracle level.
* An altar always appears on the Oracle's level.

### Temple to Moloch level
* Ported from SLASH'EM
* Gargoyles replace the statue gargoyles in the original map
* Winged gargoyles replace 4 of the original gargoyles
* 2 ghoul mages were added

### Lost Tomb level
* Ported from SLASH'EM - this level now has some additional rooms (and treasures) with randomized passages.
* A second variation was created using Demogorgon's Lair from xNetHack. This level had a very mazelike structure that lends itself well to a lost tomb (but with no Demogorgon of course...).
* Both lost tomb levels are no-teleport

### The Wyrm Caves
* Ported from SLASH'EM as it was
* This level offer the player a small but difficult branch. There may be the promise of dragon scales in addition to various loot.
* Occurs from levels 20-21

### Big Room
* Ported bigroom variants from UnNetHack and SpliceHack.
* Imported two bigroom variants from xNetHack.
* An additional big room was added to the latter half of the main dungeon (SpliceHack)

### Grass
* Ported using code from xNetHack, SpliceHack, and HackEM.
* Monsters can hide under grass (xNetHack).
* You cannot dust engrave on grassy tiles.
* Burned engravings also burn up grass.
* Walking on grass makes you more stealthy.
* Herbivore pets will eat grass (EvilHack)

### Puddles
* Ported from EvilHack and SlashTHEM.
* Puddles act as a nerf for early water sources by limiting a useful resource for diluting and blanking items.
* Many pools are replaced with puddles instead.
* Fountains gush out puddles instead of pools
* Disarming a rust trap results in a puddle instead of a fountain
* Scrolls of flood mostly create puddles instead of pools (unless cursed)
* Whetstones can be used in puddles and can dry up puddles.
* Tiny monsters can drown in puddles (relevant if polymorphed into one)

### Forges
* Forges were ported in from EvilHack
* Forges let the player repair metallic armor, bless items, dispose of zombies or organic items, dispose of the iron ball and chain, and summon lava demons and fire elementals.
* Forging recipes are available in the object lookup
* Weapons can be forged by applying a hammer whilst standing on a forge.
* Items can pass over forges.
* New forging feature: There is a one-time 1 in 30 chance of erodeproofing an item when dipping in a forge. After this occurs, the forge will instead emit a puff of steam.
* Forges always light up the square they occupy.
* Cold rays have a chance cool forges.
* Forges burn the grease and poison off dipped items.
* You cannot forge while confused, stunned, hallucinating, weak from hunger, or with STR under 4.

#### Forging and Forging Recipes
* Ported from EvilHack with modifications.
* No artifact forging
* No armor recipes are available if you aren't a dwarf or orc.
* Much narrower list of forgeable weapons, mostly bladed and blunt weapons.
* Only samurai can forge katanas, tsurugi, and shuriken.
* Only dwarves can forge dwarvish items
* Only orcs can forge orcish items
* Forging recipes are displayed in the object lookup.

Aside from the recipe changes - the biggest change is that we no longer have a #forge or #craft command. Simply get a hammer and apply it when standing over a forge.

### Toilets
Toilets have received many enhancements after adapting them from SLASH'EM. Notably, toilets can now appear on their own, separate from sinks, whereas in SLASH'EM, they only came in pairs with sinks. Overall, their frequency has been dialed way back so they are quite rare.

* Toilet prayer can now stop the vomiting process
* Praying at toilets can cure sickness.
* Sitting on toilets can alleviate satiated status.
* If giants sit on toilets, they break.
* Sitting on toilets fully heals your HP.
* Toilets can sometimes break when sat on.
* Dipping potions into toilets only contaminates potions into sickness.

#### Toilet kicking:
* Like sinks, toilets now have a couple different effects from kicking them, including a few YAFM.
* Kicking now only breaks the toilet 1/7 chance (was 1/4 in SLASH'EM)
* Kicking can generate giant cockroaches and pools from kicking (1 in 17 chance)
* Kicking can generate brown puddings (only once per toilet)
* Kicking can generate a random tool. Normally this tool will weigh under 15aum, but sometimes you'll get a large tool that bonks against the piping. If a large tool bonks 3x - you'll get that tool no matter now big it is and the toilet is destroyed in the process.

Dipping an edged weapon into a toilet can poison it, but also probably rust any metallic items.

### Bloody tiles
* Ported from SpliceHack
* When a monster is killed, it can spray blood around the surrounding tiles depending on it's size.
* The blood is mostly cosmetic, however, players cannot engrave in the dust whilst blood covers that tile.
* Blood can be wiped off with a towel, or will wear off after enough activity.
* Fire and acid rays also burn off blood from tiles.
* Bloody doors are more difficult to open and close.

### Traps
* Polytraps always disappear whenever a monster steps on one.
* Invisibility from magic traps lasts a long time (2500-5000 turns), instead of permanently.
* Anti-magic fields block spellcasting for the player and monsters
* Anti-magic fields also block wand zapping
* Arrow traps and dart traps cannot be avoided by flight.

* **Partially reverted commit 5c7c9d10a from 3.7.0** - Rejigger anti-magic traps. I thought the severity of the
  original change was actually fine, anti-magic traps were historically a joke in NetHack
  3.4.3 so this makes them somewhat threatening.

#### New container traps
* A cream pie may spring out of the box and hit the player in the face.
* A small critter (rat, snake, or spider) maybe jump out of the container, briefly scaring the player.
* A loud alarm may sound, waking up nearby monsters.

#### Falling rock traps
* At higher levels, boulders can drop from falling rock traps.
* Falling rock traps can result in stunning
* Falling rock traps can drop multiple rocks (or boulders).
* You cannot fly over falling rock traps.
* You can now #untrap falling rock traps, obtaining rocks (Fourk).

#### Spear traps
* A new floor trap ported from EvilHack
* Spear traps only start appearing after level 5
* Spear traps can be untrapped, potentially yielding a random spear type in the process.
* Flying and levitation usually protect from being harmed by spear traps, however, there is still a 25% chance of being hit (by a abnormally long spear)
* If you or a monster hit by the trap is thick-skinned, the spear just breaks and the trap is deleted.
* The trap also doesn't affect unsolid monsters.
* When hit, it deals 7-14 damage and wounds your legs for 10-19 turns.
* Spear traps sometimes have poisoned spears.
* Spear traps abuse strength and constitution.

#### Magic beam traps
* A new trap ported from EvilHack
* Magic beam traps only start appearing after level 14
* When you (or a monster) steps on this trap, it shoots a random ray type from a pre-set location that crosses through the beam trap. The beam type is set for each trap, so once you notice it shoots fire rays, it will always shoot fire rays.
* Magic beam traps can very rarely shoot disintegration rays.

#### Grease traps
* A new creation debuting in NerfHack
* Grease traps function similarly to rust traps, but they spray a blast of grease at the player or monster that stepped on it.
* When you step on a grease trap, you either slip in a puddle of grease or get sprayed by a grease hose.
* When stepped on, the trap disarms with a random 1 in 15 chance.
* You can also #untrap grease traps, if successful you may yield a rubber hose or - in rare cases - a can of grease.

**Puddle of grease:**
  * If you don't have levitation or flying, you gain fumbling ("You step in a puddle of grease.")
  * If you have flying - you are covered in grease, lose flying, and are blinded by goop.
  * Slipping in grease traps can cause you or monsters to become paralyzed for a few turns and inflicts a small amount of damage.
  * Mud boots and water walking boots protect from slipping on grease traps.

**Grease hose:**
  * If the grease hits your head, you are blinded unless you are wearing a visored helmet. Your blindfold/lenses/etc may also become greased and fall off.
  * If the grease hits your arm, your weapon(s) or shield can become greased and fall off. You also gain the Glib condition for 10 to 15 turns.
  * If the grease hits your feet, your boots can become greased and fall off.
  * Otherwise, the grease hits your torso and your outermost armor becomes greased. Random items you are carrying can also become greased and fall from your possession. If you are carrying a towel, there is a 50% chance it becomes greased as well. If you are riding a steed the saddle will get hit with grease, making you fall off.
* When a monster gets hit with grease, it will randomly grease an item in their inventory.

Note: Getting hit by grease will not knock off worn cursed items.

#### Cold Traps
* Ported from xNetHack, originally from UnNetHack
* Cold traps are nasty and deal 4d8 cold damage, potentially shattering potions.
* If you have less than 25% cold resistance, you can have your HP drained similar to fire traps
* If you are 25% or more cold resistant, you may have a significant portion of your resistance (25-50%) sucked away by the trap.

#### Door traps
* Door traps actually explode in a ball of flame (EvilHack)
* These traps will start appearing at level 8.

#### Booby-trapped tins
* From xNetHack
* Randomly generated tins have a 1 in 30 chance of exploding in a blast of fire when opened.
* Tins that you create from tinning kits will always be safe.


## SPECIAL ROOMS


### Art rooms
* Ported from SpliceHack
* These rooms have a one-time event that occurs upon entering a room
* Most of the time it's a fun piece of art depicting something with the denizens of the dungeon. But sometimes it's a special effect.
  * You might see an image of your god, invoking enlightenment
  * You might find a partial map of the level
  * You might encounter a scary image, stunning you for a few turns
  * You might discover a new item
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
* Always ruled by a titan

### New room: Real zoo (from SLASH'EM).
* Monsters in real zoos are always hostile.

### New room: Fungus farm (from SLASH'EM).
* Features a collection of slimy and oozy monsters.

### New room: Migo hive (from SLASH'EM).

### New room: terror halls (from SlashTHEM)
* Features a random assortment of U (hulk class) monsters


## ALTARS, PRAYER, AND PRIESTS


* When donating to priests - the gold vanishes upon receipt
* There is a greater chance of hostile minions appearing when converting an altar. Especially if the altar is in an occupied temple (EvilHack)
* Converting altars has higher chance of summoning minions (SLASH'EM)
* Intrinsics speed, stealth, and telepathy are no longer granted by the gods when #offering.
* Getting troubles fixed by prayer abuses constitution.
* Permanent alignment conversion prevents more divine protection from being granted

Note regarding recent #offer gift changes in NetHack 3.7.0. These recent changes make the value the corpse offered matter in what artifacts are granted. In NerfHack, the framework of these changes was retained, however, the values of all artifacts have been lowered to 1 (the minimum), so as to preserve the original behavior of #offer gifts. Because there have already been strong changes to altars (cracking and XP dependent chances of gifts), the additional effect of monster value might be too much. The value of a monster still affects the chances of receiving altar luck though.

### Revised divine protection scheme
* The more protection the player has, the less likely it is to be granted (K-Mod)
* The maximum possible divine protection is capped at -9AC.
* When protection is granted from priests or your god, it is limited to increments of 1AC per granting.


| Current protection | Chance of fail |
| ------------------ | -------------- |
| 0                  | 0%             |
| 1                  | 1%             |
| 2                  | 4%             |
| 3                  | 9%             |
| 4                  | 16%            |
| 5                  | 25%            |
| 6                  | 36%            |
| 7                  | 49%            |
| 8                  | 64%            |
| 9                  | 81%            |
| 10                 | 100%           |


### Altar cracking
**Once the player has received *any* gifts or has been crowned, altars will crack with each subsequent gift.**

* There are two stages to the cracking. In the first stage the altar becomes partially cracked, which is purely cosmetic and doesn't affect the altar's functionality. This cracked status can be seen on an altar by farlooking. However, receiving another gift from a cracked altar will certainly destroy it, losing it forever.
* Being crowned also counts as a gift. If you are crowned on a cracked altar, it will also almost always destroy it in the process (however - there is a 1 in 13 chance that the altar will survive the process).
* Altars on the Astral Plane will never be destroyed. Note that they can still become cracked but are safe from destruction.
* Many of the guaranteed altars in quests now have a good chance to already be cracked. This is especially true if they are unattended or unaligned, implying there was recent conflict and the altar was damaged.
* Converting an altar will also frequently crack it. This occurs 1 in 13 times the altar is converted or 1/3rd of the time hostile minions are summoned.
* Non-chaotic same-race sacrifice always cracks altars.

The original altar nerf came from SpliceHack, where altars had a 50% chance of being destroyed after two artifact gifts had been bestowed.

A new conduct was added to the #conduct menu so that players can track how many altars have been destroyed in their current game. Altar cracking is livelogged on game servers for the entertainment value.

### Altar generation
* **An uncracked altar is guaranteed to spawn at the Oracle's level.**
* Altars don't start spawning until level 15 (other than the Oracle altar)
* Randomly generated altars are always cracked after level 15.
* Temples cannot appear until level 15. Unlike random altars, temple altars will not be cracked, as they are maintained by a priest.


### #offer GIFT ODDS
**Altar gift frequency is tempered by your experience level (EvilHack).**

As your level increases, the probability of receiving an artifact increases. Under level 4 is not possible:
* level  4: 20% chance
* level  6: 30% chance
* level  8: 40% chance
* level 11: 50% chance
* level 13: 60% chance
* level 15: 70% chance
* level 17: 80% chance
* level 18: 90% chance
* level 20 or greater: 100% chance

This rewards leveling up and slows down the power grab that some characters might go for with a guaranteed sacrifice gift (ie: Barbarians). It also slows down the rate at which altars are cracking and getting destroyed, giving more time to utilize them for other things like building Luck or getting crowned.

* The raw odds of receiving an artifact have been adjusted in favor of the player, especially after 2 gifts have been granted.

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

* The number of artiwishes is not factored in when determining the chance of a gift. The revised gift probabilities still apply, just filtered through the level check.
* #offer odds also improve with a perfect alignment abuse record (from EvilHack)

### Crowning
* Crowning requires 13 Luck (dNetHack).
* Crowning only provides a 50% increase in resistances.
* Intrinsic see invisible is no longer granted via crowning
* Intrinsic telepathy is no longer granted via crowning
* Crowning gifts are only granted when crowned, not for offering gifts.
* Your god will not crown you until you have completed the quest.
* Crowning makes it impossible to change alignment ever again.


## THE QUEST

* Removed the quest turn limit (UnNetHack)
* Players can enter the quest as soon as they reach level XL 10 (UnNetHack)
* Prevent the player from skipping most of the quest (xNetHack).
* Mark all quest levels as hardfloor.
* Players cannot do horizontal or downward teleporting whilst the quest nemesis is alive.


## MISC CHANGES


* These don't really fit into any category, or are just silly.
* 8d93bedd9 Halu reverse genocide troll msg (UnNetHack).
* 899833966 Funny troll #chat messages (SpliceHack).
* Characters who don't like baths may resist fountain's urging (xNetHack).
* New hallucinatory monsters from Secret of Mana and Magic of Scheherazade.
* The fat lady sings if you win whilst hallucinating (xNetHack).

## CREDITS


NerfHack draws inspiration and ideas from many variants of NetHack:
* AceHack
* Dynahack
* EvilHack
* FIQHack
* Fourk
* GnollHack
* GruntHack
* K-Mod
* NetHack Fourk
* SLASH'EM
* SlashTHEM
* SLASH'EM-up
* SLASH'EM9
* SpliceHack
* Sporkhack
* UnNetHack
* xNetHack


### NetHack Ideas Archive credits

| YANI  | commit    | author               | notes                                                                   |
| ----- | --------- | -------------------- | ----------------------------------------------------------------------- |
| #8    | 763e4ed25 | bezaban              | You can fall onto your own weapon whilst fumbling.                      |
| #10   | e049887c8 | aosdict              | Wizards are able to sense magic fountains.                              |
| #125  | e03ac9fb5 | Andrio               | Spiked orcs, which are more deadly than regular orcs.                   |
| #149  | 402066eab | AmyBSOD              | Falling down stairs while stunned or confused.                          |
| #254  | 6d15685cf | NeroOneTrueKing      | Unicorn horns only reduce the timeouts of statuses.                     |
| #441  | 1036e6cf7 | aosdict/FIQ          | Strength doesn't affect to-hit calculations.                            |
| #743  | 13c4eb7c8 | jonadab              | Cancelled unicorn horns become degraded, unusable for curing.           |
| #876  | d0ebfe767 | K2                   | Healers can use uncursed unihorns as blessed.                           |
| #1022 | 05b991a0e | RGRN                 | Serenity blocks aggravate monster.                                      |
| #1058 | 9c09d7d57 | RGRN                 | Abuse WIS when over-enchanting items.                                   |
| #1278 | 571f8a98c | Chris_ANG            | King Arthur gets a full suite of resistances                            |
| #1647 | ddf5fc1dc | aosdict              | Ring of aggravate monster causes pets to fearlessly attack anything.    |
| #1727 | 22cbacacd | aosdict              | Mumakil get butts or kicks instead of bites.                            |
| #1824 | a9ce809b7 | aosdict              | Gas spores and volatile mushrooms start with exactly 1 HP.              |
| #1903 | 04913bdc5 | aosdict              | Protection from shape changers wakes up shifters when they normalize.   |
| #1923 | ed6cd6a42 | aosdict              | Recolor royal jelly to magenta                                          |
| #1942 | 75ebf9a84 | aosdict              | Boulders deal 1+5d4.                                                    |
| #1944 | 170c60410 | aosdict              | Confused cursed scroll of punishment decreases god anger by 1.          |
| #1948 | 1c8377153 | aosdict              | Spellbooks can generate pre-read.                                       |
| #1952 | e2b9d3c91 | aosdict              | Dipping scrolls of amnesia clears non-water non-polymorph potions.      |
| #1976 | ea543e77b | aosdict              | Mixing oil with water always results in diluted oil.                    |
| #1992 | 163af6658 | aosdict              | Potions of restore ability also cures wounded legs.                     |
| #2023 | 2b553fee6 | aosdict              | Nerf slow digestion.                                                    |
| #2062 | 460d74c91 | aosdict              | Casting clairvoyance at skilled lets it persist for a while.            |
| #2082 | 04f87f673 | aosdict              | Aggravate monster spell cast at hero causes temporary aggro mon.        |
| #2084 | 7800ffd44 | aosdict              | You cannot learn spells that you are restricted in [now revamped]       |
| #2090 | 8b6a11458 | aosdict              | knock and wizard lock spell nerfs                                       |
| #2199 | 896ed1feb | aosdict              | Crowning makes it impossible to change alignment ever again.            |
| #2200 | 4be06d9a9 | aosdict              | Permanent alignment conversion prevents more divine protection          |
| #2217 | b909ed83b | aosdict              | Your god will not crown you until you have completed the quest.         |
| #2246 | 912e4d7f5 | aosdict              | Anti-magic fields block spellcasting.                                   |
| #2281 | 8a2cc0e9f | aosdict              | The ranger quests gets a bunch of bear traps.                           |
| #2435 | f05429d20 | aosdict              | Being satiated abuses wisdom for Samurai.                               |
| #2472 | b9b973120 | aosdict              | You must have at least one free hand to zap a wand.                     |
| #2551 | 09f52ef60 | aosdict              | Eating domestic animals causes aggro mon for 5000-7500 turns            |
| #2589 | 10279d5a7 | aosdict              | Rogues start with a stack of knives instead of daggers.                 |
| #2640 | 8be066328 | aosdict/Tone         | New monster: third eye.                                                 |
| #2749 | 9252efc92 | aosdict              | Unique monsters can drop cards for cartomancers.                        |
| #2829 | 5acc2b12c | aosdict              | No multishot when fumbling.                                             |
| #2903 | 5a11551b7 | aosdict              | spell of knock nerf                                                     |
| #2950 | a6abab270 | aosdict              | Shopkeepers offer 1/2 price for diluted potions.                        |
| #2966 | 53c6df5fb | dingotron            | Archeologists can reach basic in axe.                                   |
| #2985 | e1d625473 | aosdict              | Unicorn horns dissolve when dipped into acid, yields healing.           |
| #3019 | 9250f9b84 | aosdict              | Cursed rings burn extra nutrition when worn.                            |
| #3044 | bea6abeb1 | aosdict/bouquet      | Potions of restore ability can be alchemized.                           |
| #3061 | 5d22ac85e | rikersan/aosdict     | Glib hands makes applying any item except towels drop them.             |
| #3085 | 902bdf934 | riker                | Free action protects from stoning paralysis.                            |
| #3092 | dd90a3c27 | aosdict              | Giant mimics get an engulf digest attack.                               |
| #3110 | ca583e428 | mobileuser           | Archeologists start out knowing dwarvish mattocks.                      |
| #3204 | 05bf49bad | aosdict              | You can kick with kicking boots even when your legs are wounded.        |
| #3368 | 150193c7a | spicycat             | Aggravate monster causes monsters not be scared of musical instruments. |
| #3375 | e8baf4d73 | many                 | A tree hit by a fire ray or explosion should instantly incinerate       |
| #3390 | cb6f97237 | aosdict              | Samurai get a bonus for twoweaponing katana with wakizashi.             |
| #3578 | fd709a04a | K2                   | Cursed armor weighs more when worn.                                     |
| #3588 | d3b3f5176 | Umbire               | Limit range of attacks to 1 square when in a pit.                       |
| #3658 | 20b345d6f | NetSysFire           | Falling rock traps can stun you.                                        |
| #3826 | b0fc3027b | spicycat/aosdict     | Towels can be used to remove grease from specific objects.              |
| #3866 | 92bca4df9 | spicycat             | Cartomancers cast spells by reading books                               |
| #3878 | 4d02dafd6 | krm26                | New item: ring of withering.                                            |
| #3931 | d70406a9a | aosdict              | Greased rings slip off your fingers                                     |
| #3977 | 5b685c2f4 | aosdict/ais523       | Falling rock traps can dump multiple rocks                              |
| #3991 | 267661174 | ais523/FIQ/Chris_ANG | Spell of charm monster nerfs/updates.                                   |
| #4083 | 7ce16cf2f | aosdict              | Grease traps.                                                           |
| #4259 | bc383ebde | aosdict/Shadow_Rider | Rogues can counterattack with knives and daggers.                       |
| #4259 | 2abbcfca6 | aosdict/Shadow_Rider | Morning stars and flails can stun monsters on critical hits.            |
| #4259 | 2abbcfca6 | aosdict/Shadow_Rider | Spears at expert skill can skewer through enemies.                      |
| #4267 | e8baf4d73 | AntiGulp             | Hitting a tree with sufficient cold damage makes it explode.            |
| #4350 | 445bbdf97 | amateurhour/aosdict  | Let rangers chop down the trees in the quest entry level.               |
| #4364 | 842f6bd1d | aosdict              | New artifact: The Lenses of Truth.                                      |
| #4411 | f9e5ea0f3 | Loggers_VIII         | Greased items sometimes slip when disarmed with a bullwhip.             |

Many thanks to all the folks who have helped out with the original Hack'EM and NerfHack, contributing ideas, making patches, playtesting, or anything!


### Changes that were later adopted into NetHack 3.7.0
* Archeologists get a luck bonus for wearing a fedora (UnNetHack).
* Improved item destruction (xNetHack). This patch fixes some problems with item destruction, making it less random and more dependent on the damage dealt in the interaction. Overall, players should expect to get a more fair deal with fewer items destroyed.

### Special thanks to:
- My wife - for being endlessly patient with this time-consuming endeavor!
- K2, for making the epic EvilHack, all his help during development, and pushing HackEM up to hardfought.
- amateurhour and qt for their endless debugging advice.
- cbus for many contributions
- mobileuser and hothraxxa for extensively playtesting the original HackEM
- malor for continuing maintenance of HackEM
- Arseniy for being the first player to succumb to an unwinnable-game bug in the quest.
- anyone who has playtested or reported bugs!

### Thanks:
- amateurhour
- antigulp
- aosdict
- arahael
- Ardub23
- Arseniy/DoktorL
- bhaak
- bouquet
- cbus
- Chris_ANG
- Demo
- disperse
- Frozty
- Hash56
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
- tinklebear
- transcendreamer
- Umbire
- VaderFLAG
- YesLaching
