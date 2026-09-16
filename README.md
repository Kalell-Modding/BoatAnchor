# ⚓ Boat Anchor

Tired of your boat slowly drifting away while you're building, fishing, or taking a break?

**Boat Anchor** lets you drop an anchor on your boat to keep it in place horizontally while still letting it naturally rise and fall with the waves.

No more coming back to find your boat halfway across the ocean.

## How to Use

1. Look at the **rudder** of your boat.
2. Press **Shift + E** to drop or raise the anchor.
3. The anchor prompt will appear in the normal hover-text box alongside the vanilla steering prompt.

That's it. Drop the anchor and your boat stays where you left it.

## Requirements

* [BepInExPack Valheim](https://thunderstore.io/c/valheim/p/denikson/BepInExPack_Valheim/)

### Multiplayer

**Everyone playing on the server needs to have this mod installed**, including the dedicated server if you're running one.

The anchor's physics are handled by whichever player currently owns the boat. If someone without the mod takes control of an anchored boat, they won't be able to raise or lower the anchor, and the boat may stop staying anchored when ownership changes.

## Notes

* The anchor prevents horizontal **X/Z movement**, but the boat can still naturally bob up and down with the waves.
* Anchor state is saved with the boat and persists through logging out and back in.

## Changelog

### 1.3.0

* Boats now continue to bob naturally with the waves while anchored.
* Moved the anchor prompt from the center of the screen to the standard hover-text box.
* The anchor prompt now only appears when looking at the rudder.
* **Shift + E** on the rudder no longer interferes with sitting or steering interactions.
