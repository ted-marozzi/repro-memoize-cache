# Repo of Lodash Memoise type issue

## Reproduce this issue with npm test

```
/usr/local/src/repro-memoize-cache$ npm test

> repro-memoize-cache@1.0.0 test
> vitest


 DEV  v0.21.0 /usr/local/src/repro-memoize-cache

 ❯ index.test.ts (0)

⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯ Failed Suites 1 ⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯

 FAIL  index.test.ts [ index.test.ts ]
TypeError: (memoize.Cache || MapCache) is not a constructor
 ❯ memoize node_modules/lodash/memoize.js:66:20
 ❯ h node_modules/swagger-ui/dist/swagger-ui-es-bundle-core.js:2:125349

 ❯ 2473 node_modules/swagger-ui/dist/swagger-ui-es-bundle-core.js:2:84210
 ❯ Ge node_modules/swagger-ui/dist/swagger-ui-es-bundle-core.js:2:233952
 ❯ 6298 node_modules/swagger-ui/dist/swagger-ui-es-bundle-core.js:2:112962
 ❯ Ge node_modules/swagger-ui/dist/swagger-ui-es-bundle-core.js:2:233952
 ❯ node_modules/swagger-ui/dist/swagger-ui-es-bundle-core.js:2:235376
 ❯ node_modules/swagger-ui/dist/swagger-ui-es-bundle-core.js:2:366155
 ❯ async /usr/local/src/repro-memoize-cache/index.test.ts:3:31

⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯[1/1]⎯

Test Files  1 failed (1)
     Tests  no tests
  Start at  14:44:38
  Duration  2.33s (setup 0ms, collect 0ms, tests 0ms)
```
