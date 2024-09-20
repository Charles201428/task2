mkdir task2
cd task2
git init
echo "This is a readme file!" > README.md
git add README.md
git commit -m "Add initial README.md with basic content"
git remote add origin https://github.com/Charles201428/task2.git
git push -u origin main
echo "This is a local readme file!" > README.md
git add README.md
git commit -m "Update README.md to reflect local changes"
git push origin main
git pull origin main
git add README.md
git commit -m "Resolve merge conflict and unify README.md content"
git push origin main
git checkout -b feature1
echo "This is feature 1!" > FEATURE1.md
git add FEATURE1.md
git commit -m "Add FEATURE1.md with initial content"
git push origin feature1
git checkout main
git pull origin main
