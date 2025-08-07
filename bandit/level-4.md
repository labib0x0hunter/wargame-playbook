# Level - 4
---

**Goal**
- username `bandit4`
- password is stored in the only human-readable file in the `inhere` directory.

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
ssh bandit4@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- change directory
```bash
cd inhere &&  ls -la
```
- check for human-readable file && find the one with 'ASCII text'
```bash
file -- -file00
```
- Read pass
```bash
cat -- -file00
```