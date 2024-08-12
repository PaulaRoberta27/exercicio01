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
echo 03 > arquivo.txt
git diff
git restore --staged arquivo.txt
git status
git add arquivo.txt
git commit -m "Updated arquivo.txt to 03"
git log --oneline
echo "*.txt" > .gitignore
git add .gitignore
git commit -m "Add .gitignore to ignore .txt files"
echo "conteúdo do novo arquivo" > novo.txt
git status

