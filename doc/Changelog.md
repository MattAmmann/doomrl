### Changelog
##### Changes to DRL since the last full release (0.9.9.7):

Change | Description | Author | Date
-- | -- | -- | -- |
fix|Current kill streak count uses correct value, instead of the 'best kill streak' count|Tung Nguyen|1/5/2018
fix|Enemy kill count no longer leaks number of enemies in player info screen. [See commit for more details](f5e074502fe73781db99d9cf094e2604a04ba5e0).|Tung Nguyen|1/5/2018
fix|Added missing messages to Abyssal Plains and Chained Court that tell the player all monsters are dead.|Tung Nguyen|1/5/2018
add|Double-tapping the 'run' key (COMMA by default) will now run-wait.|Tung Nguyen|1/5/2018
fix|Reloading now uses the bottom-most ammo stack, when all stacks are of equal size.|Tung Nguyen|1/5/2018
mod|Messages for items/enemies-in-view commands are now more condensed.|Tung Nguyen|1/5/2018
mod|Targeting range is now only limited for MF_EXACT weapons.|Tung Nguyen|1/5/2018
add|Pressing TAB in an empty equip slot now acts like ENTER.|Tung Nguyen|1/4/2018
add|Selecting ground/inventory ammo now reloads wielded weapon. Allows for reloading weapons without unequipping ammo boxes.|Tung Nguyen|1/4/2018
fix|Actual key is now displayed instead of "Enter" in "Press <Enter>" prompt|Tung Nguyen|1/4/2018
mod|Show target over player when in targeting mode (ASCII only)|Tung Nguyen|1/4/2018
mod|Remember last target positions outside field of view|Tung Nguyen|1/4/2018
mod|Skip RunDelay when run-waiting in ASCII mode|Tung Nguyen|1/4/2018
mod|Added some enhanced terrain chars for high ASCII|Tung Nguyen|1/4/2018
mod|New config option created: 'AnimationSpeed'. Controls the duration of animations in tiles mode. 100 = normal speed, 0 = instant.|Tung Nguyen|1/3/2018
mod|Condensed consecutive mouse move events to greatly speed up mouse aiming|Tung Nguyen|1/3/2018
mod|All user data separated from game data and moved to its own folder, \/bin\/userdata. High quality sound and music are now the default configs.|Matt Ammann|12/31/2017
code|Repository re-organized. Many files were moved out of \/bin and into appropriate folders.|Matt Ammann|12/30/2017 
fix|Fixed the menu sound playing when Exit is selected from the main menu. The game terminating was cutting off the sound.|Matt Ammann|12/30/2017
mod|All assemblies are now moddable when the player takes the Whizkid 2 trait, regardless of when the assemblies were created. Assemblies can only be modded once, as in vanilla DRL.|Matt Ammann|12/25/2017
doc|Added detailed compiling instructions, a table-formatted changelog, and updated readme.|Matt Ammann|12/25/2017
fix|Fixed bug that crashes game if player won or died after loading old game.|VedVid|4/11/2017
add|Description for badges and medals in mortem.txt|DRL Dev Team|12/6/2016
add|Event added: darkness|DRL Dev Team|12/6/2016
mod|Animation engine upgrade|DRL Dev Team|12/6/2016
mod|Targeting ranges use vision calculation and are locked to vision range unless the weapon specifies a different range (shark).|DRL Dev Team|12/6/2016
mod|Character screen (@) shows dodge and knockback modifiers.|DRL Dev Team|12/6/2016
mod|Ao100 / AAo666 full wins now counted as such.|DRL Dev Team|12/6/2016
mod|AoOC retooled. Starting inventory changed.|DRL Dev Team|12/6/2016
fix|Melee kills tracked properly. AoLT and ArchAoLT now working as intended.|DRL Dev Team|12/6/2016
fix|Kills are only assigned to an item if the item was used to kill.|DRL Dev Team|12/6/2016
fix|Weapon OnKill is called only if weapon is used to kill the enemy.|DRL Dev Team|12/6/2016
fix|Plural items (boots) are now properly described on floor.|DRL Dev Team|12/6/2016
fix|Fixed mouse scrolling along map edges (shark).|DRL Dev Team|12/6/2016
fix|Right click won't try to reload weapons that don't use ammo (shark).|DRL Dev Team|12/6/2016
fix|Mouse targeting now respects missile range property and vision range (shark).|DRL Dev Team|12/6/2016
fix|Targeting line has consistent coloring rules between console and graphics mode.|DRL Dev Team|12/6/2016
fix|SegFault from melee attacking during weapon restricted challenges fixed (shark)|DRL Dev Team|12/6/2016
fix|Better timed-explosion animations for weapons firing multiple shots (shark)|DRL Dev Team|12/6/2016
fix|Pump action weapons that self charge or don't use ammo will allow 'r' to pump them (shark).|DRL Dev Team|12/6/2016
fix|Shottyman no longer move-reloads self charging weapons (shark).|DRL Dev Team|12/6/2016
fix|BFG10K has better scattering, and scatters at close range (shark).|DRL Dev Team|12/6/2016
fix|Fixed a crash caused by a weird interaction between the player's death, a nuke, and being OnAction hooks (shark).|DRL Dev Team|12/6/2016
fix|'l'ooking no longer overwrites the last line of the message log (shark).|DRL Dev Team|12/6/2016
fix|Repeat level feeling command added (Shift-L by default) (shark).|DRL Dev Team|12/6/2016
fix|Hell's Armory/Deimos Lab can now generate a unique as its special item.|DRL Dev Team|12/6/2016
fix|Armory/Deimos Lab won't pick assemblies created in the current game as a schematic choice.|DRL Dev Team|12/6/2016
fix|MMB now properly performs both attacks always. (shark)|DRL Dev Team|12/6/2016
fix|Demons shouldn't freeze up any more.|DRL Dev Team|12/6/2016
fix|Vaults: Opened spaces no longer marked permanent.|DRL Dev Team|12/6/2016
fix|Deimos Lab: Schematic generation matches Armory rules.|DRL Dev Team|12/6/2016
fix|Military Base: Workaround created for graphics issues.|DRL Dev Team|12/6/2016
fix|Arch-Viles now take damage from acid/lava.|DRL Dev Team|12/6/2016
fix|Berserker trigger is based on Nominal HP (Iro/Marine will no longer affect it), still has minimum of 10 damage (for AoHu).|DRL Dev Team|12/6/2016
fix|AoOC now counts sacrifice and full wins properly.|DRL Dev Team|12/6/2016
fix|Technicians now get starting tech mod on challenges that were incorrectly removing it.|DRL Dev Team|12/6/2016
code|"res\_" properties removed. Use new resist table to access resistances. (e.g. resist.bullet)|DRL Dev Team|12/6/2016
code|New prototype syntax for resistances -- resist = { resistance = value, ... }|DRL Dev Team|12/6/2016
code|level:explosion and being:apply_damage takes source item as parameter|DRL Dev Team|12/6/2016
code|kills.get and get_type only operate on string IDs|DRL Dev Team|12/6/2016
code|kills tracks 'melee' and 'other' separately|DRL Dev Team|12/6/2016
code|Expanded kills object in Lua|DRL Dev Team|12/6/2016
code|Shotgun range is now maxrange. Range has new functionality.|DRL Dev Team|12/6/2016
code|Missile/Shotgun range field determines targeting distance. maxrange limits missile distance.|DRL Dev Team|12/6/2016
code|Changed default maxrange in template to 30 to maintain existing behavior with existing missiles.|DRL Dev Team|12/6/2016
code|IF_SCATTER now works properly without MF_EXACT.|DRL Dev Team|12/6/2016
code|IF_HALFKNOCK now works with ranged weapons.|DRL Dev Team|12/6/2016
code|statistics.get_date added: returns the current system date/time in a table. Fields are year, month, day, dayofweek, hour, minute, second, and millisecond.|DRL Dev Team|12/6/2016
code|level.feeling property added. Level feeling automatically clears at level start.|DRL Dev Team|12/6/2016
code|ui.msg_feel function added. msg_feel(msg) prints msg and adds it to the level feeling.|DRL Dev Team|12/6/2016
code|ui.repeat_feel function added. repeat_feel() prints the stored level feeling. (This is the function assigned to the SHIFT-L binding).|DRL Dev Team|12/6/2016
code|ui.clear_feel function added. clear_feel() clears out the stored level feeling.|DRL Dev Team|12/6/2016
code|New item blueprint field and property 'rechargelimit' created that indicates where nano regeneration/natural regeneration stops. 0 = no limit (which is also the default).|DRL Dev Team|12/6/2016
