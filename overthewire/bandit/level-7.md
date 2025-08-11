# Level - 7
---

**Goal**
- username `bandit7`
- password  is stored in the file `data.txt` next to the word `millionth`


---
**CMD Usage**
- ssh
- ls
- grep
- cat

---
**Exploit**
- Connecting
```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- Read pass
```bash
cat data.txt | grep millionth
```