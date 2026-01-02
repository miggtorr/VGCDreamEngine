# Rotom Draft

![](https://raw.githubusercontent.com/miggtorr/RotomDraft/refs/heads/main/icon.iconset/icon_256x256.png)

### The All-In-One VGC Draft League Software Suite for macOS.

**Rotom Draft** is a feature-rich suite of software tools to help **VGC Draft League** players bring their best game to their matches. 
Powerful integrations with [Pokemon Showdown](https://play.pokemonshowdown.com), the [PokeAPI](https://pokeapi.co/), and **PokePast.es** let you quickly design the optimal strategy for your next match!

Though optimized for Draft League, Rotom Draft's powerful tools and integrations are adaptable to many forms of VGC prep, including ladder and tournament prep.

# Requirements

- macOS 14 Sonoma or higher.
- An intenet connection is required when adding a Pokémon to a Roster for the first time, as its data is downloaded and cached from the PokéAPI. If a Pokemon has already been cached, no connection is required.


NOTE: There are currently no plans to port the software to Windows/Linux.

# AI Disclosure

**Rotom Draft** was created with AI-assisted coding. The software was tweaked, debugged, and tested manually on macOS hardware by a real human (me).

**No** visual art was created using AI.

Icons and buttons were created by hand in Adobe Illustrator with no AI assistance.

All Pokémon Sprites and type icons were sourced from the [PokéAPI Sprite Repository](https://github.com/PokeAPI/sprites). 

# Features

**Rotom Draft** features three main workspaces: the **Tool Drawers**, the **Analysis Panes**, and the **Damage Calculator**. 

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

# Tool Drawers

## Rosters Drawer

The Rosters Drawer can be thought of as the Home Base of Rotom Draft: this is where it all begins.

### Creating a League

When you open Rotom Draft for the first time, it's a good idea to create a League. To do so, click the "Manage Leagues..." button and add a "New" League. Give the League a name and select a Ruleset for the league. If you don't see an applicable ruleset, don't worry. You can add/edit a custom ruleset later. 

### Creating a Roster

Next you'll want to create your first roster. There are multiple ways of going about this, but the best way to start is by typing a Roster Name at the top and clicking Save Roster. This will create an empty Roster with the given name.

You'll want to associate this Roster with your League, so click on it and then click the "Manage Leagues..." button again and assign it to the correct League.

### Adding Pokémon to a Roster

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

### Managing Rosters

The Rosters Drawer offers a handful of other convenient functions for managing Rosters:

#### Roster Duplication 
If you change the name of the Roster in the Roster Name box at the top and click Save, it will not Rename the Roster. Rather, it will create a duplicate Roster with the new name (to Rename a Roster, use the Rename button instead).

#### Filtering
- Filter Rosters by Name or by the name of any Pokémon on a Roster!
- Filter Rosters by League

#### Create/Rename/Delete
- New: Generates a new, unsaved blank Roster. Does not save a new Roster. The same as deselecting all Rosters. 
- Rename: Rename the current Roster.
- Clear: Clears the current Roster. WARNING: This clears AND saves the current Roster. Only use this if you really want to rebuild a Roster from scratch.
- Delete: Deletes the current Roster. WARNING: This deletes the current Roster permanently.
- Favorite: If checked, keeps the current Roster at the top of the Rosters list.

#### Remove Pokémon
- Remove Selected: When a Pokémon is selected in the Current Roster section, it removes that Pokémon from the roster. Does not save (click Save Roster to save).

#### Current Roster Section
- This Section lets you see all the Pokémon on a roster at a glance.

#### Type Matchup Pane Adjustments
- A Pokémon's default ability can be set here (affects Type Matchup pane)
- A custom (Tera) type can be set here (affects Type Matchup pane)

## Tera Type Calculator

The Tera Type Calculator lets you calculate a Pokémon's optimal Tera Type based on its typing and defensive abilities (e.g., Levitate, Thick Fat, etc.).

It uses an algorithm to determine a score for each tera type and rank them for the user, similar to [the calculator at terastal.net](https://terastal.net/tera-type-calculator.html/). 

NOTE: This algorithm is meta-agnostic. It's just a starting point. Always consider your league's meta when making final tera-type selections. 

To calculate a Pokémon's optimal tera type:
1) Make sure a Roster is selected in the Rosters Drawer.
2) Back in the Tera Type Calculator Drawer, select the Pokémon from the ribbon at the top
3) Note the summary of its defensive typing.
4) Consult the generated Tera Type Scores table.

Select **Additional Considerations** for a summary of special tera type features (e.g., Grass-types cannot be spored, Fire-types cannot be burned, etc.)

Select **Calculation Information** for a summary of the tera type calculation algorithm.

