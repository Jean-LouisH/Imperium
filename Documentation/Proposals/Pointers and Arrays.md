# Pointers and Arrays

Pointers and arrays are mostly be the same as in C and C++. However, in Imperium, they are strictly defined as types. As such, on variable pointer declaration, the pointer can be represented either with `*` or the unspecifically sized array `[]` on the declared type only. The `[]` brackets are used to communicate that the variables are intended to be arrays.

```cpp
float32[] values := alloc(float32[500])
```

and

```cpp
float32* value := alloc(float32)
```

Pointers can be dereferenced like in C based languages by

```cpp
nat* number := alloc(nat)
*number = 5
```

An array with a statically specified size is declared with the `[]` by the data type. Elements are accessed from 0 to the maximum number - 1 from the variable name. The separation between the declaration's brackets and the dereferencing bracket is meant to prevent confusion to beginners.

```cpp
void example()
	int[15] numbers
	numbers[0] := 4
	int a = numbers[0] + numbers[14]
```

