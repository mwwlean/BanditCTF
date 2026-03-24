# Bandit Level 2 → Level 3
### Level Goal

The password for the next level is stored in a file called --spaces in this filename-- located in the home directory

Commands you may need to solve this level
``` ls , cd , cat , file , du , find ```

Helpful Reading Material
Google Search for “spaces in filename”

Commands:

```
ssh -p 2220 bandit2@bandit.labs.overthewire.org
du -ah
cat ./--spaces\ in\ this\ filename--
```
```
bandit2@bandit:~$ du -ah
4.0K    ./.bash_logout
4.0K    ./.bashrc
4.0K    ./--spaces in this filename--
4.0K    ./.profile
20K     .
bandit2@bandit:~$ cat ./--spaces\ in\ this\ filename--
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
bandit2@bandit:~$
```

### Flag

```
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```