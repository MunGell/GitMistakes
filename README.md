# GitMistakes

A collection of mistakes I saw in repositories around the Internet that I hope we could avoid.

### 1. Short, undescriptive commit messages

#### Why is it mistake

One of the advantages of using Git is being able to see history of all changes in your repository. Having descriptive clear commit message makes it easy to navigate in history and track changes.

#### How to avoid it

Try to explain what was changed in your commit in 80 characters.

#### Examples

- [5b2b8bf](https://github.com/MunGell/GitMistakes/commit/15b47b41ac8ac0f44a84e6893bb9222a1949ee72)
- [cec5f10](https://github.com/MunGell/GitMistakes/commit/cec5f1038b4f2e714324d914520b74bf6ecaae31)
- [33c719a](https://github.com/MunGell/GitMistakes/commit/33c719aa18c98fbbac3f70b07a5f802e13a38ddf)

### 2. Documentation in commit messages

#### Why is it mistake

Almost opposite to the previous point – documenting code or changes in commit messages. Commits contain very time-specific information, while documentation is relevant for a much longer period. No one is going to scroll through a long list of commits to find description of a particular piece of code and reasoning behind it.

#### How to avoid it

Commit message should be short and informative, it describes the change that you made. Everything else is better to be placed in the code itself or in any other resource that you use for documentation.

#### Examples

- [381f9d9](https://github.com/MunGell/GitMistakes/commit/381f9d931e1e8f678f3f0f9da6de0ea558d3d1b9)

### 3. Describing code instead of describing change in commit message

#### Why is it mistake

Git already provides us with `git diff` functionality that shows differences between file versions, so description of _additions_ and _deletions_ in commit message does not any value.

#### How to avoid it

It would be much more helpful to explain what was actually changed in term of functionality or meaning.

## License

CC0 1.0 Universal
