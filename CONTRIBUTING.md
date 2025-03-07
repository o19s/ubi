# Contributing

We would ❤️ it if you contributed to the project and helped make UBI even better. We will make sure that contributing to UBI is easy, enjoyable, and educational for anyone and everyone. All contributions are welcome, including features, issues, documentation, translation, guides, and more.

## Got a question?

You can ask questions, consult with more experienced UBI users, and discuss UBI topics in the [Discussions Page](https://github.com/o19s/ubi/discussions/).

You can also join us on Relevancy Slack in the `#user-behavior-insights` channel.

## Found a bug?

If you find a bug in the source code, you can help us by [submitting an issue](https://github.com/o19s/ubi/issues/new?assignees=&labels=type%3A%20bug&template=bug_report.md&title=) to our GitHub Repository. Even better, you can submit a Pull Request with a fix.

## Missing a feature?

You can request a new feature by [submitting an issue](https://github.com/o19s/ubi/issues/new?assignees=&labels=type%3A%20feature%20request&template=feature_request.md&title=) to our GitHub Repository.

If you'd like to implement a new feature, it's always good to be in touch with us before you invest time and effort, since not all features can be supported.

- For a Major Feature, first open an issue and outline your proposal. This will let us coordinate efforts, prevent duplication of work, and help you craft the change so that it's successfully integrated into the project.
- Small Features can be crafted and directly [submitted as a Pull Request](#step-8-create-pull-request).

# <a name="submit-pr"></a> How do I make a code contribution?

Are you new to open source contribution? Wondering how contributions work in our project? Here's a quick rundown.

Find an issue that you're interested in addressing, or a feature that you'd like to add.
You can use [this view](https://github.com/o19s/ubi/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22) which helps new contributors find easy gateways into our project.

## Step 1: Make a fork

Fork the MAC repository to your GitHub organization. This means that you'll have a copy of the repository under _your-GitHub-username/repository-name_.

## Step 2: Clone the repository to your local machine

```
git clone https://github.com/{your-GitHub-username}/mac.git

```

## Step 3: Create a branch

Create a new branch for your fix.

```jsx
git checkout -b branch-name-here
```

## Step 4: Make your changes

Update the code with your bug fix or new feature.

## Step 5: Add the changes that are ready to be committed

Stage the changes that are ready to be committed:

```jsx
git add .
```

## Step 6: Commit the changes (Git)

Commit the changes with a short message. (See below for more details on how we structure our commit messages)

```jsx
git commit -m "<type>: <subject>"
```

## Step 7: Push the changes to the remote repository

Push the changes to the remote repository using:

```jsx
git push origin branch-name-here
```

## Step 8: Create Pull Request

In GitHub, do the following to submit a pull request to the upstream repository:

1.  Give the pull request a title and a short description of the changes made. Include also the issue or bug number associated with your change. Explain the changes that you made, any issues you think exist with the pull request you made, and any questions you have for the maintainer.

Remember, it's okay if your pull request is not perfect (no pull request ever is). The reviewer will be able to help you fix any problems and improve it!

2.  Wait for the pull request to be reviewed by a maintainer.

3.  Make changes to the pull request if the reviewing maintainer recommends them.

Celebrate your success after your pull request is merged :-)

## Git Commit Messages

We structure our commit messages like this:

```
<type>: <subject>
```

Example

```
fix: surnames was not required
```

### Types:

- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Changes to the documentation
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc.)
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **perf**: A code change that improves performance
- **test**: Adding missing or correcting existing tests
- **chore**: Changes to the build process or auxiliary tools and libraries such as documentation generation



## Code of conduct

Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms.

[Code of Conduct](https://github.com/o19s/ubi/blob/master/code_of_conduct.md)

Our Code of Conduct means that you are responsible for treating everyone on the project with respect and courtesy.
