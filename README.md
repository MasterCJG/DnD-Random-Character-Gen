# 5e Character Roller

A single-page web app that randomly generates a complete Dungeons & Dragons 5th Edition character sheet.

## Features

- Random race, class, level (1-20), background, alignment, and name, or pin any of them
- Ability scores (4d6 drop lowest, assigned by class priority) with racial bonuses and level-up improvements
- Combat block: HP, AC, Initiative, Speed, Proficiency, Passive Perception, Hit Dice, Spell Attack, Spell DC
- Saving throws and all 18 skills with proficiencies
- Subclass (only shown at the level the class chooses one)
- Starting equipment, background gear, and alternate starting gold
- Random spells with slots, plus damage dice, attack bonuses, and save DCs
- Appearance, faith, background description, traits, ideals, bonds, and flaws
- Class, subclass, and species feature lists
- Tap any modifier, attack, or damage to roll the dice in a pop-up
- "Copy for Sheets" exports the sheet as tab-separated text you can paste into Google Sheets

## Run locally

Open `index.html` in any modern browser. No build step or dependencies.

## Host on GitHub Pages

1. Create a new repository on GitHub and upload the contents of this folder.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. After a minute, the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Install as an Android app

Open the live site in Chrome, tap the three-dot menu, then tap **Install app** (or **Add to Home screen**). The app opens full-screen and works offline after the first visit.

When you change `index.html`, bump the `CACHE` version in `sw.js` so installed copies update.

## Customizing

All data (races, classes, spells, subclasses, features) and logic live in the `<script>` block of `index.html`. Colors are CSS variables at the top of the file and follow the visitor's light or dark mode.

## Notes and limitations

- Based on the 2014 Player's Handbook races and classes, plus some Xanathar's and Tasha's subclasses.
- Spell lists are a trimmed selection, and spell damage is shown at the spell's base level.
- Subraces, Warlock Mystic Arcanum, subclass spell lists, and later subclass features are not modeled.
- D&D is a trademark of Wizards of the Coast. This is an unofficial fan tool.
