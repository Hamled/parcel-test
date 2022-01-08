# Parcel resolve error

## Configuration

1. Arch Linux: `Linux malu 5.15.13-arch1-1 #1 SMP PREEMPT Wed, 05 Jan 2022 16:20:59 +0000 x86_64 GNU/Linux`
1. `node --version`: `v17.3.0`
1. `yarn --version`: `3.1.1`
1. parcel package version is 2.1.1
1. `yarn` was installed with: `corepack enable --install-directory ~/.local/bin` and then `yarn set version 3.1.0`

## Project setup commands:

1. `yarn init -2`
1. And the commands from the [Parcel getting started tutorial for libraries](https://parceljs.org/getting-started/library/)

## Error result:

1. When running `yarn build` (after performing the tutorial to add scripts for parcel to `package.json`) I get the following error message:

```text
🚨 Build failed.

@parcel/transformer-js: Could not resolve module "@parcel/core" from "/home/charles/tmp/parcel-test/.yarn/__virtual__/@parcel-workers-virtual-efd5323745/0/cache/@parcel-workers-npm-2.1.1-f042fe0b0e-b49cb0443b.zip/node_modules/@parcel/workers/lib/Handle.js"

  Error: Could not resolve module "@parcel/core" from "/home/charles/tmp/parcel-test/.yarn/__virtual__/@parcel-workers-virtual-efd5323745/0/cache/@parcel-workers-npm-2.1.1-f042fe0b0e-b49cb0443b.zip/node_modules/@parcel/workers/lib/Handle.js"
  at NodeResolverSync.resolve (/home/charles/tmp/parcel-test/.yarn/__virtual__/@parcel-package-manager-virtual-d1b88c7bb9/0/cache/@parcel-package-manager-npm-2.1.1-a3dae91c51-0cf14f0fb1.zip/node_modules/@parcel/package-manager/lib/NodeResolverSync.js:36:15)
  at NodePackageManager.resolveSync (/home/charles/tmp/parcel-test/.yarn/__virtual__/@parcel-package-manager-virtual-d1b88c7bb9/0/cache/@parcel-package-manager-npm-2.1.1-a3dae91c51-0cf14f0fb1.zip/node_modules/@parcel/package-manager/lib/NodePackageManager.js:313:36)
  at NodePackageManager.requireSync (/home/charles/tmp/parcel-test/.yarn/__virtual__/@parcel-package-manager-virtual-d1b88c7bb9/0/cache/@parcel-package-manager-npm-2.1.1-a3dae91c51-0cf14f0fb1.zip/node_modules/@parcel/package-manager/lib/NodePackageManager.js:127:14)
  at Module.m.require (/home/charles/tmp/parcel-test/.yarn/__virtual__/@parcel-package-manager-virtual-d1b88c7bb9/0/cache/@parcel-package-manager-npm-2.1.1-a3dae91c51-0cf14f0fb1.zip/node_modules/@parcel/package-manager/lib/NodePackageManager.js:151:19)
  at require (node:internal/modules/cjs/helpers:102:18)
  at _core (/home/charles/tmp/parcel-test/.yarn/__virtual__/@parcel-workers-virtual-efd5323745/0/cache/@parcel-workers-npm-2.1.1-f042fe0b0e-b49cb0443b.zip/node_modules/@parcel/workers/lib/Handle.js:9:16)
  at Object.<anonymous> (/home/charles/tmp/parcel-test/.yarn/__virtual__/@parcel-workers-virtual-efd5323745/0/cache/@parcel-workers-npm-2.1.1-f042fe0b0e-b49cb0443b.zip/node_modules/@parcel/workers/lib/Handle.js:57:5)
  at Module._compile (node:internal/modules/cjs/loader:1097:14)
  at Object.Module._extensions..js (node:internal/modules/cjs/loader:1149:10)
  at Module.load (node:internal/modules/cjs/loader:975:32)
```
