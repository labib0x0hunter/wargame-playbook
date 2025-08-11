# Level - 0
---

**Goal**
- Connect to `bandit.labs.overthewire.org` on port `2220` using `ssh`.
- username `bandit0` and password `bandit0`
- password is stored in a file called `readme` located in the `home` directory

---
**CMD Usage**
- ssh
- ls
- cat

---
**Exploit**
- Connecting
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
- Read pass
```bash
ls -la
cat readme
```