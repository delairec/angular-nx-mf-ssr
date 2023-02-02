# AngularNxMfSsr

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
