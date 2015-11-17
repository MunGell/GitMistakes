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

#### Examples

- [eaeff4b](https://github.com/MunGell/GitMistakes/commit/eaeff4ba46f78c5d3b7e1d106e358b8148a78245)

### 4. Commit merge conflict pointers

#### Why is it mistake

In most cases your code will stop working.

#### How to avoid it

Check the conflicting files.
If you are unsure if you resolved all the conflicts - search in file for ">>>".

#### Examples

- [0a5c8e5](https://github.com/MunGell/GitMistakes/commit/0a5c8e54ae6a892360d2da0baa2b529d5d76f62a)

### 5. Remove merge conflict information from merge commit

#### Why is it mistake

Usually git automatically adds infomation about conflicted files into merge commit message. This information is important for future use in case of any problems with code loss and wrong conflict resolutions.

#### How to avoid it

Just do not delete this information from there. It costs you nothing to store it  and one day it might save you days of debugging.

#### Examples

- [dff1d64](https://github.com/MunGell/GitMistakes/commit/dff1d644a1da2718081d608070991a896adb70a9)

### 6. Make changes in conflicted merge

#### Why is it mistake

When git asks you to manually resolve a merge conflict it also allows you to make any changes in the code that will be then added to the merge commit.
This kind of changes are incredibly difficult to track, which makes git pointless for the project.

#### How to avoid it

Never ever change anything in your code other than conflicting part. Create a separate commit - it costs nothing anyways.

#### Examples

- Uh-oh

## License

CC0 1.0 Universal
