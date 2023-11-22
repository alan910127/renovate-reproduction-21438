# Renovate Issue #21438 Reproduction

- issue: [renovatebot/renovate#21438](https://github.com/renovatebot/renovate/issues/21438)

## Current behavior

For those updates that comply with the range specified in the `package.json` file, i.e., which do not need to make a change in the `package.json` file, Renovate failed to create a PR when using PNPM as the package manager.

[Renovate Log](./renovate.log)

## Expected behavior

Renovate should be able to open a PR with the versions changed in the `pnpm-lock.yaml` file just like how `npm` and `yarn`-based repositories are.
