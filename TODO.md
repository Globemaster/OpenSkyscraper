OpenSkyscraper TODO
===================

Background
----------

- Put background drawing stuff into its own `Background` class
- Figure out drawing of the sky sprites. Now they're showing the raindrops.


Tower
-----

### Drawing
- Reorganize tower stuff into *game/tower" directory
- Add the little crane from SimTower. Whenever the Tower's height changes, the crane is positioned at the left edge of the item that caused the height increase.
- Add the city background (it's in 065)
- Draw the fire ladders on the far left and right of each floor; also on the lobby floor. (they're in 075)
- Add clouds to the sky
- Add *funds*, *star rating*, *time* and *date* to the `Tower` class and animate them


Items
-----

- Disable the progression of the construction animation for draggable items.
- When two adjacent items are collapsed, they both show the construction animation. It should be possible to only show the animation for the part that was actually added to cause the collapse.


Lobby
-----

- The `Lobby` needs it's entrance decorations on the left and right side to be drawn
- Multiple unconnected lobbies on the ground floor allowed. This should *not* be the case!
- `Lobby` shouldn't show construction step bitmap 212
- `Lobby` needs a texture (don't know where to find it though�)


User Interface
--------------

- Figure out a way to draw the UI (windows, sprites, entities, hierarchies, etc.)
- Create `Tools`, `Map` and `Control` windows that also were in the original SimTower.


Audio
-----

- Initialize OpenAL or whatever we will use for audio
- Create `Sound` class
- Create `SoundEmitter` class
- Locate listener at the center of the screen (POI of the `TowerScene`)