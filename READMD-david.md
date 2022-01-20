# NX workspae

```
npx create-nx-workspace nx-egghead
```

## lesson2

```
npx nx list

npm install @nrwl/react
npx nx list@nrwl/react

npx nx g @nrwl/react:application -- help
npx nx g @nrwl/react:application store --dry-run
npx nx g @nrwl/react:application store

```

## lesson 4

```
npx nx run store:serve --port=3001
```

## lesson 5

```
npm install @material-ui/core
```

## lesson 6

```
npx nx g @nrwl/react:lib ui-shared --directory=store --dry-run
npx nx g @nrwl/react:component header --project=store-ui-shared
```

## lesson 9

```
npx nx g @nrwl/workspace:lib util-formatters --directory=store --dry-run

tsconfig.base.json
    "paths": {
      "@nx-egghead/store/ui-shared": ["libs/store/ui-shared/src/index.ts"],
      "@nx-egghead/store/util-formatters": [
        "libs/store/util-formatters/src/index.ts"
      ]
```
