# Matrix
Matrix style screen saver

This is a "Matrix" style screen saver for RISC OS 4 and above, and has been adapted from code by [Jacob Sorber](https://www.youtube.com/watch?v=K8dCh3ZMLN8).
Gamma fade code (C) Geoff Steeper.


# Installation

Copy the directory "!Matrix" into your screen savers directory (BootResources:Configure.ScrSavers) in order for it to appear on the list of available screen savers.

It requires version 0.50 or later of the ZapRedraw module. This module comes as part of !ZapFonts, which can usually be found in "BootResources:". The latest version can be found in Zap Ultimate which is available via PlingStore (!Store).


# Configuration

Whilst the screen saver will configure itself to your screen mode, there are a number of configuration options available, which can be specified in a text file "Choices:ScrSavers.Matrix"

Title:
  This is the number of centi-seconds before the title starts to fade.
  For modes with 85 text rows or less then suggest using 250 otherwise 550.
  Maximum is 600.

Delay:
  This is the number of centi-seconds between Wimp polls.
  For modes with less than 85 text rows suggest using 16 otherwise 4.
  Maximum is 50.

Fade:
  This controls whether the Desktop is faded or not when the screen saver is run. Set to 0 for no fade, or any non-zero value to fade the Desktop

CharDbl:
  This controls whether to use double height characters or not. Set to 0 for single height characters, or any non-zero value for double height.
  For modes with 115 text rows or more suggest using 1 otherwise 0.


# History

1.00 : Initial release

1.01 : Minor fix to !Run file for ensuring ZapRedraw is loaded

1.02 : Minor fix to require ZapRedraw 0.50 although 0.49 also seems okay

