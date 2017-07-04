# Cheatsheet

## Run flask app

`FLASK_APP=path/to/app.py FLASK_DEBUG=1 flask run`

## Python vs. JSON

```
Python  JSON     JSON Representation   Difference
======  ====     ===================   ==========
dict    object   {} 
list    array    []
str     string   ""                    JSON strings must use double-quotes
int     number   1
float   number   1.0                   JSON has one type for both float and int: number
tuple   -        -                     JSON does not have tuple. Use array instead: ["apple", 1]
bool    boolean  true/false            JSON booleans are lowercase
None    null     null                  JSON has `null` instead of `None`
set     -        -                     JSON has no set. Use array instead: [1, 2, 3]


Expression    Valid Python?  Valid JSON?  Why? (if no)
==========    =============  ===========  ============
[{}, {}]      Y              Y
a             Y*             N            In python, this would be an expression for the var `a`
'123'         Y              N
False         Y              N            JSON booleans must be lowercase
true          Y*             Y            Python bools must be capitalized (but could have var `true`)
1+1           Y              N            JSON does not have operators; cannot represent/do computations
{a: 0}        Y              N            JSON objects must have double-quoted keys
{"k": False}  Y              N            `False` should be lowercase for JSON
{false: 1}    Y*             N            JSON object keys must be strings
{"": ""}      Y              Y           
[123,]        Y              N            JSON does not allow trailing commas
{4, 5}        Y              N            JSON does not have sets
```
