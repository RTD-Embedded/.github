# Visual Studio 2022 and above scripts

This is a location to include Gremlin tools related
to VS2022.

## vs_upgrader.py

This script is designed to upgrade our drivers (pre 2025) from using
makefiles to using project/solution files which stopped supporting
makefiles in v8.1 or something.

I've only designed this on MURAL board. I am not sure what you'll have
to change for non-MURAL boards.

Usage: You just need to pass the board
name and the current version of the installed WDK on your device.

***See OneNote on migrating to VS2022 for full details***

### template.inf

Used by the script above `vs_upgrader.py`. This is an inf file that gets string
substitution based on the function: `gen_inf()`.
