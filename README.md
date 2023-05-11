# basic-example-itb-2023
This is the basic example to create a vue/vite project and integrate vitest

## Create the base project
```bash
npm create vite@latest ITB-2023 -- --template vue
```

## Install vitest
```bash
npm install -D vitest
```

## Update vite.config.js
```bash
export default defineConfig({
  plugins: [vue()],
  test : {
    globals : true,
    environment : "jsdom"
  }
});
```

## Install jsDom
```
npm install -D jsdom
```

## Install vitest/ui
```bash
npm i -D @vitest/ui
```

## Update package.json
```bash
"tests" = "vitest --ui --api 9527"
```

## Add src/tests and create this test
```bash
import { describe, it } from "vitest";

describe( "My example", () => {
   it.todo( "is my example", () => {
    //
   } );
} );
```



