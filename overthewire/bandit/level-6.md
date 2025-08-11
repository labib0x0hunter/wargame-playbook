# Level - 6
---

**Goal**
- username `bandit6`
- password  is stored `somewhere on the server` and has all of the following properties:

    owned by user bandit7
    owned by group bandit6
    33 bytes in size


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
ssh bandit6@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- check for human-readable file && find the one with owner and 33 in size
```bash
find / -user bandit7 -group bandit6 -exec ls -l "{}" \;
```
- Read pass
```bash
cat /var/lib/dpkg/info/bandit7.password
```