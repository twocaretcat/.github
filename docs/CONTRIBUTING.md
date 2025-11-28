# 🤝 Contributing Guidelines

Thanks for your interest in contributing to the project! We don't have a specific contribution process for this project yet, but here are some general guidelines.

## Open to Contributions?

Check the README first to see if this project accepts contributions. Most of my projects do, but some projects are not maintained or are for personal use only. If you're not sure, **create a dicussion** to ask.

## Finding Issues to Work On

Issues with the `🚦 ready` label are ready to be worked on. If you comment on an issue, I can assign it to you.

Issues with the `🚦 needs triage` label generally need some more information before they can be worked on, but if you
**start a discussion** about it or leave a comment on the issue, I can likely get it ready for you.

If an issue is unclear or you have any questions about how a feature should be implemented, reach out before making any
changes so we can discuss the best way to do it.

## Development Workflow

### Prerequisites

There are usually installation and usage instructions in the README, so check there first for what you need to get started. If the README doesn't have this information, you might need to take a peek at the source code.

### Getting Started

Here's a quick example of how to contribute a new feature or bug fix:

1. Fork and clone the repository:

   ```bash
   git clone https://github.com/OWNER/REPO.git
   cd REPO
   ```

2. Create a new branch:

   ```bash
   git checkout -b feat/your-feature-name
   ```

   You can also do this from the relevant GitHub issue.

   See the [Branch Names](#branch-names) section below for how to name branches.

3. Make your changes
4. Write or update tests as needed
5. Write or update docs as needed
6. Run any other commands you can find for verifying code quality (ex. linting, formatting, typechecking, etc.)

   You can often find these commands in the README or in the project's `package.json`.

7. Commit your changes:

   ```bash
   git add .
   git commit -m "feat: add your feature description"
   ```

   See the [Commit Messages](#commit-messages) section below how to write commit messages.

8. Push and create a pull request:

   ```bash
   git push origin feat/your-feature-name
   ```

9. Request a review from a maintainer and wait for feedback

See below for more details.

## Code Style Guidelines

See the existing source for examples of how to write code that fits with the project's style.

### Formatting

My projects are generally auto-formatted with tabs and single quotes. Check the README or `package.json` for details on the exact tool used.

Make sure code is formatted correctly before creating a pull request.

### Documentation

Documentation should be kept up-to-date with code changes.

The README usually contains everything you need to know to use the project. Contributing information and other documentation can usually be found in the docs/ directory.

Some larger projects have a dedicated documentation site.

### Testing

If the project has tests, make sure they pass before creating a pull request.

Check the README or `package.json` for details on how tests are set up.

### Commit Messages

We follow [Conventional Commits]:

- `feat:` - New features
- `fix:` - Bug fixes
- `docs:` - Documentation changes
- `refactor:` - Code refactoring
- `test:` - Test additions or modifications
- `chore:` - Maintenance tasks

If you are making a breaking change, add an exclamation mark after the type and a `BREAKING CHANGE:` footer further
explaining the breaking changes for users. For example:

<!-- Example from https://www.conventionalcommits.org/en/v1.0.0/ | MIT -->

```txt
feat!: allow provided config object to extend other configs

BREAKING CHANGE: `extends` key in config file is now used for extending other config files
```

This text is included in release notes, so it should be clear and concise.

### Branch Names

We prefix branch names with types from [Conventional Commits]. For example:

```txt
feat/some-feature
fix/some-bug
docs/update-readme
```

## License

By contributing to this project, you agree that your contributions will be licensed under the project
license.

[Conventional Commits]: https://www.conventionalcommits.org/
