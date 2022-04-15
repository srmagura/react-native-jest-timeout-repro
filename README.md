# react-native-jest-timeout-repro

Shows that Jest fake timers do not work with the react-native Jest preset.

## Repro Steps

1. `yarn install`
2. `yarn test`

**Expected behavior:** Test passes in < 10ms.

**Actual behavior:** Test times out after 5 seconds.

Remove the `react-native` preset from `jest.config.js` and the test will pass.
