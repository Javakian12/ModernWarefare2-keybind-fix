# ModernWarefare2-keybind-fix
# Fixes the keybinds on mw2. Specifically, sets night vision to "J"

# How To Implement
First, go to the current location of your keybinds file, usually it is in `\Users\(your user)\Documents\Call of Duty MWII\players\`. There should be two folders here, one that says `cod22` and another that is some random number. Choose the random number folder, and find `keybinds.kb`.

**RENAME** the current keybind file to `keybinds_original.kb`. This saves your current keybinds, so you do not accidentally lose them. Then, place the new `keybinds.kb` file in that same folder.

Lastly, right click on the `keybinds.kb` file, hit "properties", and select "Read Only" then hit "Apply". This prevents the game from overwriting that file if the checksum doesn't match.

After, load the game, and the night vision keybind should be the letter "J". All other keybinds are standard, default binds.

# Why This Happens
There is a bug in the MW2 campaign that prevents the settings menu from opening. Because of this, you cannot set the night vision keybind, which commonly conflicts with auto sprint button. This makes some of the missions suck, so it addresses that, as it is much more fun to play the game as it was intended.

`keybinds.kb` is a custom file format in binary. It cannot be edited from a notepad, so I had to edit the hex of the file to specifically alter the keybind. Everything else other than night vision is the same.

If you want to change normal graphic settings, you can find them in `options.3.cod22.cst` in the `players/` folder. That file can be edited with notepad, so no new file needed.
