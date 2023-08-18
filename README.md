# maid

Enforces a whitelist upon the files that are present in the `$HOME` directory
and purges any non-allowed files to `$MAID_TEMP_FILES`, before attempting to
move them to system's trash using the `trash` cmd.

To make a whitelist:
```bash
ls $HOME -a > $XDG_CONFIG_HOME/maid
```
Then delete `.` and `..`. Remove any unwanted files.
Then run this script to clear.
You are able to use the same syntax `find` uses in order to match to multiple
files.

To install just copy the file contents into `~/.local/bin/`, or any directory in
your `$PATH`.

Author: ayham
Website: ayham.xyz
Licence: Unlicense license

