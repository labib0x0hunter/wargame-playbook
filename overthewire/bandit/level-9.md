# Level - 9
---

**Goal**
- username `bandit9`
- password  is stored in the file `data.txt` in one of the `few human-readable strings`, preceded by several `‘=’ characters`.


---
**CMD Usage**
- ssh
- ls
- file
- strings

---
**Exploit**
- Connecting
```bash
ssh bandit9@bandit.labs.overthewire.org -p 2220
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
strings -n 6 data.txt
```