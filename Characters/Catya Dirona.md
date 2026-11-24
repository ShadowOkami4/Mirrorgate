---
statblock: true
atlas-template: "player-character-5e-cc5e01"
name: "Catya Dirona"
level: 5
type: "Tiefling Wizard 5 (Bladesinger)"
size: "Medium"
alignment: "Chaotic Good"
background: "Guide"
ac: 13
initiative: 3
hp: 32
hit_dice: "5d6"
speed: "30 ft."
proficiency_bonus: 3
stats: [8, 16, 15, 16, 10, 10]
saves:
  "strength": -1
  "dexterity": 3
  "constitution": 2
  "intelligence": 6
  "wisdom": 3
  "charisma": 0
skillsaves:
  "acrobatics": 6
  "animal handling": 0
  "arcana": 6
  "athletics": -1
  "deception": 0
  "history": 3
  "insight": 0
  "intimidation": 0
  "investigation": 6
  "medicine": 0
  "nature": 3
  "perception": 0
  "performance": 0
  "persuasion": 0
  "religion": 3
  "sleight of hand": 3
  "stealth": 9
  "survival": 3
senses: "Darkvision 60 ft., Passive Perception 10, Passive Investigation 16, Passive Insight 10"
languages: "Common, Draconic, Common Sign Language"
proficiencies: "Simple Weapons, Battleaxe, Flail, Longsword, Morningstar, Rapier, Scimitar, Shortsword, Trident, Warhammer, War Pick, Whip, Cartographers Tools"
damage_resistances: "Fire"
resources:
  - name: Level 1 slots
    max: 4
    used: 0
    reset: long-rest
  - name: Level 2 slots
    max: 3
    used: 0
    reset: long-rest
  - name: Level 3 slots
    max: 2
    used: 0
    reset: long-rest
  - name: Arcane Recovery
    max: 1
    used: 0
    reset: long-rest
  - name: Bladesong (Invoke)
    max: 3
    used: 0
    reset: long-rest
actions:
  - "name": "Seelenspiegel"
    "desc": "*Melee Weapon Attack:* +6 to hit, reach 5 ft. *Hit:* 1d6 + 3 piercing damage. (Finesse, Light, Vex)"
  - "name": "Dagger"
    "desc": "*Melee Weapon Attack:* +6 to hit, reach 5 ft. or range 20/60 ft. *Hit:* 1d4 + 3 piercing damage. (Finesse, Light, Thrown, Nick)"
  - "name": "Initiate a Circle Spell"
    "desc": "You take a Magic action to initiate casting a Circle spell. When you do so, choose which Circle casting option you’re using for this casting; you must also meet any of the other requirements described in that option’s text. Until the Circle spell’s casting is complete, you must maintain Concentration on the spell."
bonus_actions:
  - "name": "Bladesong (Invoke)"
    "desc": "You can invoke the Bladesong, provided you aren’t wearing armor or using a Shield. You can invoke the Bladesong {{limiteduse}} times per Long rest, and regain one expended use when you use Arcane Recovery."
spellcasting: "Wizard: Intelligence, spell save DC 14, +6 to hit with spell attacks."
spells:
  - "Cantrips (at will)": "Blade Ward, Evil Eye, Fire Bolt, Frigid Blade, Frostbite, Message, Thaumaturgy, Vengeful Blade"
  - "1st level (4 slots)": "Accelerate/Decelerate, Detect Magic, Goodberry, Hellish Rebuke, Mage Armor, Thunderwave"
  - "2nd level (3 slots)": "Arcane Vigor, Darkness, Dragon's Breath, Wind Sprint"
  - "3rd level (2 slots)": "Fireball, Mass Leech"
