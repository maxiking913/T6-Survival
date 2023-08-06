# T6-Survival
A MW3 inspired Gamemode. Back in the days i spend days in this Mode.
Then after Bo2 had his GSC breakthrough 10 Years or so ago i created an buggy shitty version of this.
Old Link: https://nextgenupdate.com/forums/black-ops-2-gsc-mods-scripts/807231-game-mode-survival-v14a.html

Now i got back into BO2 and completely rewrite from scratch.

This is ment to be played on Plutonium T6 Multiplayer.
I only give support for Server Mode but it should work on Private Game too.

No need to set any Dvars but you can set the Dvar for bot difficulty.

# Upload on next Version 1.5

# ToDo (Top to Bottom Prio)
```
FIX IMPORTANT: _weapon.gsc exceeded maximum number of parent server script variables / need attachment checker max 3 and check for invalid combos (didnt wanted to do that sadly need to crashes server)

-Make Bosses look more like Bosses
-Perma V-Sat Killsteak
```

# Currently in testing 
(working but still not on live - lets call it PBE)
```
-Respawn at Round 10+ will be with $800. Buy 1x Health and 1 Weapon to not die instantly in high Rounds.
-Revive and give Money to others not working on yourself anymore .
-Joining after Round 1 should trigger respawnmonitor
-Self Revive (can be bought in shop. If solo play you will get one free at the start of round 2 since round 1 is a init round and in round 1 connecting players will spawn and not be dead)
-Fixxed: -buying health will now add +100 to max health and not current health
-Fixxed: -Round Respawn while whole intervall and not just on roundend (moved the function form level to a self monitor)

```

# Features added in next Version
```
(Everything in "Currently in testing" for this Release)

-Knife kills give $80

-War & Death Machine Ammo costs $500 (No refill all Weapons aviable when they are in inventory)

-Increased kills for Round to End. Also scaling now with each player and rescale if player quits

-Vote to skip interval (tested with more players)

-Share Money with other Players - Costs $50 / Retrieve $50

-Revive Player in Round $500

-Perk Shop

-Custom Perk:
  More Money

-Fast Buy Ammo @Essential Shop

Fixxed:
-Fix: Quick Ammo buy now doesnt buy 3 times in a row
-FIX: Ammo refill for both weapons 
-FIX: Max ammo after Bossrounds only for current Weapon (now for both)
-FIX: KillHud now working the right way in Boss Rounds
-FIX: Death and War Machine
-FIX: Round doesnt end when 2+ players each kill a bot at the same time
-FIX: Last killed Bot before roundend and Bossbot name now visible in killfeed 
```

# Changelog
Big Update 1.4:
```
-More Bossbots (Each 10 Round + 1 Bossbot)

-Bossrounds more often:
  20% - Round 5-9
  30% - Round 10-14
  40% - Round 15-19
  50% - Round 20+

-Players are now in Spectator when dead and will be respawned after Round

-Intervall-Handler reworked

-Kills left for Round to end HUD

-Buying HP now increase its cost for every purchase (Resets upon dying)

-Normal Bots increases for each Round (Capped for now on 12)

-Reworked Round calculation. (Now its calculating at roundstart instead of recalculating upon each kill)

-Added Vote System to skip Interval (Life but still in testing)

-Added Notifiers:
  Interval (with vote count)
  Round start (with normal Bots Health)
  Boss Announcer (with Boss HP´s)

-Roundhandler rewritten again

-Shops rewritten again

-NEW: Attachment shop added

-NEW: Nuke! (Nuke wont trigger Max Ammo or Boss Money)

-Each Boss will drop Money upon death ($300)

-After Bossround everyone gets Max Ammo

-Normal Bots now increase their Health starting at Round 10 with +10 each Round

-Bots increase starting at Round 3 and ending at Round 8 with 12 Bots (was Round 6 before)

-Fixxed a bug where Game doesnt end when all Players are dead xd
```
Update 1.3a:
```
-Server Crash Fixxed
```
Update 1.3:
```
-NEW: Essential Shop
```
Update v1.2:
```
-Shops:
  Weapon Shop
  Killstreak Shop
  Grenade Shop
-Overflow Fixxed
```
Update v1.1:
```
-2+ Player Support
```
Initial Release v1.0:
```
-Hud

-Individual Rounds

-Bossrounds

-Money & Health

-Server Implementation
```

Greetings
