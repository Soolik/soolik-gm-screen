# Soolik's GM Screen — User Guide

A toolkit for Pathfinder 2e Game Masters on Foundry VTT. This guide explains, for
every feature: what it does, where to find its button, exactly what you click, and
when you would use it.

Works on Foundry VTT v14 (verified on 14.363), Pathfinder 2e system.

---

## Table of contents

- [Getting started](#getting-started)
- [The Control Panel](#the-control-panel)
- [Free features](#free-features)
  - [Accessibility Controls](#accessibility-controls)
  - [Whisper Toast](#whisper-toast)
  - [Whisper Autocomplete](#whisper-autocomplete)
- [Premium features](#premium-features)
  - [Misidentify](#misidentify)
  - [Lore Checks](#lore-checks)
  - [Connection Map](#connection-map)
  - [Emporium](#emporium)
- [Premium: subscribe and install](#premium-subscribe-and-install)
- [Settings reference](#settings-reference)
- [FAQ and troubleshooting](#faq-and-troubleshooting)

---

## Getting started

Soolik's GM Screen comes in two parts:

- **Free** (installed from the Foundry module browser): Accessibility Controls,
  Whisper Toast, Whisper Autocomplete, and the Control Panel.
- **Premium** (a Ko-fi subscription, then a separate add-on you install): Misidentify,
  Lore Checks, Connection Map, Emporium.

Every feature is a separate on/off switch. You turn features on in the **Control Panel**
(or in Foundry's module settings). Turning a feature on or off **reloads Foundry**, so
do it between scenes, not mid-combat.

**Where the buttons live.** Each active feature adds a button to the **Token** scene
controls (the left-hand toolbar, top group). The icons are:

| Feature | Icon | Who sees the button |
|---|---|---|
| Control Panel | dungeon | GM only |
| Accessibility Controls | eye | Everyone (each player) |
| Misidentify | magic wand | GM only |
| Lore Checks | open book | GM only |
| Connection Map | linked diagram | Everyone with board access |
| Emporium | shop | GM only |

Whisper Toast and Whisper Autocomplete have **no button**. They work quietly in the
background once enabled.

---

## The Control Panel

**What it does.** One window that lists every feature with an on/off toggle and an
**Open** button, so you do not have to hunt through Foundry's settings. Premium features
show here too: if you have the add-on installed they work like any other feature; if you
do not, they show as **Locked** with a one-click link to subscribe.

**Where it is.** Token scene controls, the **dungeon** icon ("Soolik's GM Screen").
GM only.

**How to use it.**
1. Click the dungeon icon to open the panel.
2. Each feature row has a toggle (**On / Off**) and, where it makes sense, an **Open**
   button that launches that feature's window.
3. Flipping a toggle reloads Foundry (you are asked to confirm).

**When to use it.** As your home base. Open it to launch any feature, to enable
something you have not used before, or to check what is on.

---

## Free features

### Accessibility Controls

**What it does.** Lets each player adjust **brightness**, **contrast** and **saturation**
of the map on their own screen. It is a personal, screen-only filter: it never changes
the scene, lighting, token vision, or anyone else's view. Two people at the same table
can use completely different settings.

**Where it is.** Token scene controls, the **eye** icon ("Accessibility Controls").
Visible to every player, because everyone sets their own.

**How to use it.**
1. Click the eye icon to open the floating panel.
2. Use the **Filter on / Filter off** switch and the three sliders (brightness, contrast,
   saturation).
3. Pick a **Preset** for a quick setup: *Default*, *Bright Map*, *High Contrast*,
   *Low Saturation*. **Reset** returns to normal.
4. You can also set the same values in **Configure Settings → Module Settings →
   Accessibility Controls**.

**When to use it.** When a scene is too dark to read, when a player needs higher contrast
or less color for eye comfort, or when a map's art fights with token visibility.

**Good to know.** The filter only touches the map canvas, never the chat, sidebars or
windows. On a very large map on weak hardware it can cost a few FPS; turning the filter
off resolves it.

### Whisper Toast

**What it does.** Shows a banner at the top-center of your screen whenever you receive a
whisper, so private messages do not get lost in a busy chat log.

**Where it is.** No button. It appears on its own when a whisper arrives.

**How to use it.**
1. Enable it (Control Panel or module settings). There is nothing else to click during play.
2. When a whisper comes in, the banner shows with a countdown bar. **Hover** the banner to
   pause the countdown; click **Dismiss** to close it early.
3. Tune it in **Module Settings**: display time, maximum banners on screen at once, and an
   optional notification sound.

**When to use it.** Always-on quality of life, especially useful for the GM trading private
notes with players, or for players who miss whispers during combat.

### Whisper Autocomplete

**What it does.** After you type `/w` or `/whisper` in chat, it suggests user and target
names in a dropdown so your whisper goes to the right person, including group targets like
all Players or the GM.

**Where it is.** No button. It hooks into the chat box.

**How to use it.**
1. Enable it (Control Panel or module settings).
2. In chat, type `/w` (or `/whisper`) and start typing a name. Pick from the dropdown,
   then type your message.

**When to use it.** Any time you whisper and do not want to misspell a name or remember who
is who. Helpful at tables with many players or similar character names.

---

## Premium features

> These four are part of the premium add-on. If you have not installed it yet, see
> [Premium: subscribe and install](#premium-subscribe-and-install).

### Misidentify

**What it does.** When a player critically fails an Identify check, you hand them a
convincing **fake** identity for the item instead of just "unidentified." The fake is the
same kind of item (a sword stays a sword, a scroll stays a scroll), sits near the real
level, and gets a believable level-scaled stat block. The truth is stored GM-only, so the
player walks away certain they know what they are holding. Every swap is fully reversible.

**Where it is.** Token scene controls, the **magic wand** icon ("Misidentify"). GM only.

**How to use it.**
1. Open the Misidentify panel.
2. Pick the **Character**, then pick the **Item** they failed to identify. Only items the
   player has not identified appear in the list.
3. Click **Propose a fake**. You get four option cards: three hand-written tiers plus one
   random draw from the source compendium:
   - **Off / uneasy** — reads as plausible, but the description gives the player a vague bad
     feeling with no concrete sign of a real curse.
   - **Ordinary** — a believable, unremarkable item.
   - **Impressive** — the player believes they found something powerful or valuable.
   - **Random** — a real item pulled from the compendium near the right level. Use the
     **Reroll** button to draw again.
4. Compare **Really is** against **Will look like**, then click **Use this** on the option
   you want. The player's item now shows the fake identity, marked as identified.
5. To reverse it: the panel's **Active misidentifications** list has **Undo (restore
   original)** for each one. **Clear deleted entries** tidies up items that were since
   deleted.

**When to use it.** When a player botches Identify and you want a real consequence: a wrong
belief that drives play, rather than a bland "you can't tell." Great for cursed-feeling
loot, traps disguised as treasure, or red herrings.

**Good to know.** The truth (original name, image, description, and which items are faked)
lives in a GM-only journal with no player access, so nothing on the player's copy can leak
the lie. Works for both magic items and alchemical items (poisons, bombs, elixirs).

### Lore Checks

**What it does.** Prepared, **tiered** knowledge checks. You write a topic as a ladder of
DCs: hit the base DC and the player learns the basics, beat higher thresholds and they
learn more. Roll badly and they learn nothing; **critically** fail and they get a
confident, wrong answer. Rolls are **blind** (only you see the dice) and the lore is stored
GM-only, so players never see the thresholds, the answers, or the false lead.

**Where it is.** Token scene controls, the **open book** icon ("Lore Checks"). GM only.

**How to use it.**
1. Open the Lore Checks panel and click **New Lore Check**.
2. In the editor, fill in:
   - **Topic / question** (what can be learned).
   - **Skill** (any Knowledge skill, Perception, or a custom **Lore** with its slug).
   - **Success thresholds** — click **Add threshold** for each tier, giving it a DC and the
     **Revealed text** the player learns at that DC and above. Reveals are cumulative; the
     lowest DC is the base DC.
   - **False info (critical failure)** — a believable lie shown as truth on a critical
     failure (or a natural 1 that drops a failure a step). Leave empty for none.
3. **Save**. Back in the panel, choose the **Player who will roll** and click
   **Post to chat**.
4. The player clicks **Roll (secret)** on the chat card. The blind roll resolves and the
   matching tier, or the false lead, is whispered to them. You see a private diagnostic
   line with the total and outcome.

**When to use it.** For prepared lore you want to dole out by how well the player rolls:
history of a place, a monster's weakness, a faction's secret. Especially good when a wrong
answer on a fumble would be more interesting than a blank.

**Good to know.** Your prepared checks are stored in a GM-only journal folder. Players never
see the DCs or the lie they were handed; they only ever see the answer whispered to them.

### Connection Map

**What it does.** A shared **investigation board**, styled like a tavern notice-board:
stained-wood planks, aged-parchment cards, iron pins, and waxed-red rope between clues. It
is genuinely collaborative: the GM creates a board and players with access pin suspects,
add notes, and string connections in real time while you watch.

**Where it is.** Token scene controls, the **linked diagram** icon ("Connection Maps").
Visible to everyone who has access to a board.

**How to use it.**
1. Click the icon to open the board picker. The GM clicks **New board** to create one
   (each board is a shared journal entry; players you grant access can edit it). Open an
   existing board to keep working on it.
2. **Add nodes**: drag an actor (or item) from the sidebar onto the board to make a card
   with its portrait and a link to its sheet, or click **New node** for a blank card.
3. **Connect**: drag from a node's pin to another node to string a rope between them.
4. **Edit a node**: double-click it. You can set the **Title**, **Notes**, **Color**, the
   **Pin** style, and a **State** (Normal, Wounded, Ally, Enemy, Captured, Dead, Destroyed,
   Missing, Suspect) that shows an art overlay. The GM can also set a node **Image**.
   Optionally, a node linked to an NPC can **auto-update its state** from that actor's HP
   and disposition.
5. **Edit a rope**: click it to set a **Label**, a **Color** (Natural, Red, Green, Blue,
   Purple, Gold, Silver, Black, White), **Thickness**, and **Tension** (how much the rope
   sags).
6. **Navigate**: left-drag draws a selection box, right-drag pans, the mouse wheel zooms.
   Click to select (Shift to multi-select), drag any selected item to move the whole group,
   and **Del** deletes the selection.

**When to use it.** Mystery and investigation sessions: murder boards, conspiracy webs,
who-knows-whom. Let the table build it together so everyone shares the same picture of
the case.

**Good to know.** Only the GM can create or delete boards; players edit content. If you use
the PF2e **Bestiary Tracking** module, met-monster cards get an **Add to connection map**
icon so you can drop them straight onto a board.

### Emporium

**What it does.** Generates a believable **merchant** or a level-appropriate **treasure**
hoard from the PF2e equipment compendium. Preview it, reroll the bits you do not like, then
drop it on the map as a ready-to-use loot actor.

**Where it is.** Token scene controls, the **shop** icon ("Emporium"). GM only.

**How to use it.**

*Merchant mode:*
1. Open Emporium and select the **Merchant** tab.
2. Set the **Merchant type** (16 archetypes: blacksmith, alchemist, scribe, temple, fence,
   and more), the **Location level**, and **Number of items**. Optional knobs: **Price
   modifier %**, **Max rarity**, **Level spread**, **Theme traits** (click the chips), and
   whether to include items that only have placeholder art.
3. Click **Generate** for a preview. Use **Reroll all**, **Reroll this item**, or
   **Remove** to fix the list; **Clear preview** starts over.
4. Click **Create merchant**. A loot actor with a merchant sheet appears in your chosen
   folder.

*Treasure mode:*
1. Select the **Treasure** tab.
2. Set the **Party level** and **Party size**. A live budget bar tracks the official Party
   Treasure by Level allowance as you go.
3. **Generate**, reroll as needed, then **Create treasure**. You get a chest plus coins.

*Custom pool (both modes):* drag your own physical items into the **Custom pool** and give
each a **Chance** to appear in what you generate.

**When to use it.** Whenever you need a shop stocked fast, or a hoard that matches the
party's level without doing the math by hand. The spellcasting archetypes (mage, witch,
druid, temple, scribe) reliably stock scrolls or wands of random spells of their tradition.

**Good to know.** Stock respects sensible rarity caps per archetype and a per-archetype set
of staples (the temple always carries holy water, and so on). Location level is a hard
ceiling, so a low-level town will not stock items above its level.

---

## Premium: subscribe and install

The premium features are a separate add-on, distributed outside the Foundry browser.

1. In the **Control Panel**, the premium section shows the locked features and a
   **Subscribe on Ko-fi** button. Click it to open the Ko-fi page and subscribe.
2. After subscribing you receive a personal **manifest link** to install the premium
   add-on. If you already subscribed, use **Already subscribed? Get your install link** in
   the panel, or the claim page, to retrieve it.
3. In Foundry, go to **Add-on Modules → Install Module**, paste the manifest link into the
   **Manifest URL** field, and install. Enable it, then the premium features appear in the
   Control Panel ready to toggle on.
4. While your subscription is active you get every update; if it lapses, your installed copy
   keeps working but you stop receiving new downloads.

---

## Settings reference

Most day-to-day controls live in each feature's panel. These extra options are in
**Configure Settings → Module Settings**.

**Accessibility Controls**: enable filter, brightness, contrast, saturation.

**Whisper Toast**: enable, display time (seconds), max banners on screen, play a sound,
sound file path.

**Misidentify**: source compendium (default `pf2e.equipment-srd`), level band (how far from
the real level a fake may start), registry journal name.

**Lore Checks**: name of the GM-only journal folder that stores your prepared checks.

**Connection Map**: default pin style, and whether nodes auto-update their state from linked
actors (off by default, so offscreen events are not revealed to players).

**Emporium**: the folder where generated merchant and treasure actors are created.

---

## FAQ and troubleshooting

**A feature's button is missing.** It is probably turned off. Open the Control Panel and
toggle it on (Foundry reloads). Remember some buttons are GM-only.

**Toggling a feature reloaded my game.** That is expected. Feature on/off switches need a
reload, so change them between scenes.

**Players cannot see a connection map.** Only the GM creates boards, and a player needs
access to that specific board. Create or share one for them.

**The premium features show as Locked.** The premium add-on is not installed. Subscribe on
Ko-fi and install the add-on with your personal manifest link (see above).

**Will Misidentify or Lore Checks leak the secret to players?** No. Both keep their hidden
data in GM-only journals with no player access, and Misidentify writes nothing
revealing onto the player's item.
