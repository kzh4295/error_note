```js
{
  "name": "boiler-plate",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",

   > debug
  
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },


  
  "author": "jihye",
  "license": "ISC"
}
```

```
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
```


-------------------------------------------------------------------------------------



|  |  |
|:----------|:----------|
| 상황 | node init으로 package.json을 구성한 뒤 script위에 debug 발생 |
| 해결시도 |  1. 주석 처리 -> 다른 파일 실행 과정에서 주석처리로 인한 에러|
|          |  2. npm cache clean --force : 캐시 제거 |
|          |  3. npm install --global node-gyp |
|          |  4. peer dependency install |
|          |  5. "script" "test" : "echo : mocha" 로 수정 |
| 해결 | 이것은 오류가 아니며 "디버그" 텍스트는 실제로 파일의 일부가 아닙니다. VSCode가 패키지 json 파일에서 스크립트를 실행하기 위한 바로 가기로 "디버그" 단추를 삽입합니다. 이 단추를 클릭하면 실행하거나 디버깅할 스크립트를 선택할 수 있는 팝업이 나타납니다. |   








