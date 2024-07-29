## Challenge - Create `commit-msg` hook

After `commitlint` is configured:

1. Create a `commit-msg` hook


## Solution

Create a `commit-msg` hook in your project by running the code below:

```
echo "pnpm dlx commitlint --edit \$1" > .husky/commit-msg
```