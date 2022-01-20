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

## lesson 11

```
npx nx g @nrwl/react:lib feature-game-detail --directory=store --appProject=store  --dry-run
```

## lesson 12

```
npm install -D @nrwl/express
npx nx g @nrwl/express:application api --frontendProject=store --dry-run
npx nx run api:serve

http://localhost:3333/api/games
http://localhost:4200/api/games

npx nx run-many --target=serve --projects=api,store --parallel=true
```

### lesson 13

```
npx nx run store:serveAppAndApi

-- see apps/store/project.json
    "serveAppAndApi": {
      "executor": "@nrwl/workspace:run-commands",
      "options": {
        "commands": [
          {
            "command": "nx run api:serve"
          },
          {
            "command": "nx run store:serve"
          }
        ]
      }
    },
```

### lesson 14

```
npx nx dep-graph

proxy.conf.json
```

### lesson 19

```
npx nx run store:test --watch
```
