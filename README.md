# Serve Vue on GitHub Pages

### 1) Create vue.config.js file and set publicPath: '' 

### 2) Build Project
```
npm run build
```

### 3) Cd to dist folder
```
cd dist
```

### 4) Create new git repo in dist
```
git init
```

### 5) Create new local & create a remote branch (same name)
```
git checkout -b gh-pages
```

### 6) Stage all files & commit locally
```
git add .
git commit -m "commit message"
```

### 3) Link new repo to remote repo
```
git remote add origin https://github.com/MiminaH/VUE-GitHub-Pages.git
```

### 3) Push new repo to remote branch (branch-source for github pages)
```
git push -f origin gh-pages
```