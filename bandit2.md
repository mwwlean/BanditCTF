# Bandit Level 1 → Level 2
### Level Goal
The password for the next level is stored in a file called - located in the home directory

Commands you may need to solve this level
``` ls , cd , cat , file , du , find ```

### Command:
```
ssh -p 2220 bandit1@bandit.labs.overthewire.org
du --h
du -ah

```

then i found this 
```
bandit1@bandit:~$ du -ah
4.0K    ./.bash_logout
4.0K    ./.bashrc
4.0K    ./.profile
4.0K    ./- < --- this one
20K
```

``` 
cat ./-
```

### FLAG:

``` bash
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```
