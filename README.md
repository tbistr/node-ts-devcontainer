# node-ts-devcontainer

## Init project

```bash
yarn init
yarn add -D typescript
yarn tsc --init --rootDir src --outDir dist
yarn add express
yarn add -D @types/node @types/express nodemon ts-node

mkdir src
touch src/index.ts src/handlers.ts
```

## Add scripts

```json
"scripts": {
    "dev": "nodemon --watch 'src/**/*.ts' --exec 'ts-node' src/index.ts",
    "start": "node dist/index.ts",
    "build": "tsc"
}
```
