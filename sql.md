# SQL

# Primary Key

Suppose we have a table `Person` with primary key (`first_name`, `last_name`).

```
Person:
first_name last_name age
========== ========= ===
steve      mitchell  27
alan       campbell  28
bart       allen     29
alan       mitchell  27 -- OK. There's already a person with last name "mitchell", but they have a different first name
steve      mitchell  11 -- ERROR! There's already a "steve mitchell"
```
