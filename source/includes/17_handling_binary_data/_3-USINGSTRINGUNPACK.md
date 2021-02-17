## Using string.unpack

STRING.UNPACK can be found in the string library. It returns values read from the binary data string. The first result is the position at which the unpack stopped. This can be used as init value for subsequent calls. The first result is followed by values defined by the format string. Numerical values in the format string are interpreted as repetitions like in pack, except if used with the A operator, in which cases the number tells unpack how many bytes to read. Unpack stops if either the format string or the binary data string are exhausted. 

The following example uses string.unpack to take a hexadecimal value and create a hexadecimal output:

Input:

`foo =   "\022\001\002\003\004"`

`pos, mybyte, mylong = string.unpack(foo, "b>l")`

`print("mybyte = " .. mybyte .. " mydword = " .. mylong)`

Output:

`mybyte = 22 mydword = 16909060`


