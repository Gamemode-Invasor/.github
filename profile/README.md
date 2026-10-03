<p align="center">
  <img src="invasor.svg" alt="Invasor logo: a pixelated alien above a gamepad" width="160">
</p>

# Invasor

**English** · [Español](https://github.com/Gamemode-Invasor/.github/blob/main/profile/README.es.md)

*A small panel that lives inside Steam, made to be used with a controller from the couch.*

An alternative to Decky Loader, designed to break less and to survive Steam updates. Invasor doesn't aim to compete
with Decky Loader or to dethrone it: it is simply a light and simple alternative.

<p align="center">
  <img src="img/Artwork.jpg" alt="The Invasor panel open over Steam's library in Game Mode" width="720">
</p>

## What is it?

Invasor adds one extra tab to Steam's controller interface (**Game Mode** and **Big Picture**), on the Steam Deck,
the Legion Go, other handhelds, or any Linux PC running Game Mode. Press **L3 + R3** and the panel opens. Close it, and
you are back in your game.

Inside, every feature is its own little **module**. Use the ones you like, switch off the ones you don't.

## A quick look

<p align="center">
  <img src="img/Frame-Generation.jpg" alt="A game's page in Steam with the Invasor panel showing frame generation options" width="720"><br>
  <em>Frame generation options for the game you have selected.</em>
</p>

<p align="center">
  <img src="img/Settings.jpg" alt="The Invasor settings: installed modules, controller shortcut and panel options" width="720"><br>
  <em>Settings: turn modules on and off, install new ones, and choose how to open the panel.</em>
</p>

## Some modules

| | |
|---|---|
| **[Artwork](https://github.com/Gamemode-Invasor/invasor-artwork)** | Find community artwork for your games and shortcuts and apply it without leaving the couch. |
| **[Deckico](https://github.com/Gamemode-Invasor/invasor-deckico)** | Puts each game's icon on its hidden Proton folders, so you can tell which one belongs to which game. |
| **[Patito](https://github.com/Gamemode-Invasor/invasor-patito)** | Frame generation per game, with lsfg-vk. Pick a profile and play. |
| **[Pescao](https://github.com/Gamemode-Invasor/invasor-pescao)** | The same idea with MAKO Renderer: frame generation and scaling per game. |
| **[GE-RR](https://github.com/Gamemode-Invasor/invasor-ge-rr)** | Keeps the latest GE-Proton installed under one name, so you never have to re-pick it after an update. |
| **[Noty](https://github.com/Gamemode-Invasor/invasor-noty)** | Shows Steam notifications from your own scripts. |

## Why Invasor?

- **Built to survive updates.** It doesn't lean on Steam's inner workings. Like anything that plugs into Steam it can
  still break, but it is not as fragile as other tools of its kind.
- **Light.** With everything loaded it uses about 38 MB of memory and around 1 % of one CPU core.
- **No admin password.** It runs as you and never asks for root.
- **One broken module doesn't break the rest.** If a module fails, only its own tab is affected.

## Try it

1. Download the latest release from the [Invasor repository](https://github.com/Gamemode-Invasor/invasor).
2. Unpack it and double-click the installer.
3. Restart Steam once. That's it.

The step-by-step instructions are in that repository's README. Modules are installed from a zip, right from the
panel's settings.

## Make your own module

A module can be as small as a single settings file. There's a template to start from and a guide that explains
everything: see [how to write a module](https://github.com/Gamemode-Invasor/invasor/blob/main/docs/MODULES.md).
The template is MIT-licensed, so you can start from it with any license you like.

## The small print

- Invasor is free software, under the GPL-3.0-or-later license.
- A module is code that runs on your device: install only the ones from people you trust.
- Invasor is not affiliated with Valve, SteamGridDB, lsfg-vk, MAKO, GloriousEggroll or any of the projects its
  modules work with. Please don't report problems with Invasor or its modules to them.
- In the spirit of transparency: AI tools were used at some points in this project. They were directed and
  orchestrated by an experienced engineer, who makes every decision about the architecture and the design.
- Made by [FranjeGueje](https://github.com/FranjeGueje).
