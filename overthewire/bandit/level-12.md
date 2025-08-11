# Level - 12
---// UNSOLVED //

**Goal**
- username `bandit12`
- password  is stored in the file `data.txt`, where all lowercase (a-z) and uppercase (A-Z) letters have been `rotated by 13 positions`.

---
**CMD Usage**
- ssh
- ls
- cat
- tr

---
**Exploit**
- Connecting
```bash
ssh bandit12@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- Read pass
```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```