# bigsea_Boatanchor
Very simple and basic boats anchor script. While anchored, boat will drift back and forth in anchored place depending on location where it was anchored. If force exceeds, anchor might brake, for example if you start driving anchor will brake.
# Config
All of the configs here are set using setr [anchor:configOption] [boolean]

ConVar	Default	Description	Parameter(s)
anchor:command_enabled	true	Defines if command /anchor is enabled on resource start.	boolean
anchor:use_ace_permissions	false	Defines if command can be used only with ace permissions.	boolean
anchor:max_speed	3.0	If speed of the boat is higher than defined, player won't be able to anchor.	number
anchor:min_drift_distance	0.1	Defines minimum drift distance from anchored position before it starts to apply mass relatively to world coords.	number
anchor:breaking_force	600.0	Defines breaking force before anchor breaks.	number
# Documentation
Exports
Client
Toggles
Export	Description
ToggleAnchor	Toggles boat anchor
Getters
State Bag	Description	Parameter(s)	Return Type
CanAnchor	Returns if current boat can be anchored, vehicle need to passed.	int	boolean
IsAnchored	Return if current is currently anchored, vehicle need to passed.	int	boolean
