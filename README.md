# React Library Starter

Starter template for your next react typescript library. Complete with changeset, tsup, and tailwind with prettier-plugin. Publish to npm the right and easy way.

## Setup

1. Go to npm and create your access token with type of "Publish" or "Automation". Copy the token.
2. Go to your repo, click on "Settings" => "Secrets and variables" => "Actions" => "New repository secret" then create token named "NPM_TOKEN" and paste token from step 1.
3. Go to your repo, click on "Settings" => "Actions" => "General" then make sure Workflow permissions is set to "Read and write permissions" and check "Allow Github Actions to create and approve pull requests."

## How to use

Create your package in package/index. Then import and test from src/App.

Run `pnpm changeset` then push to your Github and workflow will create a PR for you to merge. Once you merge, your package will be automatically publish to npm.

Or run `pnpm release` to publish directly from your command line. Remember to login with `npm login` and update version property in package.json.
