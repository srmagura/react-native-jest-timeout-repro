# jest-expo-timeout-repro

## Repro Steps

1. `yarn install`
2. `yarn test`

**Expected behavior:** Test passes in < 10ms.

**Actual behavior:** Test times out after 5 seconds.

Remove `jest-expo` from `jest.config.js` and the test will pass.
