# AngularNxMfSsr

## About
Reproduction of the issue https://github.com/nrwl/nx/issues/14428

Start the server with `npx nx serve-ssr dashboard`

You should see this error immediately after the build :
```
path/to/your/workspace/angular-nx-mf-ssr/dist/apps/login/server/main.js:549
/******/                                if(typeof factory !== "function") throw new Error("Shared module is not available for eager consumption: " + id);
                                                                          ^

Error: Shared module is not available for eager consumption: 3473
    at __webpack_require__.m.<computed> (C:\projects\angular-nx-mf-ssr\dist\apps\login\server\main.js:549:54)
    at __webpack_require__ (C:\projects\angular-nx-mf-ssr\dist\apps\login\server\main.js:228:42)
    at 4544 (C:\projects\angular-nx-mf-ssr\dist\apps\login\server\main.js:16:82)
    at __webpack_require__ (C:\projects\angular-nx-mf-ssr\dist\apps\login\server\main.js:228:42)
    at C:\projects\angular-nx-mf-ssr\dist\apps\login\server\main.js:844:37
    at Object.<anonymous> (C:\projects\angular-nx-mf-ssr\dist\apps\login\server\main.js:849:12)
    at Module._compile (node:internal/modules/cjs/loader:1159:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1213:10)
    at Module.load (node:internal/modules/cjs/loader:1037:32)
    at Module._load (node:internal/modules/cjs/loader:878:12)

```

## Nx Report
```
 >  NX   Report complete - copy this into the issue template

   Node : 18.13.0
   OS   : win32 x64
   npm  : 9.2.0

   nx : 15.6.0
   @nrwl/angular : 15.6.3
   @nrwl/cypress : 15.6.0
   @nrwl/detox : Not Found
   @nrwl/devkit : 15.6.3
   @nrwl/esbuild : Not Found
   @nrwl/eslint-plugin-nx : 15.6.0
   @nrwl/expo : Not Found
   @nrwl/express : Not Found
   @nrwl/jest : 15.6.0
   @nrwl/js : 15.6.3
   @nrwl/linter : 15.6.0
   @nrwl/nest : Not Found
   @nrwl/next : Not Found
   @nrwl/node : Not Found
   @nrwl/nx-cloud : Not Found
   @nrwl/nx-plugin : Not Found
   @nrwl/react : Not Found
   @nrwl/react-native : Not Found
   @nrwl/rollup : Not Found
   @nrwl/schematics : Not Found
   @nrwl/storybook : Not Found
   @nrwl/web : Not Found
   @nrwl/webpack : 15.6.3
   @nrwl/workspace : 15.6.0
   @nrwl/vite : Not Found
   typescript : 4.8.4
   ---------------------------------------
   Local workspace plugins:
   ---------------------------------------
   Community plugins:
         @nguniversal/express-engine: 15.1.0
         @nguniversal/builders: 15.1.0

```
