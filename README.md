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

## Boat Dismantling (optional)

Boat Anchor can optionally let you dismantle boats with **Hammer → Remove**, blocking removal while a player is onboard or the boat's storage still has items in it.

This is controlled by the **Boat Dismantling → Enable** config option (`true` by default). Turn it off if you'd rather use vanilla behavior, or a different mod, to handle boat (and cart) dismantling:

* When **enabled**, Boat Anchor performs its own onboard/storage safety checks before allowing the removal.
* When **disabled**, Boat Anchor doesn't touch boat removal at all — it doesn't flag boats as removable, doesn't intercept the removal call, and doesn't block anything. Vanilla behavior and any other boat/cart-dismantling mod are left completely free to handle it themselves.

## Changelog

### 1.3.3

* Fixed a compatibility issue where disabling **Boat Dismantling** still blocked other mods (e.g. boat/cart dismantling mods) from removing boats.
* When the **Boat Dismantling** option is disabled, Boat Anchor now leaves boat removal completely untouched instead of forcing it off, so other mods and vanilla behavior can take over cleanly.

### 1.3.2

* Added optional **Hammer → Remove** support for boats.
* Boats can only be dismantled when **no player is onboard**.
* Boats cannot be dismantled while their **storage contains items**.
* Added warning messages explaining why a boat cannot be dismantled.
* Boat dismantling uses Valheim's normal removal behavior so build materials are returned.
* Added a **Boat Dismantling** config option (`Enable = true` by default) to turn the feature on or off without affecting the anchor system.

### 1.3.1

* Boats now continue to bob naturally with the waves while anchored.
* Moved the anchor prompt from the center of the screen to the standard hover-text box.
* The anchor prompt now only appears when looking at the rudder.
* **Shift + E** on the rudder no longer interferes with sitting or steering interactions.
