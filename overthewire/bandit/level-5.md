# Level - 5
---

**Goal**
- username `bandit5`
- password  is stored in a file somewhere under the `inhere` directory and has all of the following properties:

    human-readable
    1033 bytes in size
    not executable

---
**CMD Usage**
- ssh
- ls
- find
- grep
- cat

---
**Exploit**
- Connecting
```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- check for human-readable file && find the one with read permission and 1033 in size
```bash
find inhere -readable -size -2000c -perm /040 -exec ls -l "{}" \; | grep '1033'
```
- Read pass
```bash
cat inhere/maybehere07/.file2
```