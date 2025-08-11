# Level - 10
---

**Goal**
- username `bandit10`
- password  is stored in the file `data.txt`, which contains `base64 encoded data`.

---
**CMD Usage**
- ssh
- ls
- file
- cat
- base64

---
**Exploit**
- Connecting
```bash
ssh bandit10@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- check file type
```bash
file data.txt
```
- Read pass
```bash
cat data.txt | base64 -d
```