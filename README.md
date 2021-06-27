# osuReplayEditorV3

The continuation of the replayEditorV2. Old software did not work properly, this one should be better.

Requires 64 bit Windows.

# Download

You can find all the downloads on the [releases page](https://github.com/thebetioplane/osuReplayEditorV3/releases)

Or use this direct link to .zip file: https://github.com/thebetioplane/osuReplayEditorV3/archive/beta.zip

Extract it and run the .exe. The first time it runs it will prompt you to edit your settings file. The settings file should be edited to point towards your osu! installation. The application will stay up to date with this repo unless the "update_url" setting is changed or deleted.

# Keybinds

* A - scrub backwards
* D - scrub forwards
* (scrub speed dependent on playback speed... for finer control lower the playback speed)
* S - toggle play / pause
* I - mark in
* O - mark out
* M - mark mid
* Mouse wheel - zoom
* Right click = pan
* R - reset zoom pan
* Ctrl+Z - undo
* Ctrl+Y - redo

# How do selections work? What is marking?

Right now the only way to make a selection is by choosing a starting frame (mark in) and an ending frame (mark out) which will drop two triangles showing where these marks lie. The mark goes off the current cursor position, so I recommend scrubbing (A / D) to find your spot. Changing the key presses will affect all marks in your selection -- all marks between mark in and mark out.

A middle mark (white) gets created automatically when both marks are set, but fine tune with with mark mid (M). This mark you can click and drag with your mouse to move the path of the cursor. The algorithm is a weighted average based on distance: mark in and mark out are locked in place while the marks in between are pulled depending on how close they are to mark mid.

# Reporting bugs / feature requests

If you encounter a bug then please tell me about it using the Github [issues page](https://github.com/thebetioplane/osuReplayEditorV3/issues). It is possible that your bug is already reported as well. If the program crashed then please also attach or copy/paste the contents of the "crash.log" file that was created.

# Disclaimer on replays produced

The replays produced are designed to be read and played back by osu! client successfully, but please advise that the .osr is not a 100% accurate representation of one that would be produced by the game. For example, the replay hash, online id, seed, etc. are not guaranteed to be correct for score submission. This is not designed to be cheat software.

# License

This software costs no money. Redistribution is allowed as long as no modification is made to any DLL or EXE and this README file is also reproduced. Content in the asset directory can be modified. I take no responsibility for what you might get downloading this software from places besides this Github page.

Right now the full source code is not available. This repo is binaries only. In the future I might GPLv3 this and provide source.

# Donate

Developing this software does take time and was highly in demand going off the Github issues created on the old V2 repo, so if you like the software then you can show your appreciation by donating. But rest assured if you do not donate that this software will still be free.

BTC: `bc1qn8g579mdawh3n6tt9u8s7dr7cyq6ex973vuxvm`

