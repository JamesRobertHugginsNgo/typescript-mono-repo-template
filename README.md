# typescript-mono-repo-template

[![Open in Github](https://img.shields.io/badge/Open_in_GitHub-6e5494)](https://github.com/JamesRobertHugginsNgo/typescript-mono-repo-template)
[![Open in Github Page](https://img.shields.io/badge/Open_in_GitHub%20Page-4078c0)](https://jamesroberthugginsngo.github.io/typescript-mono-repo-template)
[![Open Tag](https://img.shields.io/badge/Open_Tag-1.0.0-6cc644)](https://github.com/JamesRobertHugginsNgo/typescript-mono-repo-template/tree/1.0.0)

Typescript mono repo project template.

# Usage

## Clone

```
git clone https://github.com/JamesRobertHugginsNgo/typescript-mono-repo-template.git PROJECT_NAME
```

## Remove Git Folder

Before running the commands below make sure you are in the new project folder.

MacOS/Linux

```
rm -rf .git
```

Windows

```
rmdir /s /q .git
```

## Reset Package.json

Before running the commands below make sure you are in the new project folder.

For best result also update the README.md file as `npm init -y` command will take the description value from the this file.

```
rm package.json
npm init -y
npm install --save-dev @types/node typescript
npm pkg set scripts.build="tsc --build"
npm pkg set scripts.watch="tsc --watch"
npm pkg set type="module"
```
