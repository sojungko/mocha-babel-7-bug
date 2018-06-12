# mocha-babel-7-bug

1. `yarn`
2. `yarn test`
3. Should see error:
```
import expect from 'expect';
^^^^^^
SyntaxError: Unexpected token import
    at createScript (vm.js:56:10)
    at Object.runInThisContext (vm.js:97:10)
    at Module._compile (module.js:542:28)
    at Module._compile (/Users/spark/mocha-test/node_modules/pirates/lib/index.js:91:24)
    at Module._extensions..js (module.js:579:10)
    at Object.newLoader [as .js] (/Users/spark/mocha-test/node_modules/pirates/lib/index.js:96:7)
    at Module.load (module.js:487:32)
    at tryModuleLoad (module.js:446:12)
    at Function.Module._load (module.js:438:3)
    at Module.require (module.js:497:17)
    at require (internal/module.js:20:19)
    at /Users/spark/mocha-test/node_modules/mocha/lib/mocha.js:250:27
    at Array.forEach (native)
    at Mocha.loadFiles (/Users/spark/mocha-test/node_modules/mocha/lib/mocha.js:247:14)
    at Mocha.run (/Users/spark/mocha-test/node_modules/mocha/lib/mocha.js:576:10)
    at Object.<anonymous> (/Users/spark/mocha-test/node_modules/mocha/bin/_mocha:637:18)
    at Module._compile (module.js:570:32)
    at Object.Module._extensions..js (module.js:579:10)
    at Module.load (module.js:487:32)
    at tryModuleLoad (module.js:446:12)
    at Function.Module._load (module.js:438:3)
    at Module.runMain (module.js:604:10)
    at run (bootstrap_node.js:389:7)
    at startup (bootstrap_node.js:149:9)
    at bootstrap_node.js:504:3
```
