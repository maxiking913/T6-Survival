# T6-Survival
A MW3 inspired Gamemode. Back in the days i spend days in this Mode.
Then after Bo2 had his GSC breakthrough 10 Years or so ago i created an buggy shitty version of this.
Old Link: https://nextgenupdate.com/forums/black-ops-2-gsc-mods-scripts/807231-game-mode-survival-v14a.html

Now i got back into BO2 and completely rewrite from scratch.

This is ment to be played on Plutonium T6 Multiplayer.
I only give support for Server Mode but it should work on Private Game too.

No need to set any Dvars but you can set the Dvar for bot difficulty.

# Upload on next Version 1.5 (Current Game State 5.09.2023 - Upload will be when the Variables Leak is fixxed):
```
Came into Game LImitations. I have a workaround. will implement it some times next week but currently my time is limited.
```

Old:
As it seems there are no variable leaks.
```
child var allocations where count > 1

total: 0, total calculated: 327
```
```
child var allocations where count > 1

total: 0, total calculated: 26782
```
```
child var allocations where count > 1


total: 0, total calculated: 30029
```
Checking further now. Also made thread at [Plutonium](https://forum.plutonium.pw/topic/32144/exceeded-maximum-number-of-parent-server-script-variables):
You can post there or write me here if you have suggestions or the idea to fix.


# ToDo (Top to Bottom Prio)
```
-PET SHOP - Perma Dog / Perma Hunter Killer
-Perk (inc melee range,self revive+ - save everything including perks weapons etc after dead, golden knife / golden sniper - oneshot in non bossorunds / double dmg in bossrounds)
-custom boss perks (money remover, no health recovery or other stuff)
-Drops like ammo/instakill/money


-FIX:bug lost weapon dying in bossround (happend once cant be replicated)
-Make Bosses look more like Bosses
```

# Currently in testing 
(working but still not on live - lets call it PBE)
```
-Bosses now sometimes has air support or grouns support:
  -Air Support 20%
  -Ground Support 20%
  -Air and Ground Support 10% (Not before Round 10+)

-3rd Weapon Perk
-Added shop checks so only allies get the shop info and not bots (fixxed the random server crash)

-Fixxed: Random Server Crash
```

# Features added in next Version
```
(Everything in "Currently in testing" for this Release)
-Attachment checker

-Reworked Intervall message & handler

-Changed various shop prices

-Self Revive (can be bought in shop. If solo play you will get one free at the start of round 2 since round 1 is a init round and in round 1 connecting players will spawn and not be dead)

-Respawn at Round 6+ will be with $1000. (Only if you have less than $1000. Also triggers if respawned by player)

-Balistic Knife and Added:Knife now Free in Weaponshop

-Knife kills give $80 (Also scales with Money Perk)

-War & Death Machine Ammo costs $500 (No refill all Weapons aviable when they are in inventory)

-Increased kills for Round to End. Also scaling now with each player and rescale if player quits

-Vote to skip interval (tested with more players)

-Share Money with other Players - Costs $50 / Retrieve $50

-Revive Player in Round $500

-Perk Shop

-Custom Perk:
  -More Money
  -Perma UAV

-Fast Buy Ammo @Essential Shop

Fixxed:
-Fix: Quick Ammo buy now doesnt buy 3 times in a row
-FIX: Ammo refill for both weapons 
-FIX: Max ammo after Bossrounds only for current Weapon (now for both)
-FIX: KillHud now working the right way in Boss Rounds
-FIX: Death and War Machine
-FIX: Round doesnt end when 2+ players each kill a bot at the same time
-FIX: Last killed Bot before roundend and Bossbot name now visible in killfeed
-FIX: Select Fire Mode not working
-FIX: Instant Iinterval Vote bugged out the game
-FIX: Revive and give Money to others not working on yourself anymore
-FIX: Essential Shop Players Menu should now not show 1 Bot only Players
-FIX: Buying health will now add +100 to max health and not current health
-FIX: Joining after Round 1 should trigger respawnmonitor (This fixxes the problem that you dont respawn when joining while intermission time is running)
-FIX: Round Respawn while whole intervall and not just on round end (moved the function form level to a self monitor)
 FIX: Bossround in higher rounds now end how they should and not stop the game (Had sth to do with Max Ammo after Round)
-FIX: When dead rebuy same weapon doenst work
-FIX: Bug where the Drone in Bossround is gone when self revive used
-FIX: Boss max ammo
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
