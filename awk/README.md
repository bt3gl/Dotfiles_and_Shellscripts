## awk

<br>


### data manipulation

<br>

* print elements in the column 3 that has the word "good" in the other columns

```
$ awk '/good/ { print $3 }' inventory
```

* syntax:

```
$ awk -f {PROGRAM FILE} FILENAME
```

* awk program is:

```
PATTERN{
  ACTION 1
  ACTION 2
  ACTION 3
}
```

with

```
. (Dot) Match any character
* Match zero or more character
^ Match beginning of line
$ Match end of line
\ Escape character following
[ ] List
{ } Match range of instance
+ Match one more preceding
? Match zero or one preceding
| Separate choices to match
```

<br>

---

### if condition

<br>

```
if (condition)
{
  Statement 1
  Statement 2
  Statement N
  if condition  is TRUE
}
else
{
  Statement 1
  Statement 2
  Statement N
  if condition is FALSE
}
```

