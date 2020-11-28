# Primitive Data Types

### Void placeholder
`void`

### Booleans
`bool`, `boolarr8`, `boolarr16`, `boolarr32`, `boolarr64`, `boolarr`

### Natural numbers / Unsigned Integers
`nat8`, `nat16`, `nat32`, `nat64`, `nat`

### Integers, Signed
`int8`, `int16`, `int32`, `int64`, `int`

### Text
`ascii`, `utf8`, `utf16`

### Floating Point
`float32`, `float64`, `float`

* Data types with unspecified sizes such as `boolarr`, `nat`, `int`, and `float` are intended to be converted at compile time into the specific sizes based on the largest constants assigned to them. Otherwise, the target precision is 32-bits.

## Code example
```cpp
void example()
	bool testBoolean := false
	boolarr testBooleanArray := 0xE8
	nat testNaturalNumber := 3
	int testInteger := -40
	ascii testASCIILetter := 'Q'
	utf8 testUTF8 := '€'
	utf16 testUTF16 := '😏'
	float32 testRealValue := 3.14159
```