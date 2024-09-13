## Steps to sucess for using this template

1. create git repo with following commands:
```
//TODO git config email username
git init
git remote add origin https://github.com/uegwq/ObsidianQuartoTemplate.git
git branch -M main
git pull origin main
git add .
git commit -m "Initial commit"
git push -u origin main
git checkout -b gh-pages
git push -u origin gh-pages 
```
2. go to `Settings>pages>Build and deployment>Branch` and set it to be *gh-pages* and the folder to `/ (root)`.

3. create contents website view with fancy program and change 
- theme
- date

4. modify the index.qmd file (title, description, possibly image)

5.  change repo url for editing and issues

7. profit