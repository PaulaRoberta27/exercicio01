@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ echo 01 > arquivo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git add arquivo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   arquivo.txt

@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git commit -m "git add example - arquivo.txt"
[main f89b271] git add example - arquivo.txt
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ echo 02 > arquivo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git add arquivo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git diff --staged
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ echo 03 > arquivo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git restore --staged arquivo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git add arquivo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git commit -m "Updated arquivo.txt to 03"
[main 4b0fb0e] Updated arquivo.txt to 03
 1 file changed, 1 insertion(+), 1 deletion(-)
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git log --oneline
4b0fb0e (HEAD -> main) Updated arquivo.txt to 03
f89b271 git add example - arquivo.txt
59d7bd2 (origin/main, origin/HEAD) Update README.md
e205f14 Update README.md
7a20787 Update README.md
389efc5 Update README.md
302904f Initial commit
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ echo "*.txt" > .gitignore
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git add .gitignore
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git commit -m "Add .gitignore to ignore .txt files"
[main 1e835ea] Add .gitignore to ignore .txt files
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ echo "conteúdo do novo arquivo" > novo.txt
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
@PaulaRoberta27 ➜ /workspaces/exercicio01 (main) $ 

![image](https://github.com/user-attachments/assets/edd2dbd4-c396-40c4-9103-3b091a8fbf54)

![image](https://github.com/user-attachments/assets/1b593bd1-1a6e-44e3-bd62-cd20c2bffc52)

![image](https://github.com/user-attachments/assets/88fe6915-46f1-49da-b281-5dc505243776)

![image](https://github.com/user-attachments/assets/9ab925ce-92d0-4e7d-9b28-c4ae42e0620c)

![image](https://github.com/user-attachments/assets/760887dc-9785-44d8-b15b-834fbafa05e3)

![image](https://github.com/user-attachments/assets/71578a23-829e-4377-bbfa-3ad6c950bdcc)

![image](https://github.com/user-attachments/assets/e057e31b-6452-40db-82a8-251c894ea5f3)