spellbook: "Witch Bolt, False Life, Shield, Ice Knife, Magic Missile, Disguise Self, Burning Hands, Shadow Blade, Vampiric Claws, Misty Step, Find Familiar, Feather Fall, Spellfire Flare, Tremor, Hell’s Lash, Initiative, Grease, Void Strike"
traits:
  - "name": "Bladesong"
    "desc": "As a Bonus Action, you invoke an elven magic called the Bladesong, provided you aren’t wearing armor or using a Shield.\n\nThe Bladesong lasts for 1 minute and ends early if you have the Incapacitated condition, if you don armor or a Shield, or if you use two hands to make an attack with a weapon. You can dismiss the Bladesong at any time (no action required).\n\nWhile the Bladesong is active, you gain the following benefits. You can invoke the Bladesong a number of times equal to your Intelligence modifier (minimum of once), and you regain all expended uses when you finish a Long Rest. You regain one expended use when you use Arcane Recovery.\n\n***Agility.*** You gain a bonus to your AC equal to your Intelligence modifier (minimum of +1), and your Speed increases by 10 feet. In addition, you have Advantage on Dexterity (Acrobatics) checks.\n\n***Bladework.*** Whenever you attack with a weapon with which you have proficiency, you can use your Intelligence modifier for the attack and damage rolls instead of using Strength or Dexterity.\n\n***Focus.*** When you make a Constitution saving throw to maintain Concentration, you can add your Intelligence modifier to the total.\n\n*Select Invoke the Bladesong below to apply the effects. Deselect it to dismiss the Bladesong.*"
  - "name": "Training In War and Song"
    "desc": "You gain proficiency with all Melee Martial weapons that don’t have the Two-Handed or Heavy property.\n\nYou can use a Melee weapon with which you have proficiency as a Spellcasting Focus for your Wizard spells.\n\nYou also gain proficiency in one of the following skills of your choice: Acrobatics, Athletics, Performance, or Persuasion."
  - "name": "Spellcasting"
    "desc": "As a student of arcane magic, you have learned to cast spells.\n\n***Cantrips.*** You know three Wizard cantrips of your choice. Whenever you finish a Long Rest, you can replace one of your cantrips from this feature with another Wizard cantrip of your choice.\n\nWhen you reach Wizard levels 4 and 10, you learn another Wizard cantrip of your choice, as shown in the Cantrips column of the Wizard Features table.\n\n***Spellbook.*** Your wizardly apprenticeship culminated in the creation of a unique book: your spellbook. It is a Tiny object that weighs 3 pounds, contains 100 pages, and can be read only by you or someone casting Identify. You determine the book’s appearance and materials, such as a gilt-edged tome or a collection of vellum bound with twine.\n\nThe book contains the level 1+ spells you know. It starts with six level 1 Wizard spells of your choice.\n\nWhenever you gain a Wizard level after 1, add two Wizard spells of your choice to your spellbook. Each of these spells must be of a level for which you have spell slots, as shown in the Wizard Features table. The spells are the culmination of arcane research you do regularly.\n\n***Spell Slots.*** The Wizard Features table shows how many spell slots you have to cast your level 1+ spells. You regain all expended slots when you finish a Long Rest.\n\n***Prepared Spells of Level 1+.*** You prepare the list of level 1+ spells that are available for you to cast with this feature. To do so, choose four spells from your spellbook. The chosen spells must be of a level for which you have spell slots.\n\nThe number of spells on your list increases as you gain Wizard levels, as shown in the Prepared Spells column of the Wizard Features table. Whenever that number increases, choose additional Wizard spells until the number of spells on your list matches the number in the table. The chosen spells must be of a level for which you have spell slots. For example, if you’re a level 3 Wizard, your list of prepared spells can include six spells of levels 1 and 2 in any combination, chosen from your spellbook.\n\nIf another Wizard feature gives you spells that you always have prepared, those spells don’t count against the number of spells you can prepare with this feature, but those spells otherwise count as Wizard spells for you.\n\n***Changing Your Prepared Spells.*** Whenever you finish a Long Rest, you can change your list of prepared spells, replacing any of the spells there with spells from your spellbook.\n\n***Spellcasting Ability.*** Intelligence is your spellcasting ability for your Wizard spells.\n\n***Spellcasting Focus.*** You can use an Arcane Focus or your spellbook as a Spellcasting Focus for your Wizard spells.\n\nExpanding and Replacing a Spellbook\n\nThe spells you add to your spellbook as you gain levels reflect your ongoing magical research, but you might find other spells during your adventures that you can add to the book. You could discover a Wizard spell on a Spell Scroll, for example, and then copy it into your spellbook.\n\n***Copying a Spell into the Book.*** When you find a level 1+ Wizard spell, you can copy it into your spellbook if it’s of a level you can prepare and if you have time to copy it. For each level of the spell, the transcription takes 2 hours and costs 50 GP. Afterward you can prepare the spell like the other spells in your spellbook.\n\n***Copying the Book.*** You can copy a spell from your spellbook into another book. This is like copying a new spell into your spellbook but faster, since you already know how to cast the spell. You need spend only 1 hour and 10 GP for each level of the copied spell.\n\nIf you lose your spellbook, you can use the same procedure to transcribe the Wizard spells that you have prepared into a new spellbook. Filling out the remainder of the new book requires you to find new spells to do so. For this reason, many wizards keep a backup spellbook."
  - "name": "Ritual Adept"
    "desc": "You can cast any spell as a Ritual if that spell has the Ritual tag and the spell is in your spellbook. You needn’t have the spell prepared, but you must read from the book to cast a spell in this way."
  - "name": "Arcane Recovery"
    "desc": "You can regain some of your magical energy by studying your spellbook. When you finish a Short Rest, you can choose expended spell slots to recover. The spell slots can have a combined level equal to no more than half your Wizard level (round up), and none of the slots can be level 6 or higher. For example, if you’re a level 4 Wizard, you can recover up to two levels’ worth of spell slots, regaining either one level 2 spell slot or two level 1 spell slots.\n\nOnce you use this feature, you can’t do so again until you finish a Long Rest."
  - "name": "Scholar"
    "desc": "While studying magic, you also specialized in another field of study. Choose one of the following skills in which you have proficiency: Arcana, History, Investigation, Medicine, Nature, or Religion. You have Expertise in the chosen skill."
  - "name": "Memorize Spell"
    "desc": "Whenever you finish a Short Rest, you can study your spellbook and replace one of the level 1+ Wizard spells you have prepared for your Spellcasting feature with another level 1+ spell from the book."
  - "name": "Darkvision"
    "desc": "You have Darkvision with a range of 60 feet."
  - "name": "Otherworldly Presence"
    "desc": "You know the Thaumaturgy cantrip. When you cast it with this trait, the spell uses the same spellcasting ability you use for your Fiendish Legacy Trait."
  - "name": "Fiendish Legacy"
    "desc": "You are the recipient of a legacy that grants you supernatural abilities. Choose a legacy from the Fiendish Legacies table. You gain the level 1 benefit of the chosen legacy.\n\nWhen you reach character levels 3 and 5, you learn a higher-level spell, as shown on the table. You always have that spell prepared. You can cast it once without a spell slot, and you regain the ability to cast it in that way when you finish a Long Rest. You can also cast the spell using any spell slots you have of the appropriate level. Intelligence, Wisdom, or Charisma is your spellcasting ability for the spells you cast with this trait (choose the ability when you select the legacy).\n\n*Legacy · Level 1 · Level 3 · Level 5*\n**Abyssal:** You have Resistance to Poison damage. You also know the Poison Spray cantrip. · Ray of Sickness · Hold Person\n**Chthonic:** You have Resistance to Necrotic damage. You also know the Chill Touch cantrip. · False Life · Ray of Enfeeblement\n**Infernal:** You have Resistance to Fire damage. You also know the Fire Bolt cantrip. · Hellish Rebuke · Darkness"
  - "name": "Fiendish Legacy Spells"
    "desc": "When you choose your Fiendish Legacy, and at character levels 3 and 5, you learn a spell as shown on the table. You always have that spell prepared. You can cast it once without a spell slot, and you regain the ability to cast it in that way when you finish a Long Rest. You can also cast the spell using any spell slots you have of the appropriate level. Intelligence, Wisdom, or Charisma is your spellcasting ability for the spells you cast with this trait (choose the ability when you select the legacy)."
  - "name": "Guide Ability Score Improvements"
    "desc": "The Guide Background allows you to choose between Dexterity, Constitution, and Wisdom. Increase one of these scores by 2 and another one by 1, or increase all three by 1. None of these increases can raise a score above 20."
  - "name": "Magic Initiate (Druid)"
    "desc": "*Origin Feat*\n\nYou gain the following benefits.\n\n***Two Cantrips.*** You learn two cantrips of your choice from the Druid spell list. Intelligence, Wisdom, or Charisma is your spellcasting ability for this feat’s spells (choose when you select this feat).\n\n***Level 1 Spell.** *Choose a level 1 spell from the same list you selected for this feat’s cantrips. You always have that spell prepared. You can cast it once without a spell slot, and you regain the ability to cast it in that way when you finish a Long Rest. You can also cast the spell using any spell slots you have.\n\n***Spell Change.*** Whenever you gain a new level, you can replace one of the spells you chose for this feat with a different spell of the same level from the chosen spell list.\n\n***Repeatable.*** You can take this feat more than once, but you must choose a different spell list each time."
  - "name": "Spell Sniper"
    "desc": "*General Feat (Prerequisite: Level 4+, Spellcasting or Pact Magic Feature)*\n\nYou gain the following benefits.\n\n***Ability Score Increase.*** Increase your Intelligence, Wisdom, or Charisma score by 1, to a maximum of 20.\n\n*** Bypass Cover.*** Your attack rolls for spells ignore Half Cover and Three-Quarters Cover.\n\n*** Casting in Melee.*** Being within 5 feet of an enemy doesn’t impose Disadvantage on your attack rolls with spells.\n\n*** Increased Range.*** When you cast a spell that has a range of at least 10 feet and requires you to make an attack roll, you can increase the spell’s range by 60 feet."
  - "name": "Dark Bargain"
    "desc": "At your GM's discretion, you can take a Dark Bargain."
  - "name": "Circle Magic (Intelligence)"
    "desc": "**Initiating a Circle Spell**\n\nYou take a Magic action to initiate casting a Circle spell. When you do so, choose which Circle casting option you’re using for this casting; you must also meet any of the other requirements described in that option’s text. Until the Circle spell’s casting is complete, you must maintain Concentration on the spell.\n\nIf a Reaction would trigger when a creature casts a spell—such as the Reaction taken to cast Counterspell— it also triggers when you take this action to initiate a Circle spell.\n\n**Circle Casting Options**\n\nThe following options provide ways to enhance a spell when casting it as a Circle spell. You can use only one Circle casting option on a spell at a time.\n\nSome spells have a “Casting as a Circle Spell” section in their description. Instead of using one of the following options, you can create the effect described in that section when casting the spell as a Circle spell. Such effects are often uniquely powerful and specific to their respective spells.\n\n**Augment**\n\nWhen you cast a spell with a range of at least 5 feet, you can increase the range of the spell by 1,000 feet per secondary caster contributing to the spell, up to a maximum of a 1-mile increase.\n\n**Distribute**\n\nWhen you cast a spell that requires Concentration, you can distribute the mental load of the spell among you and the secondary casters. Once the casting is complete, you and all secondary casters can maintain Concentration on this spell. As long as at least one caster who contributed to the spell maintains this Concentration, the spell’s effects remain active.\n\n**Expand**\n\nWhen you cast a spell that creates an area of effect, you can increase one dimension of the spell’s area of effect for this casting by 10 feet per secondary caster contributing to the spell. For example, if a spell creates a 20-foot-radius Sphere, casting it as a Circle spell with two secondary casters would increase the radius to 40 feet. A spell that creates a Line that is 5 feet wide and 300 feet long, cast as a Circle spell with two secondary casters, could make a Line that is either 25 feet wide or 320 feet long.\n\nEach secondary caster contributing to the spell must expend a spell slot (no action required). If the spell fails, these spell slots aren’t expended.\n\n**Prolong**\n\nWhen you cast a spell that has a duration of 1 minute or longer, you can increase the duration of the spell depending on the number of secondary casters contributing to the spell, as detailed in the table below.\n\nEach secondary caster contributing to the spell must expend a spell slot (no action required). If the spell fails, these spell slots aren’t expended.\n\n*Secondary Casters · The Spell Increases Duration by*\n**1–3:** 1 hour\n**4–6:** 8 hours\n**7+:** 24 hours\n\n**Safeguard**\n\nWhen you cast a spell that creates an area of effect, you can carve out a safe zone within that area of effect that is unaffected by the spell for its duration. This safe zone consists of a number of 5-foot Cubes equal to your spellcasting ability modifier plus the number of secondary casters contributing to the spell (minimum of one Cube). You can arrange the Cubes as you like, but each Cube must be contiguous with at least one other Cube.\n\nIf the spell’s area of effect can be moved, the safe zone moves with it.\n\n**Supplant**\n\nWhen you cast a spell that requires at least one Material component with a specified cost that is consumed by the spell, you can reduce the minimum cost of one such Material component by 50 GP per each secondary caster contributing to the spell. For example, casting Revivify as a Circle spell with two secondary casters would reduce the Material component’s minimum cost to 200 GP.\n\nEach secondary caster contributing to the spell must expend a spell slot of a level greater than or equal to the spell’s level (no action required). If the spell fails, these spell slots aren’t expended."
  - "name": "Circle Spell: Augment"
    "desc": "When you cast a spell with a range of at least 5 ft., you can increase the range of the spell by 1,000 ft. per secondary caster contributing to the spell, up to a max of a 1-mile increase."
  - "name": "Circle Spell: Distribute"
    "desc": "When you cast a spell that requires Concentration, you can distribute the mental load of the spell among you and the secondary casters. Once the casting is complete, you and all secondary casters can maintain Concentration on this spell. As long as at least one caster who contributed to the spell maintains this Concentration, the spell’s effects remain active."
  - "name": "Circle Spell: Expand"
    "desc": "When you cast a spell that creates an area of effect, you can increase one dimension of the spell’s area of effect for this casting by 10 ft. per secondary caster contributing to the spell.\n\nEach secondary caster contributing to the spell must expend a spell slot (no action required). If the spell fails, these spell slots aren’t expended."
  - "name": "Circle Spell: Prolong"
    "desc": "When you cast a spell that has a duration of 1 min or longer, you can increase the duration of the spell depending on the number of secondary casters contributing to the spell.\n\nEach secondary caster contributing to the spell must expend a spell slot (no action required). If the spell fails, these spell slots aren’t expended."
  - "name": "Circle Spell: Safeguard"
    "desc": "When you cast a spell that creates an area of effect, you can carve out a safe zone within that area of effect that is unaffected by the spell for its duration. This safe zone consists of a number of 5-ft. Cubes equal to **{{modifier:cha#unsigned}} + the number of secondary casters** contributing to the spell (min of 1 Cube). You can arrange the Cubes as you like, but each Cube must be contiguous with at least one other Cube.\n\nIf the spell’s area of effect can be moved, the safe zone moves with it."
  - "name": "Circle Spell: Supplant"
    "desc": "When you cast a spell that requires at least one Material component with a specified cost that is consumed by the spell, you can reduce the min cost of one such Material component by 50 GP per each secondary caster contributing to the spell.\n\nEach secondary caster contributing to the spell must expend a spell slot of a level greater than or equal to the spell’s level (no action required). If the spell fails, these spell slots aren’t expended."
