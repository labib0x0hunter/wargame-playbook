# Level - 2
---

**Goal**
- username `bandit2`
- password is stored in a file called `–spaces in this filename–` located in the `home` directory

---
**CMD Usage**
- ssh
- ls
- cat

---
**Exploit**
- Connecting
```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- Read pass
```bash
cat -- --spaces\ in\ this\ filename--
```