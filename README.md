# Git Hooks

This repo shows how you can use Git Hooks in your project! Simply run `make hooks` in your repository (or without make, run: `git config --local core.hooksPath .githooks`). Add whatever checks you want to `.githooks/pre-commit` and `.githooks/pre-push` and have them execute automagically before committing and pushing!

## Recommended Hooks

I recommend at least the the following:

### Pre-Commit Recommendations

* Create a shell script that verifies you are not committing to the master branch

### Pre-Push Recommendations

* Run your formatting (cargo fmt, clang, eslint, etc...) and static analysis tools (clippy, cppcheck, etc...)
* Ensure your test suite completes with no errors 

## Screenshots 

![image](https://user-images.githubusercontent.com/36173115/132224379-b4fb2652-0e95-4a32-8638-b6ee45e48935.png)
