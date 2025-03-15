# LAB-4

1. **Name**: Divya Darshan Tiwari
2. **SAP**: 500105299
3. **Roll No.**: R2142220070
4. **Batch**: B1H Full Stack AI

---

## **Project Setup**

### **Created a project directory, navigated into it, created a `src` directory, and listed its contents:**

```bash
$ mkdir project
$ cd project
$ mkdir src
$ ls
```

---

## **Creating and Modifying Files**

### **Created a `README.md` file using `touch`, listed files in the directory with `ls`, checked its contents with `cat` (which was empty initially), and then added "Hello World" to it using `echo`:**

```bash
$ touch README.md
$ ls
$ cat README.md
$ echo "Hello World" >> README.md
```

---

### **Displayed the contents of `README.md` using `cat`, and experimented with `echo` to print text and add escape sequences:**

```bash
$ cat README.md
$ echo "hello \n me"
$ echo -c "hello \n me"
$ echo -e "hello \n me"
```

---

### **Overwrote the contents of `README.md` with "Hello World 1" and then added "content" to it:**

```bash
$ echo "Hello World 1" > README.md
$ echo "content" >> README.md && cat README.md
```

---

## **Git Repository Setup**

### **Initialized a new Git repository, checked remote repositories, and listed branches:**

```bash
$ git init
$ git remote -v
$ git branch
$ cd .
$ ls
```

---

### **Checked the Git status, staged all files, and committed them with a message:**

```bash
$ git status
$ git add . && git commit -m "readme.md added"
```

---

### **Renamed the default branch from `master` to `main`:**

```bash
$ git branch -M main
$ git branch
```

---

### **Added and committed more files (`a.txt` and `b.txt`) and checked the commit history:**

```bash
$ git log
```

---

### **Performed a soft reset to an earlier commit and checked the status:**

```bash
$ git reset --soft 280e2b
$ git status
```

---

### **Switched to an older commit, putting Git in a detached HEAD state:**

```bash
$ git checkout 4981f
$ git log
```

---

### **Switched back to the `main` branch, added `b.txt`, and committed it again:**

```bash
$ git checkout main
$ git add .
$ git commit -m "Added b.txt"
```

---

### **Checked the commit history after re-adding `b.txt`:**

```bash
$ git log
```

---

## **Branching and Merging**

### **Created a new branch `featureA` and switched to it:**

```bash
$ git branch featureA
$ git checkout featureA
```

---

### **Added and committed new files (`z.txt` and `x.txt`) in the `featureA` branch:**

```bash
$ touch z.txt
$ git add . && git commit -m "z file added"
$ touch x.txt
$ git add . && git commit -m "x file added"
$ git log
```

---

### **Switched back to the `main` branch and checked the logs:**

```bash
$ git checkout main
$ git log
```

---

### **Added and committed a new file (`s.txt`) in the `main` branch:**

```bash
$ touch s.txt
$ git add . && git commit -m "s file added in main"
$ git log --oneline
```

---

### **Switched back to `featureA` and checked the logs:**

```bash
$ git checkout featureA
$ git log --oneline
```

---

### **Rebased `featureA` onto `main` to include changes from `main`:**

```bash
$ git rebase main
$ git log --oneline
```

---

### **Created a new branch `featureB` as a copy of `featureA` and switched to it:**

```bash
$ git branch -c featureB
$ git checkout featureB
$ git log --oneline
```

---

### **Merged `featureB` into `main` using a fast-forward merge:**

```bash
$ git checkout main
$ git merge featureB
```

---

### **Performed a hard reset to an earlier commit:**

```bash
$ git reset --hard ffd8
$ git log --oneline
```

---

### **Performed a squash merge from `featureB` into `main`:**

```bash
$ git merge --squash featureB
$ git status
```

---

### **Committed the squashed changes and forcefully deleted the `featureA` branch:**

```bash
$ git add . && git commit -m "file added only using squash"
$ git branch -D featureA
```

---
