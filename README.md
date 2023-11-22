# Renovate Issue #21438 Reproduction

- issue: [renovatebot/renovate#21438](https://github.com/renovatebot/renovate/issues/21438)

## Current behavior

For those updates that comply with the range specified in the `package.json` file, i.e., which do not need to make a change in the `package.json` file, Renovate failed to create a PR when using PNPM as the package manager.

<details>
  <summary>Updates failed to be created</summary>

 - <!-- other-branch=renovate/autoprefixer-10.x-lockfile -->Update dependency autoprefixer to v10.4.16
 - <!-- other-branch=renovate/postcss-8.x-lockfile -->Update dependency postcss to v8.4.31
 - <!-- other-branch=renovate/prettier-2.x-lockfile -->Update dependency prettier to v2.8.8 (`prettier`, `@types/prettier`)
 - <!-- other-branch=renovate/tailwind-scrollbar-3.x-lockfile -->Update dependency tailwind-scrollbar to v3.0.5
 - <!-- other-branch=renovate/node-18.x-lockfile -->Update dependency @types/node to v18.18.12
 - <!-- other-branch=renovate/eslint-8.x-lockfile -->Update dependency eslint to v8.54.0 (`eslint`, `@types/eslint`)
 - <!-- other-branch=renovate/framer-motion-10.x-lockfile -->Update dependency framer-motion to v10.16.5
 - <!-- other-branch=renovate/jotai-2.x-lockfile -->Update dependency jotai to v2.5.1
 - <!-- other-branch=renovate/react-hook-form-7.x-lockfile -->Update dependency react-hook-form to v7.48.2
 - <!-- other-branch=renovate/react-icons-4.x-lockfile -->Update dependency react-icons to v4.12.0
 - <!-- other-branch=renovate/tailwindcss-3.x-lockfile -->Update dependency tailwindcss to v3.3.5
 - <!-- other-branch=renovate/zod-3.x-lockfile -->Update dependency zod to v3.22.4
 - <!-- other-branch=renovate/nextjs-monorepo -->Update nextjs monorepo to v13.5.6 (`eslint-config-next`, `next`)
 - <!-- other-branch=renovate/react-monorepo -->Update react monorepo (`@types/react`, `@types/react-dom`)
 - <!-- other-branch=renovate/typescript-eslint-monorepo -->Update typescript-eslint monorepo to v5.62.0 (`@typescript-eslint/eslint-plugin`, `@typescript-eslint/parser`)

</details>

[Renovate Log](./renovate.log)

## Expected behavior

Renovate should be able to open a PR with the versions updated in the `pnpm-lock.yaml` file just like how `npm` and `yarn`-based repositories are.
