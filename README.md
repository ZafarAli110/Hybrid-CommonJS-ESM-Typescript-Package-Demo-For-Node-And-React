# Simple Monorepo with PNPM Workspace
A simple monorepo starter featuring a workspace set up using pnpm that demonstrates a hybrid CJS and ESM typescript library. The repository contains apps and packages folders.

## About The Project
This project has the following components:

apps/react-app: a React application created with Vite.js that demonstrates how to consume the packages/lib library.
apps/node-app: a Node.js application that also demonstrates how to consume the packages/lib library.
packages/lib: a simple hybrid TypeScript library that support both commonjs and esm format that can be consumed by both apps/react-app and apps/node-app.

## Getting Started
To get started, follow these steps:

Clone this repository.

Install dependencies using pnpm install.

Make sure to build the typscript library first by running the following command from the root
```
pnpm --filter lib build or run pnpm build:lib

```

From the root run the following commands to run the react and node application 
```
pnpm --filter react-app dev or pnpm vite:dev
pnpm --filter node-app start or pnpm node:start

```


Contributing
Contributions are always welcome! Here's how you can contribute:

Fork the repo.
Create a new branch.
Make necessary changes in the code/files.
Commit your changes with a meaningful commit message.
Push your changes to the branch.
Submit a Pull Request explaining the changes you've made.
License
See LICENSE for more information.