## Schedule Drawer

The Schedule Drawer is a multi-faceted tool for helping you keep track of:
- All the matches you play (including notes for prep and post-mortems)
- All the matches the other coaches play
- The current standings
- The playoff bracket

At the top you will see an option to **Select a League**. Schedules are League-specific. To use these features, you must select a League. 

### Sections

The Schedule Drawer contains three tabs:
- Swiss
- Leaderboard
- Playoffs

### Swiss

In the Swiss Rounds section. You can specify the number of Swiss rounds that a tournament will hold.

You can then select a Defending Roster (usually your own Roster) to open up the Schedule for that roster. The **Analyze Defending Roster** button will select that Roster in the Rosters Drawer for you, allowing you to see its details in the Analysis Panes. If it's already selected, the button does nothing.

A Roster's points are populated automatically based on match scores.

In the Rounds section, you record the following for each round:

- The opposing Roster the defending Roster will be facing. When you do this, those rounds update automatically for the opposing Rosters. This makes filling in a complete Swiss schedule a little easier.
- Record the final score for a Round. This awards points to any relevant players.
- Quickly **Analyze** an opponent's Roster. This button selects their Roster in the Rosters drawer, allowing you to see its details in the Analysis Panes.
- Record **Notes** for a Round, which includes spaces for prep notes and post-mortem thoughts, as well as fields for match replays. Notes are Defending Roster-specific.

**IMPORTANT**: When you update a Round in any way, ALWAYS make sure to click **Save Roster Schedule** at the bottom or it won't save. This is especially important when adding Notes.

### Leaderboard

The Leaderboard tab populates automatically based on the Round scores. 

### Playoffs

The Playoffs tab is similar to the Swiss tab, but is formatted as a standard 12-person tournament bracket. Right now, it's hard-coded to have 12 places. This will change with a later update.

The **Popout Bracket** button gives a zoom-able graphic overview of the playoffs.

The **Autopopulate** button automatically seeds the playoffs based on the leaderboard.

Only the initial seed rounds can be set. The rest of the rounds are populated automatically based on the winners of previous rounds. Winners are specified via the **Score** setting.

Each round has a space for **Notes** like the Swiss rounds.

**IMPORTANT**: When you update a Round in any way, ALWAYS make sure to click **Save Playoffs** at the bottom or it won't save. This is especially important when adding Notes.

## Team Builder

Rotom Draft features a powerful Team Builder that lets you quickly assemble permutations of the Pokémon on a particular Roster, optimizing for each new opponent.

### Select a League and Roster

Selecting a League is optional, but recommended if you have more than one League saved to Rotom Draft. This filters the list of Rosters below.

Select a Roster from the dropdown or click **Load Current** to load in whichever Roster is selected in the Rosters Drawer.

### Creating a New Team

1) Click **New Team** and give the new Team a name. 
2) Optionally adjust the Team Size if you want to add more than the standard six Pokémon.

NOTE: It is common to make "Full Roster" teams of all ten Pokémon in an opposing Roster to allow for easy calc'ing in the Battle Calculator.

3) Simply Click and Drag the desired Pokémon from the Roster Pokémon ribbon to the appropriate Team slot!

### Managing Existing Teams

There are several buttons that let you manage existing teams easily:

- Rename
- Delete
- Duplicate
- Import Paste
- Export Paste

The **Import Paste** button lets you import a team using a PokePast.es URL or the Showdown notation copied right from Showdown.

The **Export Paste** bitton lets you copy the current team's data to your clipboard using Showdown notation.

You can re-arrange Pokémon on a Team by Drag-and-Dropping them from one slot to another

You can overwrite a Pokémon on a Team by dragging a new Pokémon from the Roster Ribbon onto the slot in question.

You can clear a slot by right-clicking and selecting **Clear Slot**.

### Editing Pokémon on a Team

Selecting a slot with a Pokémon in it will open the Team Slot Detail window. This lets you view and edit everything about a Pokémon.

- All stat calculations are based on Level 50 Pokémon.
- Abilities and Movesets are derived from a Pokémon's available Moves & Abilties. 

**NOTE**: It is **HIGHLY** recommended to have the Team Builder open in conjucntion with the Moves tab of the Pokémon Analysis Pane (detailed below). This lets you see a Pokémon's learnet in detail with advanced filters and metrics.

When populated, each Move has an Info button that lets you see the move's effects in detail.

Team data autosaves when edited. 

**NOTE**: Rotom Draft's Battle Calculator is extremely powerful and integrates seamlessly with the Team Builder. You may prefer to simply populate a Team in the Team Builder and edit the Pokémon in the Battle Calculator instead. This is a common workflow. See the Battle Calculator explanation below for details.
