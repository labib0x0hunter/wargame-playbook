# Level - 1
---

**Goal**
- username `bandit1`
- password is stored in a file called `-` located in the `home` directory

---
**CMD Usage**
- ssh
- ls
- mkdir
- cp
- cat

---
**Exploit**
- Connecting
```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```
- list directory
```bash
ls -la
```
- Create a personal folder in `/tmp` directory and copy the `-` file content to that directory.
```bash
mkdir /tmp/9xzer0_playground
cp - /tmp/9xzer0_playground/level1.txt
```
- Read pass
```bash
cat /tmp/9xzer0_playground/level1.txt
```