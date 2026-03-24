# Bandit Level 3 → Level 4
### Level Goal
- The password for the next level is stored in a hidden file in the inhere directory.

Commands you may need to solve this level
``` ls , cd , cat , file , du , find ```

Commands:

``` 
ssh -p 2220 bandit3@bandit.labs.overthewire.org
bandit3@bandit:~$ ls
inhere
bandit3@bandit:~$ cd inhere/
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ cat -a
cat: invalid option -- 'a'
Try 'cat --help' for more information.
bandit3@bandit:~/inhere$ du -ah
4.0K    ./...Hiding-From-You
8.0K    .
bandit3@bandit:~/inhere$ cat ./...Hiding-From-You
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
bandit3@bandit:~/inhere$
```
FLAG:

```
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```