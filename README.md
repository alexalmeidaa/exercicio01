# exercicio01


### Config. inicial

```
@alexalmeidaa ➜ /workspaces/codespaces-blank $ git config --global user.name "xxxxxxxx"      
@alexalmeidaa ➜ /workspaces/codespaces-blank $ git config --global user.email "xxxxxxxx@xxx.com"     
@alexalmeidaa ➜ /workspaces/codespaces-blank $ mkdir exercicio01      
@alexalmeidaa ➜ /workspaces/codespaces-blank $ cd exercicio01/     
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 $ git init     
Initialized empty Git repository in /workspaces/codespaces-blank/exercicio01/.git/    
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cd .git/     
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01/.git (main) $ ls -a    
.  ..  HEAD  branches  config  description  hooks  info  objects  refs     
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01/.git (main) $ git status     
```

### a) 
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 01 > arquivo.txt
```
### b)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add .
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt
```

### c)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add example -arquivo.txt"
[main (root-commit) bb165f8] git add example -arquivo.txt
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo.txt
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
nothing to commit, working tree clean

@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git log
commit bb165f81d7351ee12bc1077d260e090a049dca25 (HEAD -> main)
Author: xxxxxxxx <xxxxxxxx@xxx.com>
Date:   Tue Aug 6 21:34:54 2024 +0000

    git add example -arquivo.txt
```

### d)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 02 > arquivo.txt
```

### e)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02
```

### f)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add .
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt
```
### g)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
```

### h)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 03 > arquivo.txt
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
```
### i)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
```
### j)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git restore .
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
```
### k)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "novo commit"
[main 73aed88] novo commit
 1 file changed, 1 insertion(+), 1 deletion(-)
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git log
commit 73aed8815e0db29f6aac40a39fb8e3ed982388ac (HEAD -> main)
Author: xxxxxxxx <xxxxxxxx@xxx.com>
Date:   Tue Aug 6 21:48:01 2024 +0000

    novo commit

commit bb165f81d7351ee12bc1077d260e090a049dca25
Author: xxxxxxxx <xxxxxxxx@xxx.com>
Date:   Tue Aug 6 21:34:54 2024 +0000

    git add example -arquivo.txt
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
```
### l)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo > .gitignore
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ vi .gitignore
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
```
### m)
```
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo > novo.txt
@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

@alexalmeidaa ➜ /workspaces/codespaces-blank/exercicio01 (main) $
```
