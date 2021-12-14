# ion6-pwa-crashing-tabs
This repo lives to show a fresh ionic 6 vue project with vue add pwa no longer allowing ionic serve to work

running ionic serve in this folder results in the following stack trace for me:

C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs>ionic serve
> vue-cli-service.cmd serve
[9%] setup (compilation vue-cli:pwa-html-plugin)
[vue-cli-service] (node:24292) UnhandledPromiseRejectionWarning: TypeError: Cannot read property 'tapAsync' of undefined
[vue-cli-service]     at C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\@vue\cli-plugin-pwa\lib\HtmlPwaPlugin.js:62:63
[vue-cli-service]     at Hook.eval [as call] (eval at create (C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\tapable\lib\HookCodeFactory.js:19:10), <anonymous>:256:1)
[vue-cli-service]     at Hook.CALL_DELEGATE [as _call] (C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\tapable\lib\Hook.js:14:14)
[vue-cli-service]     at Compiler.newCompilation (C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\webpack\lib\Compiler.js:1055:26)
[vue-cli-service]     at C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\webpack\lib\Compiler.js:1099:29
[vue-cli-service]     at Hook.eval [as callAsync] (eval at create (C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\tapable\lib\HookCodeFactory.js:33:10), <anonymous>:40:1)
[vue-cli-service]     at Hook.CALL_ASYNC_DELEGATE [as _callAsync] (C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\tapable\lib\Hook.js:18:14)
[vue-cli-service]     at Compiler.compile (C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\webpack\lib\Compiler.js:1094:28)
[vue-cli-service]     at C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\webpack\lib\Watching.js:214:19
[vue-cli-service]     at _next0 (eval at create (C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs\node_modules\tapable\lib\HookCodeFactory.js:33:10), <anonymous>:41:1)
[vue-cli-service] (Use `node --trace-warnings ...` to show where the warning was created)
[vue-cli-service] (node:24292) UnhandledPromiseRejectionWarning: Unhandled promise rejection. This error originated either by throwing inside of an async function without a catch block, or by rejecting a promise which was not handled with .catch(). To terminate the node process on unhandled promise rejection, use the CLI flag `--unhandled-rejections=strict` (see https://nodejs.org/api/cli.html#cli_unhandled_rejections_mode). (rejection id: 1)
[vue-cli-service] (node:24292) [DEP0018] DeprecationWarning: Unhandled promise rejections are deprecated. In the future, promise rejections that are not handled will terminate the Node.js process with a non-zero exit code.

---

Ionic info:

C:\Users\Dries\Desktop\Nieuwe map\ion6-pwa-crashing-tabs>ionic info
[WARN] Error loading @capacitor/ios package.json: Error: Cannot find module '@capacitor/ios/package'

       Require stack:
       - C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli\lib\project\index.js
       - C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli\lib\index.js
       - C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli\index.js
       - C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli\bin\ionic
[WARN] Error loading @capacitor/android package.json: Error: Cannot find module '@capacitor/android/package'

       Require stack:
       - C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli\lib\project\index.js
       - C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli\lib\index.js
       - C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli\index.js
       - C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli\bin\ionic

Ionic:

   Ionic CLI       : 6.18.1 (C:\Users\Dries\AppData\Roaming\npm\node_modules\@ionic\cli)
   Ionic Framework : @ionic/vue 6.0.0

Capacitor:

   Capacitor CLI      : 3.3.3
   @capacitor/android : not installed
   @capacitor/core    : 3.3.3
   @capacitor/ios     : not installed

Utility:

   cordova-res : not installed globally
   native-run  : 1.5.0

System:

   NodeJS : v14.17.5 (C:\Program Files\nodejs\node.exe)
   npm    : 6.14.14
   OS     : Windows 10

---

Vue cli: @vue/cli 4.5.15