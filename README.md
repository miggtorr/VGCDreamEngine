# Rotom Draft

![](https://raw.githubusercontent.com/miggtorr/RotomDraft/refs/heads/main/icon.iconset/icon_256x256.png)

### The All-In-One VGC Draft League Software Suite for macOS.

**Rotom Draft** is a feature-rich suite of software tools to help **VGC Draft League** players bring their best game to their matches. 
Powerful integrations with [Pokemon Showdown](https://play.pokemonshowdown.com), the [PokeAPI](https://pokeapi.co/), and **PokePast.es** let you quickly design the optimal strategy for your next match!

## Requirements

macOS 14 Sonoma or higher.

NOTE: There are currently no plans to port the software to Windows/Linux.

## Features

**Rotom Draft** features three main workspaces: the **Analysis Panes**, the **Tool Drawers**, and the **Damage Calculator**. 

The **Tool Drawers** features **powerful applets** that let you: 
- Build your best Roster
- Calculate optimal tera-types
- Keep track of the league's schedule and standings
- keep notes, records, and replay URLs (Showdown, YouTube, Twitch, etc.) for each match
- Build Teams based on the Pokémon on your Roster

The **Analysis Panes** are where you go to deep dive into a Roster's strengths and weaknesses, including:
- Moves
- Stats
- Type Matchups
- Battle Strategies
- Ability Interactions
- Weather/Terrain Synergies
- Speed Control Methods
- and More!

You can also keep track of your League's **Draft Board** here, filtering Pokémon by draft point value and availablity status to plan trades and free agency swaps!

Finally, the **Battle Calculator** lets you quickly make critical calcs between Pokemon on different teams and rosters, saving tweaks, as needed. It's a fully-embedded version of the [Pokémon Showdown calculator](https://github.com/smogon/damage-calc), so all the results and interactions are identical to what you would calculate [online](https://calc.pokemonshowdown.com/). 

## Organizing Principles

The basic organizing principle behind Rotom Draft is that groups of Pokémon are organized hierarchically like so: 

**League => Roster => Team**

### League

A League is the event in which the player is participating. Essentially, a tournament. 

Leagues have Rulesets associated with them that specify what's available on the Draft Board, how many draft points each player receives, and how many pokemon can be selected.

In Rotom Draft, a League also features its own schedule, leaderboard, and playoff bracket. 

If you are participating in several Draft Leagues at the same time, **Rotom Draft** helps you keep those different Leagues sequestered—along with their associated Pokemon, Players, Standings, etc.—so you're never confused as to which League your looking at!

### Roster

A Roster is a player's selection of drafted Pokémon, usually 10 in standard VGC formats. In Rotom Draft, Rosters can be associated with a particular League. Multiple rosters typically associate with a single League. 

All of Rotom Draft's analysis functions apply to entire Rosters so you can see the plethora of interactions and counter-interactions that you or an opponent can create using the Pokémon on a roster. 

For exmaple, tools like [Marrilan's Pokémon Team Builder](https://marriland.com/tools/team-builder/en/) help you see the defensive type profile of a group of up to six Pokémon—brilliant for ladder or tournament teams. But the Rotom Draft Type Matchup Analysis Pane lets you see the defensive type profile of all your entire roster, factoring in moves like Freeze Dry and abilities like Neutralizing Gas that turn off things like Levitate and Flash Fire. 

All Rosters can be imported via PokePast.es or exported to the clipboard in Showdown format, so you can easily move data to and from Showdown for backup, analysis, or playtesting.

### Teams

Teams are the party of six Pokémon a player brings to a match. 

Teams are typically composed of a subset of the Pokémon in a Roster. They can be customized and tweaked just like on Showdown, with Abilities, Movesets, Natures, Items, and the like. 

Teams can be created and edited inside of Rotom Draft's powerful Team Builder. They can also be imported or exported to/from Showdown for backup or playtesting. 

Teams are what you load into Rotom Draft's Battle Calculator, and can feature more than 6 Pokémon, e.g., if you need to calc your team against an opponent's entire roster. 

## Tool Drawers

### Rosters Drawer

The Rosters Drawer can be thought of as the Home Base of Rotom Draft: this is where it all begins.

#### Creating a League

When you open Rotom Draft for the first time, it's a good idea to create a League. To do so, click the "Manage Leagues..." button and add a "New" League. Give the League a name and select a Ruleset for the league. If you don't see an applicable ruleset, don't worry. You can add/edit a custom ruleset later. 

#### Creating a Roster

Next you'll want to create your first roster. There are multiple ways of going about this, but the best way to start is by typing a Roster Name at the top and clicking Save Roster. This will create an empty Roster with the given name.

You'll want to associate this Roster with your League, so click on it and then click the "Manage Leagues..." button again and assign it to the correct League.

#### Adding Pokémon to a Roster

To add Pokémon to this Roster, make sure it's selected. Then you can do one of the following:

- You can type in a Pokémon's name in the "Add Pokémon" box and click "Add."

IMPORTANT: Make sure to click **Save Roster** at the top again to Save your changes or they'll revert!

NOTE: This will need to be the PokeAPI name of the Pokemon. Some PokeAPI names are normal—e.g., "Sunflora"—but when you get into Pokémon with spaces and odd characters in their names, or pokemon with multiple forms, things can be unintuitive. For example, Water Tauros's PokeAPI name is "tauros-paldea-aqua-breed". What a mouthful! Luckily, there are alternative methods to adding Pokémon to a Roster so you don't need to worry about looking up the correct PokeAPI name for each Pokémon.

- You can Import via a Poképaste.

This may be the simplest thing to do for first-time users. Save a new Box on Showdown with the Pokémon you want (no need to add moves, EVs, etc) and export that to Pokepast.es. Then click "Import Pokepaste" and paste in the URL.

IMPORTANT: Make sure to click **Save Roster** at the top again to Save your changes or they'll revert!

- You can Add Pokémon via your League's Draft Board!

Rotom Draft makes it easy to draft Pokémon straight from the Draft Board corresponding to your League's Ruleset! The **Draft Board** section below details how to do this, but the basic idea is that you open the Draft Board pane and—with your Roster selected in the Rosters drawer—double click on a Pokémon's name to add/remove it from your Roster. You can search for a Pokémon's name so no need to worry about odd spellings and form names. 

Rosters save automatically when updated in this way.

#### Managing Rosters

The Rosters Drawer offers a handful of other convenient functions for managing Rosters:

- Roster Duplication: If you change the name of the Roster in the Roster Name box at the top and click Save, it will not Rename the Roster. Rather, it will create a duplicate Roster with the new name (to Rename a Roster, use the Rename button instead).

Filters
- At the top of the Drawer, under the Roster Name and Save button

- New: Generates a new, unsaved blank Roster. Does not save a new Roster. The same as deselecting all Rosters. 
- Rename: Rename the current Roster.
- Clear: Clears the current Roster. WARNING: This clears AND saves the current Roster. Only use this if you really want to rebuild a Roster from scratch.
- Delete: Deletes the current Roster. WARNING: This deletes the current Roster permanently.
- Favorite: If checked, keeps the current Roster at the top of the Rosters list.

- Remove Selected: When a Pokémon is selected in the Current Roster section, it removes that Pokémon from the roster. Does not save (click Save Roster to save).




