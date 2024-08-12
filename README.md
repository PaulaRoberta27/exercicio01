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
