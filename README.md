# Typescript Starter Project Template

## Install

1. **Download Node.js:** [https://nodejs.org/dist/v16.14.0/node-v16.14.0-x64.msi](https://nodejs.org/dist/v16.14.0/node-v16.14.0-x64.msi)
2. **Download Git Bash:** [https://github.com/git-for-windows/git/releases/download/v2.35.1.windows.2/Git-2.35.1.2-64-bit.exe](https://github.com/git-for-windows/git/releases/download/v2.35.1.windows.2/Git-2.35.1.2-64-bit.exe)

### Check NodeJs

```bash
node -v
```

### Clone exists template

Clone Repository

```bash
git clone https://github.com/verve-neowise/typescript-starter-project-template.git
```

or

### Create project

1. Create folder and open on vscode
2. open terminal

### Make folder as Node.js project

```bash
npm init
```

### Create project structure

1. create **src** dir
2. create **out** dir
3. create sample file (index.ts) in src folder:

src/index.ts

```bash
console.log("Hello Typescript");
```

structure

```bash
-project
|--src
	|-index.ts
|--out 
```

### **Install typescript**

```bash
npm i -g typescript
```

### Configure TS config

```bash
tsc -init
```

### **Change tsconfig.json file parameters for compilation:**

```json
{
	"compilerOptions" : {
		"rootDir": "src",
		"outDir": "out"
	}
}
```

### Run compiler on watch mode:

```bash
tsc -w
```

### Run app file:

```bash
node out/index.js
```

## Additional

### Add start script to **package.json** for simple run:

```bash
{
	...
	"scripts": {
		"start": "node out/index.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
	...
}
```

Run:

```bash
npm start
```

## Install nodemon:

```bash
npm i -g nodemon
```

Run:

```bash
nodemon out/index.js
```

# Install types

Node types
```bash
npm i @types/node
```

Install prompt-sync
```bash
npm i prompt-sync @types/prompt-sync
```
