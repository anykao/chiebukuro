### node

```bash
yarn add -D typescript
yarn add -D @types/node
```

- tsconfig.json
```js
{
  "compilerOptions": {
    "module": "commonjs",
    // "esModuleInterop": true,
    "target": "es6",
    "noImplicitAny": true,
    "moduleResolution": "node",
    "sourceMap": true,
    "outDir": "dist",
    "baseUrl": ".",
    "paths": {
      "*": ["node_modules/*", "src/types/*"]
    }
  },
  "include": ["src/**/*"]
}
```
