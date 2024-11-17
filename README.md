# Simple-UUID
Simple UUID library for minecraft

This project is a modified version of the original project created by [Gibbsly](https://github.com/gibbsly).


## Usage
### Convert UUID into hex UUID

```mcfunction
function su:convert {UUID:[I;-586860320,-833010336,-1878233485,2119000659]}
data get storage su:main out
```
```
Result: dd0538e0-ce59-4560-900c-6e737e4d6253
```

### Convert Player UUID into hex UUID 

```mcfunction
execute as @p run function su:convert with entity @s
data get storage su:main out
```

### Convert hex UUID into UUID

```mcfunction
function su:convert {hex:"dd0538e0-ce59-4560-900c-6e737e4d6253"}
data get storage su:main out
```
```
Result: [I;-586860320,-833010336,-1878233485,2119000659]
```
