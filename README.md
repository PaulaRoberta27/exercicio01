# exercicio01
echo 01 > arquivo.txt
git add arquivo.txt
git status
git commit -m "git add example - arquivo.txt"
echo 02 > arquivo.txt
git diff
git add arquivo.txt
git status
git diff --staged
