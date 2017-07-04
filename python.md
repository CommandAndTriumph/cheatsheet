## Function Definition using the `def` keyword 

```
def increment(y):
        return y + 1
```

Or, using a lambda:

```
increment = lambda y: y + 1
```

Both can be called the same way:

```
>>> def increment(x):
...   return x + 1
... 
>>> increment(100)
101
```

```
>>> increment = lambda x: x + 1
>>> increment(100)
101

```

## Positional Arguments vs Keyword Arguments 

Define a simple function:
```
>>> def say(name, what):
...   print(f"{what} {name}")
... 
```

Using positional arguments:
```
>>> say("Bob", "Goodbye")
Goodbye Bob
```

Using keyword arguments:
```
>>> say(what="Goodbye", name="Bob")
Goodbye Bob
```

You can mix positional and keyword arguments:
```
>>> say("Bob", what = "Goodbye")
Goodbye Bob
```
