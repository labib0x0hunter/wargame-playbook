# Level - 12

**Goal**
- username `bandit12`
- password  is stored in the file `data.txt`, which is a `hexdump of a file` that has been repeatedly `compressed`.

---
**CMD Usage**
- ssh
- ls
- cp
- xxd
- mv
- file
- tar
- gzip
- bzip2
- cat

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
- Make temp folder 
```bash
mktemp -d
```
- Copy file to the temp file
```bash
cp data.txt /tmp/tmp.lNIxQicMYc
```

- Read the file && `1f8b` is for gzip files , decode
```bash
cat data.txt
```
- hex to bin
```bash
xxd -r data.txt data.gz
```
- decode
```bash
gzip -d data.gz
file data
mv data data.bz2

bzip2 -d data.bz2
file data
mv data data.gz

gzip -d data.gz
file data
mv data data.tar

tar -xf data.tar
file data5.bin

tar -xf data5.bin
file data6.bin
mv data6.bin data.bz2

bzip2 -d data.bz2
file data
mv data data.tar

tar -xf data.tar
file data8.bin
mv data8.bin data.gz

gzip -d data.gz
file data
```
- Read pass
```bash
cat data.txt
```