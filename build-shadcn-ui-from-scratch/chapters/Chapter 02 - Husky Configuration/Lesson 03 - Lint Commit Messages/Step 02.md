## Challenge - Configure `commitlint`

In this challenge, you will have complete below tasks:

1. Configure `commitlint` to make `commit-msg` hook to work

## Solution

You need `commitlint.config.js` for this `commit-msg` hook to work. Run the below command after installing `commitlint`.

```
echo "export default { extends: ['@commitlint/config-conventional'] };" > commitlint.config.js
```

