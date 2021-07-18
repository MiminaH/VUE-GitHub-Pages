# Serve Vue on GitHub Pages

### 1) Create a new VUE project
```
vue create project-name
```

### 2) Create vue.config.js file and set publicPath: '' 

### 3) Init new git repo (cd to vue project folder) & link it with remote repo (on GitHub)
```
git int
git remote add origin https://github.com/MiminaH/VUE-GitHub-Pages.git
```

### 4) Rename local branch 'main' (instead of 'master') & push it to remote
```
git branch -M main
git push -u origin main
```

### 5) Build Project
```
npm run build
```

### 6) Cd to dist folder
```
cd dist
```

### 7) Create new git repo in dist
```
git init
```

### 8) Create new local & in GitHub create a remote branch (same name)
```
git checkout -b gh-pages
```

### 9) Stage all files & commit locally (new repo in dist)
```
git add .
git commit -m "commit message"
```

### 10) Link (new dist) repo to remote repo
```
git remote add origin https://github.com/MiminaH/VUE-GitHub-Pages.git
```

### 11) Push local dist repo branch (gh-pages) to remote branch (branch-source for github pages)
```
git push -f origin gh-pages
```