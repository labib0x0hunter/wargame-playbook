# Level - 8
---

**Goal**
- username `bandit8`
- password  is stored in the file `data.txt` and is the only line of text that occurs only once


---
**CMD Usage**
- ssh
- ls
- sort
- uniq

---
**Exploit**
- Connecting
```bash
ssh bandit8@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- sort & count freq, Read pass
```bash
sort data.txt | uniq -u
```