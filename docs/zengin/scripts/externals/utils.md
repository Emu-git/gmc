# Utility functions
Utility functions are used for data types operations, such as type conversion.

## `IntToFloat`
!!! function "`IntToFloat`"
	Converts an integer to a float
	```dae
	func float IntToFloat(var int x)  {};
	```

	**Parameters**   

	- `#!dae var int x` - number to convert

	**Return value**  
	The function returns converted float

## `IntToString`
!!! function "`IntToString`"
	Converts an int to a string
	```dae
	func string IntToString(var int x)  {};
	```

	**Parameters**  

	- `#!dae var int x` - number to convert

	**Return value**  
	The function returns converted string

## `FloatToInt`
!!! function "`FloatToInt`"
	Converts a float to an int (cuts off the decimal part)
	```dae
	func int FloatToInt(var float x)  {};
	```

	**Parameters**   

	- `#!dae var float x` - float number to convert

	**Return value**  
	The function returns converted integer

## `FloatToString`
!!! function "`FloatToString`"
	Converts a float to a string with 6 decimal places
	```dae
	func string FloatToString(var float x)  {};
	```

	**Parameters**   

	- `#!dae var float x` - float number to convert

	**Return value**  
	The function returns converted string

## `ConcatStrings`
!!! function "`ConcatStrings`"
	Concatenates two strings and returns the new string
	```dae
	func string ConcatStrings(var string str1, var string str2) {};
	```

	**Parameters**   

	- `#!dae var string str1` - first string
	- `#!dae var string str2` - second string

	**Return value**  
	The function returns concatenated string


## Externals with docu comments
```dae
/// Converts an integer to a float
///
/// @param x number to convert
/// @return converted float
func float IntToFloat(var int x) {};

/// Converts an int to a string
///
/// @param x number to convert
/// @return converted string
func string IntToString(var int x) {};

/// Converts a float to an int (cuts off the decimal part)
///
/// @param x float number to convert
/// @return converted integer
func int FloatToInt(var float x) {};

/// Converts a float to a string with 6 decimal places
///
/// @param x float number to convert
/// @return converted string
func string FloatToString(var float x) {};

/// Concatenates two strings and returns the new string
/// 
/// @param str1 first string
/// @param str2 second string
/// @return concatenated string
func string ConcatStrings(var string str1, var string str2) {};
```