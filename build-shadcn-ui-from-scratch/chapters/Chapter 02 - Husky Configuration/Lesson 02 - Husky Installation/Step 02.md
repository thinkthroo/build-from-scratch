## Challenge - Initialize Husky

In this challenge, you will have to complete the below task:

1. Initialize husky to implement it in your Monorepo

## Solution

### husky init

Husky recommends using `init` command. The init command simplifies setting up Husky in a project. It creates a `pre-commit` script in `.husky/` and updates the prepare script in `package.json`. Modifications can be made later to suit your workflow.

```
pnpm exec husky init
```

Take some time and understand the files inside `.husky` folder at the root of your project.

#### `pre-commit` hook

By default, husky creates a file named `pre-commit` containing the code below:

```
pnpm test
```

If you want to run tests before a git commit, you can put your test scripts in this file but [`.husky` folder in `shadcn-ui/ui`](https://github.com/shadcn-ui/ui/tree/main/.husky) does not have `pre-commit` file.

For now, you can delete the `pre-commit` file.

#### `commit-msg` hook

 [`.husky` folder in `shadcn-ui/ui`](https://github.com/shadcn-ui/ui/tree/main/.husky) has a single file named `commit-msg` and it contains the below code:

```
#!/usr/bin/env sh
. "$(dirname -- "$0")/_/husky.sh"

npx commitlint --edit $1
```