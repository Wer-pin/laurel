# Laruel Grammar

## Basic
--------------
***The Comment***
```
// This is one line comment
```
```
/*
    This
    is
    multiple
    comment
*/
```
***The Names***

It is not available the name (of variable, function, class, ...) that includes space, any symbols and starts with number and is not same as key word name (Keyword List Below)


*Examples*
```
name_1              //-> Available
na me               //-> Not Available (including space)
name_3#             //-> Not Available (including sysmbol)
2_name              //-> Not Available (starts with number)
class               //-> Not Available (same as keyword)
```

## Keyword
---------------
*class: make a class named "@name"*
```
class @name {
    func @name_1 {
        ...
    }
    func @name_2 {
        ...
    }
    .
    .
    .
}
```

*func: define a function that named "@name" and takes infinite arguments*
```
func @name(#args, ...) {
    ...
}
```

*for: loop while the condition is true and update it after init variable*
```
for #initialization, #condition, #update {
    ...
}
```

*break: break the loop and excute code outside of the loop*
```
for #initialization, #condition, #update {
    break
}
```

*if: if the condition is true, run code and if not true just pass it*
```
if #condition {
    ...
}
```

*elsif: located after if, check the another condition and run code as if*
```
if #condition {
    ...
}
elsif #condition {
    ...
}
```

*else: located after if or elsif, run code if the conditions above else is not true*
```
if #condition {
    ...
}
else {
    ...
}
```
/ or /
```
if #condition {
    ...
}
elsif #condition {
    ...
}
else {
    ...
}
```

*try: try the code and if it detected the error just pass it, and if not, run that code*
```
try {
    ...
}
```

*except: run when after try that did not run*
```
try {
    ...
}
except {
    ...
}
```

## Arithmetic
-------------
### ***The Order***
* **Parentheses**
* **Exponent**
* **Multiplication**
* **Remainder**
* **Floor Division**
* **Division**
* **Addition**
* **Subtraction**

*Examples*

```
1 + 2 * 3 - 4 / 2
```
```
5
```
-----------------
-----------------
```
2 ** 3 + 4 % 2 * 2
```
```
8
```
----------------
----------------
```
3 // 2 * (4 + 2) % 3
```
```
0
```
