---
title: HLP functions
---
# HLP - help functions
Helper functions, generally used for safety checks, and specific operations.

## `Hlp_GetInstanceID`
!!! function "`Hlp_GetInstanceID`"
	Returns the internal ID of an instance, useful for comparison
	```dae
	func int Hlp_GetInstanceID(var instance inst)  {};
	```

	**Parameters**  

	- `#!dae var instance inst` - any instance

	**Return value**  
	The function returns internal ID of the instance

## `Hlp_GetNpc`
!!! function "`Hlp_GetNpc`"
	Finds an NPC object by its instance name
	```dae
	func C_NPC Hlp_GetNpc(var int instancename)  {};
	```

	**Parameters**  

	- `#!dae var int instancename` - instance name of the NPC

	**Return value**  
	The function returns link to NPC object

## `Hlp_IsItem`
!!! function "`Hlp_IsItem`"
	Checks if item object is a specified instance
	```dae
	func int Hlp_IsItem(var C_ITEM itm, var int instancename)  {};
	```

	**Parameters**  
    
	- `#!dae var C_ITEM itm` - C_ITEM instance of the item
	- `#!dae var int instancename` - instance name of the item

	**Return value**  
	The function returns `TRUE` if the item is the specified instance, `FALSE` otherwise

## `Hlp_IsValidItem`
!!! function "`Hlp_IsValidItem`"
	Checks if item is in the game world
	```dae
	func int Hlp_IsValidItem(var C_ITEM itm)  {};
	```

	**Parameters**  

	- `#!dae var C_ITEM itm` - instance of the item

	**Return value**  
	The function returns `TRUE` if the item is in the game world, `FALSE` otherwise

## `Hlp_IsValidNpc`
!!! function "`Hlp_IsValidNpc`"
	Checks if the NPC exists in the game world
	```dae
	func int Hlp_IsValidNpc(var C_NPC npc)  {};
	```

	**Parameters**  

	- `#!dae var C_NPC npc` - instance of the NPC

	**Return value**  
	The function returns `TRUE` if the NPC exists, `FALSE` otherwise

## `Hlp_Random`
!!! function "`Hlp_Random`"
	Generates a random value
	```dae
	func int Hlp_Random(var int bound)  {};
	```

	**Parameters**  

	- `#!dae var int bound` - maximum value

	**Return value**  
	The function returns random value form 0 to bound

## `Hlp_StrCmp`
!!! function "`Hlp_StrCmp`"
	Compares two strings (not case-sensitive)
	```dae
	func int Hlp_StrCmp(var string s1, var string s2)  {};
	```

	**Parameters**  
    
	- `#!dae var string s1` - first string
	- `#!dae var string s2` - second string

	**Return value**  
	The function returns `TRUE` if the strings are equal, `FALSE` otherwise


## zParserExtender 
zParserExtender implements quite a few new [hlp external functions](../extenders/zparserextender/externals/hlp.md).


## Externals with docu comments
```dae
/// Returns the internal ID of an instance, useful for comparison
///
/// @param inst any instance
/// @return internal ID of the instance
func int Hlp_GetInstanceID(var instance inst) {};

/// Finds an NPC object by its instance name
///
/// @param instancename instance name of the NPC
/// @return link to NPC object
func C_NPC Hlp_GetNpc(var int instancename) {};

/// Checks if item object is a specified instance
///
/// @param itm C_ITEM instance of the item
/// @param instancename instance name of the item
/// @return TRUE if the item is the specified instance, FALSE otherwise
func int Hlp_IsItem(var C_ITEM itm, var int instancename) {};

/// Checks if item is in the game world
///
/// @param itm instance of the item
/// @return TRUE if the item is in the game world, FALSE otherwise
func int Hlp_IsValidItem(var C_ITEM itm) {};

/// Checks if the NPC exists in the game world
///
/// @param npc instance of the NPC
/// @return TRUE if the NPC exists, FALSE otherwise
func int Hlp_IsValidNpc(var C_NPC npc) {};

/// Generates a random value
///
/// @param bound maximum value
/// @return random value form 0 to bound
func int Hlp_Random(var int bound) {};

/// Compares two strings (not case-sensitive)
///
/// @param s1 first string
/// @param s2 second string
/// @return TRUE if the strings are equal, FALSE otherwise
func int Hlp_StrCmp(var string s1, var string s2) {};

/// deprecated
func int Hlp_CutscenePlayed(var string csname) {};
```