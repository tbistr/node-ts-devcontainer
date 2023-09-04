# node-ts-devcontainer

## Init project

```bash
rm package.json
yarn init
yarn add -D typescript nodemon ts-node @types/node eslint prettier
yarn add -D @typescript-eslint/parser @typescript-eslint/eslint-plugin eslint-config-prettier
```

## Add scripts

```json
"scripts": {
    "dev": "nodemon --watch 'src/**/*.ts' --exec 'ts-node' src/index.ts",
    "build": "tsc",
    "start": "node dist/index.ts",
    "lint": "eslint src --ext .ts",
    "lint:fix": "eslint src --fix --ext .ts",
    "format": "prettier src/**/*.ts",
    "format:fix": "prettier src/**/*.ts --write"
}
```

## Run sample

```bash
yarn add express @types/express
yarn dev
```
