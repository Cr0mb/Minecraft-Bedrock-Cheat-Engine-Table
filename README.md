# Minecraft-Bedrock-Cheat-Engine-Table
This repository contains a Cheat Engine table for Minecraft (Windows version), designed to enhance the gameplay experience by allowing players to modify certain aspects of the game. The table includes several cheat entries such as health, max health, instant break, instant eating, coordinates, full bright, and XP manipulation.

![image](https://github.com/user-attachments/assets/41f35c4d-ca1d-4337-bb68-c4c98147805a)


## Features
```
> Player Health: Modify your current health.
> Max Health: Adjust your maximum health.
> Instant Break: Break blocks instantly.
> Instant Eating: Eat food instantly.
> Force Show Coordinates: Always show coordinates.
> FullBright: Enables 100% brightness, allowing you to see in dark areas.
> XP Manipulation: Modify XP.
> X_Velocity (Removes friction on the X-Axis)
> Y_Velocity (Removes friction on the Y-Axis)
> No Friction (Both X & Y Velocity Friction is removed)
> Sneak Phase
> Anti Knockback
> Speed Hack
```

## Update 2
```
> Added God Mode, (health, hunger, and no fall.)
> Removed XP_Display (doesn't change functionality)
> Added Anti Knockback
> Added Speedhack
```

## Updates
```
> Added XP_Display as well as XP_Write (one controls the actual xp value and one controls the text on the xp bar.)
> Added no friction (no operation for x and y velocity.)
> Added Sneak Phasing (noclip)
```

## Notes (FIXED)
- As of now for the XP_Write function you need to enable this first, you will notice in-game that you're xp value did not change.
- To fix this, you need to change your XP value in game. You can do this by killing a mob or enchanting something, but the value must change you can't just fill the XP bar halfway or else it won't work.
- So for example if your XP is level 1 whenever you toggle the script, your XP won't change to the desired value until you reach level 2.


## AOB Scanning

AOB (Array of Bytes) scanning is a technique used in Cheat Engine to search for specific byte patterns within the game's memory. These byte patterns are unique identifiers that point to specific functions or areas of memory within the game. By identifying these byte patterns, we can inject custom scripts or modify values at runtime.

## How AOB Scanning Works

In this table, we use AOB scanning to locate the memory addresses of specific functions or values that we want to manipulate. The process is as follows:

Scanning for Values:

- Use Cheat Engine to locate the desired in-game value (e.g., health, XP).
- Perform successive scans to narrow down the results.


Analyzing Memory Access:

- Right-click the identified address and select "Find out what accesses this address" or "Find out what writes to this address".
- Run in-game actions to trigger changes in the value and observe which instructions interact with the address.

Viewing in Disassembler:

- Select the correct instruction from the debugger and view it in the disassembler.
- You can do this by doing something in game to change the value, then see what changes in the debugger.

Auto Assembling with AOB Template:

- In the disassembler, go to Tools > Auto Assemble.
- Use the AOB injection template to generate a script.
- Modify the newmem section of the script to:
   - Set the desired value.
   - Freeze the value for consistent behavior.

# Why AOB Scanning?

- AOB scanning is critical for maintaining compatibility across game updates, as it targets unique byte patterns instead of static addresses. This approach ensures that the table can adapt to minor changes in the game's memory structure.
- This also comes in handy if you can not find any pointers within the game, sometimes you need to dereference a different way.



