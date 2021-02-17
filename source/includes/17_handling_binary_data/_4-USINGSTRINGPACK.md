## Using string.pack

STRING.PACK can be found in the string library. It packs given arguments into binary string according to format. The format string describes how the parameters (p1, ...) will be interpreted. Numerical values following the operators are standard for operator repetitions and need an according amount of parameters. Operators also expect appropriate parameter types. 

The following example uses string.pack to take a decimal input and create a hexadecimal output:

Input:

`mybyte = 22`

`mylong = 16909060`

`msg = string.pack("b>l", mybyte, mylong)`

`hexdump(msg)`

Output:

`00000000 16 01 02 03 04`

Note the use of the big endian modifier in the example above.

