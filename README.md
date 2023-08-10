# Salvo!

Originally a pencil-and-paper game, Salvo! is the precursor to Milton Bradley's Battleship.
In this version for MakeCode Arcade, up to four players can participate, with any combination of human and computer players.
Multiplayer is local; JACDAC is not currently supported.

## Rules

If you are familiar with Milton Bradley's Battleship, then Salvo! will be familiar to you.
Players first place their fleet on their own boards. Then, in each round, players select
locations on opponents' boards to send torpedoes.

In each round, a player can fire as many torpedoes as there are ships in the fleet.
Each player starts with seven ships, so players start with seven torpedoes per round.

When a player's torpedo hits an opponent's ship, the hit is registered with _all_
players. Similarly, when a ship is sunk, _all_ players will know about it.

The game ends when one player has eliminated all others, or when no players have
ships remaining. (Yes, a draw _is_ possible.)

Players should keep their fleet locations secret. Shot selection also should
be done in secret, although players can form alliances if they wish. Thus, when there
are multiple human players, each player should be permitted privacy when operating
the game.

## Fleet Configuration

### Standard Salvo Fleet

Quantity | Ship | Size
--- | --- | ---
1 | Aircraft Carrier | 5
1 | Battleship | 4
1 | Cruiser | 3
2 | Destroyer | 2
2 | Submarine | 1

## TODO

- [ ] Improve the AI (refer to function `takeAiTurn`).
- [ ] Allow for randomized turn order each round (refer to function `setTurnOrder`).
- [ ] Allow player to select fleet type used in the game.
  - [ ] Add an option screen.
  - [ ] Modify global variable `fleetStyle`.
- [ ] Add JACDAC support.
- [ ] Allow players to choose a randomized fleet placement (difficult).
- [X] Add legend to shot selection screen. (Done - version 1.0.)
- [X] Give option to show player boards at the end of the game. (Done - version 1.0.)

## License

### MIT License

Copyright 2019 Robo Technical Group LLC.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software
and associated documentation files (the "Software"), to deal in the Software without restriction,
including without limitation the rights to use, copy, modify, merge, publish, distribute,
sublicense, and/or sell copies of the Software, and to permit persons to whom the Software
is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Supported targets

* for PXT/arcade
(The metadata above is needed for package search.)



> Open this page at [https://memesstubs.github.io/battleships/](https://memesstubs.github.io/battleships/)

## Use as Extension

This repository can be added as an **extension** in MakeCode.

* open [https://arcade.makecode.com/](https://arcade.makecode.com/)
* click on **New Project**
* click on **Extensions** under the gearwheel menu
* search for **https://github.com/memesstubs/battleships** and import

## Edit this project ![Build status badge](https://github.com/memesstubs/battleships/workflows/MakeCode/badge.svg)

To edit this repository in MakeCode.

* open [https://arcade.makecode.com/](https://arcade.makecode.com/)
* click on **Import** then click on **Import URL**
* paste **https://github.com/memesstubs/battleships** and click import

## Blocks preview

This image shows the blocks code from the last commit in master.
This image may take a few minutes to refresh.

![A rendered view of the blocks](https://github.com/memesstubs/battleships/raw/master/.github/makecode/blocks.png)

#### Metadata (used for search, rendering)

* for PXT/arcade
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
