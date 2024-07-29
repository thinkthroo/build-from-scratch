## Challenge - Install the husky in your Monorepo project

In this challenge, you will have to install husky in your project by following the steps provided in [Get Started](https://typicode.github.io/husky/get-started.html)

## Solution

Run the below command at the root of your Monorepo

```
pnpm install --save-dev husky --workspace-root
```

> Remember to use your chosen package manager at the time of setting up your Monorepo.

If you use `pnpm`, you need to add `--workspace-root` to the command anytime you want to install a package in the workspace level root (Monorepo root folder)