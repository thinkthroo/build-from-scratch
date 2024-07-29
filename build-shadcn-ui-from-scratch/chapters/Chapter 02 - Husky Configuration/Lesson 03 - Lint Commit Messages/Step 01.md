## Challenge - Figure out how to lint your commit messages

Check the files inside [.husky](https://github.com/shadcn-ui/ui/tree/main/.husky) folder in shadcn-ui/ui. Do some research about [commit-msg file](https://github.com/shadcn-ui/ui/blob/main/.husky/commit-msg) and also find out why the default `pre-commit` file from `husky init` does not exist in `.husky` folder.

In this challenge, you will have complete below tasks:

1. Understanding `commitlint`
2. Installing `commitlint`

## Solution

[`commit-msg` hook in shadcn-ui/ui](https://github.com/shadcn-ui/ui/blob/main/.husky/commit-msg) uses the below command to lint commit messages.

```
#!/usr/bin/env sh
. "$(dirname -- "$0")/_/husky.sh"

npx commitlint --edit $1
```

[commitlint](https://commitlint.js.org/guides/getting-started.html) is used to lint your commit messages.

Do read the below `commitlint` guides:

1. https://commitlint.js.org/guides/getting-started.html
2. https://commitlint.js.org/guides/local-setup.html

### Install `commitlint`

Run the below command to install `commitlint` as your dev dependency:

```
pnpm add --save-dev @commitlint/{cli,config-conventional} --workspace-root
```