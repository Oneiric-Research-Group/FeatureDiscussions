# Welcome to Oneiric Research Group contributing guide

Thank you for joining our journey and helping us build AI x NFTs x Gaming

In this guide you will get an overview of the contribution workflow from opening an issue, creating a PR, reviewing, and merging the PR.

## New contributor guide

To get an overview of the project, please read the [README](README.md).

Here are some resources to help you get started with open-source contributions:

### Disclaimer

By contributing to this repository you provide Oneiric Research Group the ownership of any IP contributed to the project to use indefinitely. This includes code, discussions (ideas) and all types of artwork. While often designers and developers are rewarded with the NFTs and airdrops, there is no guarantee of reward.

You confirm you have the rights to the content you are contributing to the project.

## Getting started

1. Create a [Github](https://www.github.com) Account
2. Go to the [Oneiric Research Group Github Repository](https://github.com/Oneiric-Research-Group)
3. Fork the Repo to your account.
   (Impt) Make sure you fork the repo to contribute back to the parent repo
4. Download and install [Github Desktop](https://desktop.github.com/).
5. Clone your forked repo to your Github Desktop app. Again select the option to contribute to the parent repo.
6. Download and install [Visual Studio Code](https://code.visualstudio.com/Download)
7. Download and install [Git Bash](https://git-scm.com/downloads)
8. Download and install [Node.js](https://nodejs.org/en)
9. Once you installed all the required programs, go back to Github Desktop and go to File>Options>Integrations. Change the external Editor to Visual Studio Code
10. Change Shell to Git Bash
11. Open Visual Studio Code from Github Desktop. Alternatively you can use the keyboard shortcut `Ctrl + Shift + A`
12. Use the keyboard shortcut `Ctrl + Shift + P` and type in `Terminal: Select Default Profile`
13. Set Default Profile to Git Bash
14. Click on the 3 dots>Terminal>Open terminal or use the shortcut `Ctrl + Shift + ` `
15. Enter the following commands into terminal:

`npm install -g yarn`

_It may prompt you to install a newer version and tell you to enter a command to install it. Enter the provided command to install;_

`yarn install` or `yarn`

Installs yarn into your system based on the packages in [package.json](package.json);

`cp .env.sample .env`

Creates a `.env ` file which contains the data for running the code locally on your device;

_Bonus Command (not needed for setup):_

`yarn dev`

_Runs the code locally on your device_

🎉Congratulations! You are now set to contribute code to the Oneiric Research Group Repository!

### Issues

#### Create a new issue

If you spot a problem with the docs, [search if an issue already exists](https://docs.github.com/en/github/searching-for-information-on-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments). If a related issue doesn't exist, you can open a new issue using a relevant [issue form](https://github.com/github/docs/issues/new/choose).

#### Solve an issue

Scan through our [existing issues](https://github.com/Oneiric-Research-Group/FeatureDiscussions/issues) to find one that interests you. You can narrow down the search using `labels` as filters. See [Labels](https://docs.github.com/en/issues/tracking-your-work-with-issues/filtering-and-searching-issues-and-pull-requests#filtering-issues-and-pull-requests-by-labels) for more information.

As a general rule, we assign features with deadlines to core team members. If a ticket is already assigned and you are passionate about it, please reach out to the developer on the issue comments and help them out.

## How can I help?

If you have a bright idea, open an issue or join our active Discord #devs-chat first and start a discussion. We love to bring in the community ideas where possible!

Don't have any ideas? We would suggest scanning the open issues and seeing if there is something that catches your eye.

You can search by labels as well to see which items are more urgent than others.

## What should I work on?

Maintaining a project with over 50 open-source developers brings a range of challenges:

- Maintaining a consistent vision
- Ensuring best architecture practices
- Security concerns and vulnerabilities
- Automated and manual testing
- Readability and maintainability
- Managing expectations, deadlines and contributors leaving the project
- Tokenomics design
- Anything that gets added to the project is more code that needs to be maintained by Thought Farm.

While we appreciate UI and gameplay PRs, we need these pieces of work to fit into the core team's development workflow to ensure work is pair programmed, has sufficient automated testing, is understood by the team, is peer-reviewed, aligns with the tokenomics of the game and adheres with the vision of the project.

Due to the limited time resources of the team, at this point of time, we cannot accept any PRs that introduce major gameplay changes or UI workflows.

If you have an idea that introduces new UI workflows or gameplay, the best way forward is to first raise the idea for community and if consensus is met, it will get added to the roadmap. Once an item is on the roadmap, the core functionality will be developed by Thought Farm with the support from certified developers and the community. For new gameplay and UI workflows there will be plenty of tasks that can be worked on by community members.

**Examples of what can be worked on independently**

- Bug fixes
- Decorations
- Minor UI enhancements - Typos, buttons, alignment, colours
- CI & Build improvements
- Writing tests
- Animations + game polish

**Examples of what the core team will need to be involved in**

- New game features
- Major UI & UX workflows
- Architecture changes (state management, data storage, routers etc.)
- Smart contracts & APIs
- Testing infrastructure
- Repo tooling (testing, components, build)

### Update your Branch

Periodically the devs may push commits to the repository but they do not automatically appear in your local system.

Before starting on your project, be sure to update your branch first

To do this you can do the following steps:

1. Go to your forked repo page and if there's any commits that are missing from your repo you should see a message 
2. Click on Sync Fork
3. Click on Update Branch
4. Go back to Github Desktop and click on Fetch Origin
5. Click on Pull Origin

Your branch should be updated with the main ORG repo now.

### Make Changes

#### Make changes locally

1. Open Github Desktop
2. Create a new branch
   Create the branch based on `upstream/main` if this pops up
3. Once created, the program should switch you over to the branch that you just created.
4. Open VS Code
5. Make changes to the issue you're trying to resolve in VS Code.

### Preparing to submit

Before you submit, ensure you have done the following:

- Written tests for any business logic code
- Provided sufficient comments on the code
- Manually tested your code by running the repo.
  Some tests you can run:

`yarn dev`

Test your changes locally on your system;

`yarn tsc`

Runs typescript code to check for any syntax errors;

`yarn test`

Runs tests to make sure the code runs well

### Commit your update

Commit the changes once you are happy with them. We prefer atomic commits that are easily revertable.

> **TIP:** If your changes include **only** documentation updates/additions/deletions,
> make sure that you add below line to your commit message while committing:
>
> **`[skip ci]`**
>
> This **_won't_** trigger the GitHub Actions CI Workflow in turn, it **_won't_** waste the resources. 🤗 🌏
>
> > E.g.
> >
> > ```
> > [CHORE] Update README.md
> > [skip ci]
> > ```

Once you confirmed your changes, go to the Source Control Panel and name your commit. Once ready, click on commit. Then sync your changes with the remote
Then sync your changes

_Bonus fyi: There are other options for commit but they do different things:_

- _Commit: Commits the file locally on your drive_
- _Commit (Amend): Adds new stage changes to the most recent pushed commit_
- _Commit and Push: Commits the file and pushes it to the remote_
- _Commit and Sync: Commits the file and syncs your local branch with the remote branch_

### Pull Request

When you're finished with the changes, create a pull request, also known as a PR.

You will want to prefix the name of your PR with the category it falls under:

- [FEAT] Feature or enhancement
- [CHORE] Admin type work (scripts, documentation etc)
- [FIX] A bug fix

For example - "[FEAT] Add new module"

- Once you submit your PR, a Oneiric Research Group team member will review your proposal. We may ask questions or request for additional information.
- We may ask for changes to be made before a PR can be merged
- As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
- If you run into any merge issues, checkout this [git tutorial](https://lab.github.com/githubtraining/managing-merge-conflicts) to help you resolve merge conflicts and other issues.

When a PR is opened we run Github Actions to ensure the quality of the code is up to standards. This includes:

- Typescript check
- Jest (unit testing)

### Your PR is merged!

Congratulations 🎉🎉 The Oneiric Research Group Dev Team thanks you for your contributions!✨️