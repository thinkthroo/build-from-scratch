# Husky configuration 

Shadcn-ui/ui uses husky to lint commit messages.

![Screenshot 2024-05-29 at 23.28.31.png](https://strapi-8c8i.onrender.com/uploads/Screenshot_2024_05_29_at_23_28_31_540fb23e2a.png)

Navigate to [shadcn-ui/ui](https://github.com/shadcn-ui/ui) and check the commit messages.

## Challenge

1. Read the [husky documentation](https://typicode.github.io/husky/).
2. Install the husky in your monorepo project.
3. Figure out how to lint your commit messages.

## How to solve this challenge?

### 1. Read the husky documentation

Head to husky documentation and read the [Get started section](https://typicode.github.io/husky/get-started.html).

### 2. Install husky

[Get started](https://typicode.github.io/husky/get-started.html) documentation provides detailed steps to install husky.

### 3. Figure out how to lint your commit messages

Check the files inside [.husky](https://github.com/shadcn-ui/ui/tree/main/.husky) folder in shadcn-ui/ui. Do some research about [commit-msg file](https://github.com/shadcn-ui/ui/blob/main/.husky/commit-msg) and also find out why the default `pre-commit` file from `husky init` does not exist in `.husky` folder.

## Solution

Feeling stuck or need help, you can check solution for this challenge
