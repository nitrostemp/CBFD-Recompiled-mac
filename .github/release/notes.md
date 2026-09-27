Ready-to-play builds for Windows, Linux and macOS, from the macOS fork of [CBFD-Recompiled](https://github.com/sciaschi/CBFD-Recompiled): upstream's game with macOS support added. Its versions end in `-mac`, to tell them apart from upstream's releases. **You need your own US ROM of Conker's Bad Fur Day**: these packages contain no game data.

1. Download the package for your system and unpack it anywhere.
2. Run `ConkerRecomp` (`ConkerRecomp.exe` on Windows, `ConkerRecomp.app` on macOS).
3. The first time, the launcher asks for your ROM: pick your US `.z64`. Then Start Game.

ROM hacks that only change the game's assets, such as an uncensored patch that restores the bleeped words, play too (bring your own patched ROM: none is included). Add the patched `.z64` with the launcher's **Version** option, which then shows which ROM is in play and switches between the ones you've loaded; the window title shows it too. Saves are shared. Hacks that change the game's code are refused.

Linux needs SDL2, GTK 3 and FreeType (Ubuntu/Debian: `sudo apt install libsdl2-2.0-0 libgtk-3-0 libfreetype6`) and a Vulkan driver.

macOS needs Apple Silicon and macOS 15 or later. The app isn't signed with an Apple developer ID, so macOS blocks it the first time: open it once, then choose **Open Anyway** in System Settings > Privacy & Security (or run `xattr -dr com.apple.quarantine ConkerRecomp.app` in Terminal first).

To build it yourself instead, see the [README](https://github.com/nitrostemp/CBFD-Recompiled-mac#readme).
