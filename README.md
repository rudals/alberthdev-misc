# alberthdev-misc
Miscellaneous things I've created that are not big enough for a
dedicated repository, and are not small (or useless) enough for a Gist!

## Subprojects:

 * [HexChat - Debian Stretch To Jessie Package Converter][p1] -
   a simple shell script to convert a Debian Stretch HexChat package to
   a Jessie-compatible one. The stretch package is backwards-compatible
   with Jessie, but a dependency must be renamed for the package to
   install. The script provided here automates the process.

 * [Qt QtQuick Static Patches][p2] -
   patches to enable fully static compilation for Qt, whether on
   Windows or other platforms. (This is meant especially for Windows
   for those aiming to distribute a single executable.) Note that
   this still requires the relevant OpenGL/DirectX/Mesa DLLs to run,
   which unfortunately is still a limitation for QtQuick. I recommend
   bundling all three graphics DLLs to maximize compatability on
   all machines!
   
   Currently, patches are provided for Qt v5.6 and v5.7. They are
   from [this issue](https://bugreports.qt.io/browse/QTBUG-28357),
   and modified to support various other modules as well.

[p1]: HexChat_Debian_Stretch_To_Jessie_Package_Converter/
[p2]: QtQuickStaticPatches/