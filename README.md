# typescript-mono-repo-template

[![Open in Github](https://img.shields.io/badge/Open_in_GitHub-6e5494)](https://github.com/JamesRobertHugginsNgo/typescript-mono-repo-template)
[![Open in Github Page](https://img.shields.io/badge/Open_in_GitHub%20Page-4078c0)](https://jamesroberthugginsngo.github.io/typescript-mono-repo-template)
[![Open Tag](https://img.shields.io/badge/Open_Tag-1.0.1-6cc644)](https://github.com/JamesRobertHugginsNgo/typescript-mono-repo-template/tree/1.0.1)

A project template for building monorepos with TypeScript.

# Usage

Follow these instructions to clone this template and start a new project with a clean Git history.

### 1. Clone and Checkout the Template

Clone the repository and replace __YOUR_PROJECT_NAME__ with your desired project name. Then, navigate into the directory and check out the latest stable tag to ensure you have a clean starting point.

```
# Clone the template
git clone https://github.com/JamesRobertHugginsNgo/typescript-mono-repo-template.git YOUR_PROJECT_NAME

# Navigate into your new project's folder
cd YOUR_PROJECT_NAME

# Checkout the stable tag
git checkout 1.0.1
```

### 2. Prepare the Project

Remove the template's Git history and reset the package.json file to begin your new project.

```
# Remove the old Git repository
# Choose the command based on your operating system:

# MacOS/Linux
rm -rf .git
rm package.json package-lock.json

# Windows
rmdir /s /q .git
del package.json package-lock.json
```

### 3. Reconfigure Your Project

Run these commands to generate a new `package.json` file and reinstall the core dependencies for your new project.

```
# Run these commands for all operating systems:
npm init -y
npm install --save-dev @types/node typescript
npm pkg set license="MIT"
npm pkg set scripts.build="tsc --build"
npm pkg set scripts.watch="tsc --watch"
npm pkg set type="module"
```
