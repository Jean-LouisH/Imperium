# Dynamic Memory Allocation

Given that the dynamic memory allocation scheme is built on top of C's functions (malloc, calloc, realloc and free), Imperium's keywords resemble them. The difference, however, is that, by default, clear allocation is done, but Imperium's `uninit` keyword (for "uninitialized") can be used to allocate memory as malloc does. The keywords resemble C's allocation functions, but the type checking, and return types are more similar to C++'s use of new and delete.

`alloc`, `realloc`, `free`

```cpp
void example()

	//calloc() equivalent
	nat[] array1 = alloc(nat[5])
	
	//realloc() equivalent
	nat[] array1 = realloc(array1, nat[10])
	
	//malloc() equivalent
	nat[] array2 = alloc(uninit nat[5])
	
	//free() equivalent
	free(array1)
	free(array2)
```