{
  "name": "boiler-plate",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  Debug발생!!!!
  이경우) 테스트 스크립트에서 디버그 발생했으므로 해당 부분을 주석으로 처리해주면 해결 됨
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },

   // "scripts": {
  //   "test": "echo \"Error: no test specified\" && exit 1"
  // },
  
  "author": "jihye",
  "license": "ISC"
}


터미널) npm run test
Debugger listening on ws://127.0.0.1:52409/78c1e268-5ae2-4afb-850a-a16768358223
For help, see: https://nodejs.org/en/docs/inspector
Debugger attached.
Waiting for the debugger to disconnect...
(base) ➜  boiler-plate npm run test
Debugger listening on ws://127.0.0.1:52416/77c0e4b5-0a41-42ea-80b2-a7047cd0fb04
For help, see: https://nodejs.org/en/docs/inspector
Debugger attached.

> boiler-plate@1.0.0 test /Users/pro/Documents/boiler-plate
> echo "Error: no test specified" && exit 1

Error: no test specified
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! boiler-plate@1.0.0 test: `echo "Error: no test specified" && exit 1`
npm ERR! Exit status 1
npm ERR! 
npm ERR! Failed at the boiler-plate@1.0.0 test script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.
npm WARN Local package.json exists, but node_modules missing, did you mean to install?

npm ERR! A complete log of this run can be found in:
npm ERR!     /Users/pro/.npm/_logs/2021-02-14T05_34_28_205Z-debug.log
Waiting for the debugger to disconnect...
(base) ➜  boiler-plate 