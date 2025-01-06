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
## Install EsLint
```bash
  npm init @eslint/config@latest
```
### Choose so it end up like look like this
```bash
✔ How would you like to use ESLint? · check syntax and problems
✔ What type of modules does your project use? · JavaScript modules import and export
✔ Which framework does your project use? · none of these
✔ Does your project use TypeScript? · yes typescript
✔ Where does your code run? · browser
The config that you've selected requires the following dependencies:

eslint, globals, @eslint/js, typescript-eslint
✔ Would you like to install them now? · Yes
✔ Which package manager do you want to use? · npm
```
## Install Prettier
```bash
# Install Prettier med npm 
npm install --save-dev --save-exact prettier

# Create a empty config-fil with name .prettierrc
node --eval "fs.writeFileSync('.prettierrc','{}\n')"
# Create a prettierignore-file to ignore some files
node --eval "fs.writeFileSync('.prettierignore','# Ignore artifacts:\nbuild\ncoverage\n')"

# Formate all files with npm
npx prettier . --write

# Install eslint-config-prettier to make Prettier and ESLint work together:
npm install --save-dev eslint-config-prettier

```

