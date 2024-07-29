## Challenge - Link Your Turbo Monorepo to the GitHub Repository

The GitHub repository you have just created is empty. In this challenge, you have to link your local Git repository to remote Github repository, and then push your codes.

Make sure you read the official documentation to [add a local repository to GitHub using Git](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github?platform=mac#adding-a-local-repository-to-github-using-git)

## Solution

When you create Turbo Monorepo with `npx create-turbo@latest`, it initializes a local Git repository by default.

Now, After your new GitHub repository created, you can link your Turbo Monorepo with the GitHub repository.

In the command line, go to your turbo project, and run this command.

```
git remote add origin git@github.com:<your-github-username>/<your-github-repo>.git
git push -u origin main
```

If your PC is already authenticated to your GitHub account, the command above should be successful and your Turbo Monorepo is now pushed to GitHub. But, if it prompts an authentication request, you can insert your GitHub account credentials.

You can read about GitHub Authentication [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github).