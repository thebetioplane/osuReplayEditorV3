# osuReplayEditorV3

The continuation of the replayEditorV2. Old software did not work properly, this one should be better.

Requires 64 bit Windows.

# Download

You can find all the downloads on the [tags page](https://github.com/thebetioplane/osuReplayEditorV3/tags)

Or use this direct link to .zip file: https://github.com/thebetioplane/osuReplayEditorV3/archive/beta.zip

Extract it and run the .exe. The first time it runs it will prompt you to edit your settings file. The settings file should be edited to point towards your osu! installation. The application will stay up to date with this repo unless the "update_url" setting is changed or deleted.

# Source Code

This repository is binaries only. For the source code please use this other repo:

https://github.com/thebetioplane/osuReplayEditorV3_SRC

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

Selections work off a starting frame (mark in) and an ending frame (mark out) shown by two triangles. There are two ways to get this selection. The first is to just click and drag while the tool is set to "select" which draws a box. Any frames inside this box are selected. The second is to scrub (A / D) until the cursor is where you want the mark to be and then press the "Mark In" or "Mark Out" buttons (or I / O keys). Changing the key presses will affect all marks in your selection -- all marks between mark in and mark out.

A middle mark (white) gets created automatically when both marks are set, but fine tune with with mark mid (M). This mark you can click and drag with your mouse to move the path of the cursor. The algorithm is a weighted average based on distance: mark in and mark out are locked in place while the marks in between are pulled depending on how close they are to mark mid.

# Reporting bugs / feature requests

If you encounter a bug then please tell me about it using the Github [issues page](https://github.com/thebetioplane/osuReplayEditorV3/issues). It is possible that your bug is already reported as well. If the program crashed then please also attach or copy/paste the contents of the "crash.log" file that was created.

If your bug is related to the accuracy analyzer, then also attaching the "accuracy_analyzer.log" file after running `Help > Analyze Acc Trace` will be a big help for diagnosis.

# Disclaimer on replays produced

The replays produced are designed to be read and played back by osu! client successfully, but please advise that the .osr is not a 100% accurate representation of one that would be produced by the game. For example, the replay hash, online id, seed, etc. are not guaranteed to be correct for score submission. This is not designed to be cheat software.

# License

Please see: https://github.com/thebetioplane/osuReplayEditorV3_SRC