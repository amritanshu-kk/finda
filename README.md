## About Us

Edunica4IN (CodingCoach) is a FREE platform that is built entirely for developers.


## Requirements

- Git should be installed [Install Git](https://git-scm.com/downloads)
- Nodejs [Install Nodejs](https://nodejs.org/en/download/). **Notice v11.11.0 breaks the tests**
- Yarn (we recommend using yarn as a package manager) [Install Yarn](https://yarnpkg.com/en/)

## Want to contribute to this project?

That's why we're here! 😀

Have an idea? Please **use a branch** and [create a PR](https://help.github.com/articles/creating-a-pull-request/). If you aren't sure how to do this, ask us or find a mentor who can assist.

Don't have time to code it? Please open an [issue](https://github.com/Coding-Coach/find-a-mentor/issues/new).

### Workflow

This section describes the workflow we are going to follow when working on a new feature or fixing a bug. If you want to contribute, please follow these steps:

1. Fork this project
2. Clone the forked project to your local environment, for example: `git clone git@github.com:crysfel/coding-coach-front-end.git` (Make sure to replace the URL with the one to your own repository).
3. Add the original project as a remote, for this example the name is `upstream`, feel free to use whatever name you want. `git remote add upstream https://github.com/Coding-Coach/find-a-mentor.git`.

Forking the project will create a copy of that project in your own GitHub account, you will commit your work against your own repository.

#### Quick start

1. Navigate to the project folder.
2. Run `yarn`
3. Run `yarn test`
4. Type `a` to run all tests
5. Type `q` to quit (this will start cypress and set that up)
6. If the browser doesn't open automatically, navigate to [http://localhost:3000](http://localhost:3000) to see the site.

For other options, please see [Available Scripts](https://github.com/Coding-Coach/find-a-mentor#available-scripts) below.


**Production**

https://mentors.codingcoach.io/sb/

**Local**

```
yarn storybook
```

The stories are located under `src/stories`

#### Updating your local

In order to update your local environment to the latest version on `master`, you will have to pull the changes using the `upstream` repository, for example: `git pull upstream master`. This will pull all the new commits from the origin repository to your local environment.

#### Features/Bugs

When working on a new feature, create a new branch `feature/something` from the `master` branch, for example `feature/login-form`. Commit your work against this new branch and push everything to your forked project. Once everything is completed, you should create a PR to the original project. Make sure to add a description about your work.

When fixing a bug, create a new branch `fix/something` from the `master` branch, for example `fix/css-btn-issues`. When completed, push your commits to your forked repository and create a PR from there. Please make sure to describe what was the problem and how did you fix it.

#### Updating your local branch

Let's say you've been working on a feature for a couple days, most likely there are new changes in `master` and your branch is behind. In order to update it to the latest (You might not need/want to do this) you need to pull the latest changes to `master` and then rebase your current branch.

```bash
$ git checkout master
$ git pull upstream master
$ git checkout feature/something-awesome
$ git rebase master
```

After this, your commits will be on top of the `master` commits. From here you can push to your `origin` repository and create a PR.

You might have some conflicts while rebasing, try to resolve the conflicts for each individual commit. Rebasing is intimidating at the beginning, if you need help, don't be afraid to reach out in Slack.

---

This project was created with [Next.js](https://nextjs.org/)

## Available Scripts

In the project directory, you can run:

### `yarn dev`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner.

### `yarn test:e2e`

Launches the `Cypress` test runner _and_ the app; must run on port `3000`. Learn more about `Cypress` [on their website](https://docs.cypress.io/guides/overview/why-cypress.html#In-a-nutshell).

Alternatively You can also use Gitpod ( a free online IDE that will automate your dev setup )  for contributing with a single click. It will launch a ready to code workspace with the dependencies pre-installed so that you can start contributing without wasting precious time on development setup.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/Coding-Coach/find-a-mentor)