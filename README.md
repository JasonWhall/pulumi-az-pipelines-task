# Pulumi Azure RM Task for Azure Pipelines

## Release status

This lib is in alpha. **Do not make this repo public yet!**

## Prerequisites

- Node (>= 8.x)
- Yarn (>= 1.13.0)
- tslint (`npm i -g tslint`)
- typescript compiler (`npm i -g typescript`)

## Local Development

- Set the `AGENT_TOOLSDIRECTORY` env var to any directory for caching the pulumi tool.
- You can run the tool either from the root directory or the `buildAndReleaseTask` directory.
  - To run from the root folder, simply run `npm start`.
  - To run from the `buildAndReleaseTask` folder, run `tsc && node index.js` from the `buildAndReleaseTask` directory.

## Package

> Learn more [here](https://docs.microsoft.com/en-us/azure/devops/extend/develop/add-build-task?view=azure-devops#step-4-package-your-extension).

Ensure you have `tfx` cli installed by running `tfx version`. If it is not installed, then run `npm i -g tfx-cli`.

Run `npm run package` from the root directory.
