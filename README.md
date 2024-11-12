# Test create publishing package

## How

- Create npm account
- login

```sh
  npm login
```

- publish

```sh
  npm publish
```

## Test

- create link (at package folder)

```sh
  npm link
```

- link package (at test folder)

```sh
  npm link {package-name}
```

## Declare module for ts

- Create type

```sh
  npx -p typescript tsc src/**/*.js --declaration --allowJs --emitDeclarationOnly --outDir types
```

- Edit package.json

```json
types: "location of .d.ts file",
main: "location js index file"
```

- Ref: https://www.typescriptlang.org/docs/handbook/declaration-files/dts-from-js.html
