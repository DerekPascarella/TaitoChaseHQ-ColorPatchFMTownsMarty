## Taito Chase H.Q.

Thanks to some research done by Kitrinx during her development of the FM Towns Marty core for the MiSTer FPGA, insights were gained to make it possible to develop this patch to correct the flickering horizontal lines and discolored bands seen when playing "Taito Chase H.Q." on the FM Towns Marty. The game switches color palettes during each frame, but its original timing causes parts of the picture to appear in the wrong colors on Marty hardware.

This fix only applies to the game's "MODE 1" display mode, which is the only of the two modes that renders correctly on Marty hardware. As a result, the default display mode has been changed from "MODE 2" to "MODE 1".

⯈ Download Patch: [Taito Chase H.Q. (Marty Color Palette Fix).zip](xxx)

## Patching Instructions

This patch release includes a custom patch-applying kit. It specifically targets the [Redump rip](https://redump.info/disc/68172) of "Taito Chase H.Q.", and no other version of the original source disc image can be used.

To apply the patches, follow the steps below.

1. Extract the [latest release package ZIP](https://github.com/DerekPascarella/TaitoChaseHQ-ColorPatchFMTownsMarty/raw/refs/heads/main/Taito Chase H.Q. (Marty Color Palette Fix).zip) to any folder of your choosing.
2. Place the entire Redump disc image in the `redump_original` folder.
3. Launch the `apply_patch.bat` script and watch for status messages as it applies the patch.
4. Upon successful completion, patched disc images will reside in the `patched_disc_image_cue_bin` and `patched_disc_image_ccd_img_sub` folders. These disc images are acceptable for burning to CD-R, using with an ODE, or using with an emulator.
