# holo_deck
build in a whole new way

## Todo

> Last Updated: June 16, 2022

* Using [mapblock_lib](https://content.minetest.net/packages/BuckarooBanzay/mapblock_lib/) to perform serialize and deserialize operations
* Make a schematic that's 1 map block bigger (our walls)
* Support a loaded and unloaded option
* Support detecting if the player is near a wall, the floor or roof to move based on "world" dimensions (Support some handle for world boundaries)
* Support attempting to build custom entities for depicting another player in the same "virtual" world (but both must work together to save, i.e. whats different with what we have saved already and what's changed between both players)
* Build some prebuild areas for players to explore in.

## How it will work

The player will access either a node or via chat command to be summoned into a holo_deck "instance".

From there via chat commands the player can then load, save or create a map (a completely "virtual" world that doesn't fully exist in the actual world).

When the player moves to an edge the player is teleported to a position and that mapblock is loaded into the instance.

For v1.0 we will be focusing on making this work, and work well with multiple instances being operational (especially if a "virtual" world is read only, each player gets a copy of their own world where they can destroy or what ever, but saving will be disabled for read onlies unless the player really wants to then they can make a fresh copy and open that as read/write).

For future versions we will then be expanding the idea of multiple players sharing the same world but in 2 different instances (Why 2 instances? because then it's truly a holo_deck, I could explore the roof while you could explore the basement).
