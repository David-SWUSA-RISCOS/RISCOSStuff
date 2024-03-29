# Language and Implementation Benchmarks

There are a number of benchmarking areas that help in learning how to better write code, and how to choose the best programming language.

Some of these are samples of speed, some of saving memory, and more.

## Sieve of Eratosthenes

This is one that is often wasteful in memory.  Often people implement it to use an entire integer for each flag of composite vs prime, this only takes a single bit to represent, thus each 32-bit integer can hold 32 flags.

Think about how to index a flag in BASIC (similar in Assembly or other languages). to access the flag number idx% in the array flag%()  putting the result in q% you:

```
q% = flag%(idx% >> 5) AND (1 << (idx% AND &1F))
```

Then q% is non-zero if the flag is set and 0 otherwise, making it useful in a conditional directly (0 is FALSE in BASIC and any non-zero value is True).

If you need to have the return value be either 1 or 0 for some operation then you can instead use:
```
tmp% = idx% AND &1F
q% = (flag%(idx% >> 5) AND (1 << tmp%)) >> tmp%
```

To set the flag at idx% to true using the same flag%() array you would:

```
tmp% = idx% >> 5
flag%(tmp%) = flags(tmp%) OR (1 << (idx% AND &1F))
```

Then to clear a bit flag at idx% (which we do in our sieve) you:
```
tmp% = idx% >> 5
flag%(tmp%) = flag%(tmp%) EOR (1 << (idx% AND &1F))
```

It is pretty simple.  The difference in speed is very little, and it saves a lot of RAM.  Your flags array is one thirtysecond of what it would be using a full integer for each flag.
