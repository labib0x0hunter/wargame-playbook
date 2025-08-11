# Level - 3
---

**Goal**
- username `bandit3`
- password is stored in a hidden file in the `inhere` directory.

---
**CMD Usage**
- ssh
- ls
- cd
- cat

---
**Exploit**
- Connecting
```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- change directory
```bash
cd inhere &&  ls -la
```
- Read pass
```bash
cat '...Hiding-From-You'
```