# How to set up Vite project

## Github
- [ ] Create repo in Github
- [ ] >Git clone repo in VS code

## Install Vite and TypeScript

- [ ] Install npm in Terminal
 ```bash
  npm create vite@latest .
```
Choose Vanilla -> TypeScript
  
In terminal

```bash
  npm install
```

```bash
  npm run dev
```

## Fix gitignore
### Make sure these exist in .gitignore file
- [ ] .DS_Store
- [ ] *.css.map
- [ ] style.css

## Add vite.config.ts
```bash
  touch vite.config.ts
```
### Add this in the file 
```bash
  import { defineConfig } from 'vite';

export default defineConfig({
  'base': '/adressen-till-ert-repo-här/'
});
```