inventory:
  - ["Spell Scroll (Level 2)", 1, null, ""]
  - ["Kuschelbestie - Drache", 1, null, "Yes"]
  - ["Seelenspiegel", 1, 2, "Attuned"]
  - ["Dagger", 1, 1, "Yes"]
  - ["Spellbook", 1, 3, ""]
  - ["Paper", 1, null, ""]
  - ["Backpack", 1, 5, "Yes"]
  - ["Spell Scroll (2nd Level)", 1, null, ""]
  - ["Spell Scroll (Level 1)", 1, null, ""]
  - ["Shortsword", 1, 2, ""]
  - ["Oil", 6, 6, ""]
  - ["Parchment", 8, null, ""]
  - ["Robe", 1, 4, ""]
  - ["Tinderbox", 1, 1, ""]
  - ["Book", 1, 5, ""]
  - ["Lamp", 1, 1, ""]
  - ["Ink Pen", 1, null, ""]
  - ["Ink", 1, null, ""]
currency:
  "gp": 34
  "ep": 1
  "sp": 33
  "cp": 107
personality:
  - "name": "Traits"
    "desc": "Gutmütige,übermütig,flink,Eifrig"
  - "name": "Ideals"
    "desc": "Beschützt die sie nicht selbstbeschützen können, Wissen sollte allen helfen,Natur soll geschützt werden und nicht ohne grund zerstört werden"
  - "name": "Bonds"
    "desc": "Zum Wissen und der Natur, und sich selbst beweisen das etwas ändern kann"
  - "name": "Flaws"
    "desc": "irrational Entscheidungen bei stressigen Situationen und starken Vertrauens Probleme"
appearance: "Gender: Female · Age: 19 · Height: 7 ft | 2,13 m · Weight: 250 lb · Eyes: Red Eyes · Hair: Long Dark · Skin: Red · Faith: Nature Spirits"
notes:
  - "name": "Personal Possessions"
    "desc": "A necklace with a rose quartz stone on it"
image: "Characters/art/Catya Dirona.jpeg"
---
<!-- charcam:start – written by Character Cam, changes here are replaced on the next export -->
*Catya Dirona – imported from [D&D Beyond](https://www.dndbeyond.com/characters/161742278) by Character Cam.*
<!-- charcam:end -->


