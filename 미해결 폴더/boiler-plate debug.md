{
  "name": "boiler-plate",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",

<span style="color:red">debug</span>
<span style="color:#d3d3d3">#d3d3d3</span>
<span style="color:rgb(245, 235, 13)">rgb(245, 235, 13)</span>
  
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


-------------------------------------------------------------------------------------



|  |  |
|:----------|:----------|
| 상황 | node init으로 package.json을 구성하는 과정에서 script위에 debug 발생 |
| 해결시도 |  1. ~~주석 처리 -> 다른 파일 실행 과정에서 주석처리로 인한 에러~~|
|          |  2. ~~npm cache clean --force : 캐시 제거~~ |
|          |  3. ~~npm install --global node-gyp~~ |
|          |  4. ~~peer dependency install~~ |
|          |  5. ~~"script" "test" : "echo : mocha" 로 수정~~ |
| 해결 | This is not an error and the "debug" text is not actually part of the file VSCode inserts the "debug" button as a shortcut for running the scripts in the packagejson file When you click on it, a popup will appear allowing you to select the script you want to run or debug. |   








