A - echo 01 > arquivo.txt

B - git status
output : On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        arquivo.txt

C - git add arquivo.txt
git status
On branch main
Your branch is up to date with 'origin/main'.      

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   arquivo.txt

D - echo 02 > arquivo.txt

E - git diff
diff --git a/arquivo.txt b/arquivo.txt
new file mode 100644
index 0000000..d789aa4
Binary files /dev/null and b/arquivo.txt differ

F - git add arquivo.txt

G - git diff arquivo.txt
output : <<nenhum>>

H - echo 03 > arquivo.txt

I - git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 420e05c..dd4c28d 100644
Binary files a/arquivo.txt and b/arquivo.txt differ

J - git restore arquivo.txt

K - git commit -m "commit aquivo.txt"
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 arquivo.txt

L - echo *.txt > .gitignore

M - git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean


