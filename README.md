# learnGit
repo for practicing git

## Practice number 1
### Setup
Create this tree:
```
        C - D - E
      /
A - B - F
```
### Task
Create this tree:
```
            C - D - E
          /
A - B - F
```

## Practice number 2
## Setup
Create this tree:
```
                      G - H
                     / 
            C - D - E
          /
A - B - F - I - J
```
## Task
Create this tree:
```
            C - D - E
          /
A - B - F - I - J
              \
              	G - H
```
### Answer
On any branch, run `git rebase --onto master C-D-E G-H`



## Practice number 3
### Setup
Create this tree:
```
            C - D - E
          /
A - B - F - I - J
              \
              	G - H
```
### Task
Create this tree:
```
            CDE - K
          /
A - B - F - I - J
              \
              	G - H
```
### Answer
On branch `C-D-E`, run `git rebase -i HEAD~3` and use the interactive editor to squash the commits. Add commit `K`.


## Practice number 4
### Setup
Create this tree:
```
            CDE - K
          /
A - B - F - I - J
              \
              	G - H
```
### Task
Create this tree:
```

A - B - F - I - J - G - H - L - CDE - K - M

```


