# osu-replay-anticheat
ORA is a tool developed to detect osu! cheats using replays.

## How it works
Basically, when something suspicious is detected in a replay, it adds a value (which increases or decreases based on how likely they are cheating for that check) to the "violationl evel". This basically means the higher the violation level, the more likely they are to be cheating.

If a player sets off one of the checks, it gives specific details about what was detected (for example: "The player had an unstable rate of 25, and therefore ? has been added to the violation level. Unstable rate this low often indicates relax cheats.").

## What it detects
Aimbot/Aim Assist - Detects these by checking for cursor teleports, cursor speed consistency, how close the cursor is to the center of a circle, patterns, etc.

Relax - Detects this by checking the unstable rate and checking tapping consistency.

Difficulty Changer (CS, HP, and OD) - Detects these by verifying that the player actually hit the notes.

Replay Copier - Detects this by comparing 2 replays.

Timewarp - Detects this by checking the average frame time.

