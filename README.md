# cocoapods-githooks-demo

Demo project that shows how to integrate cocoapods-githooks plugin in your project and some practical usage of SwiftLint pre-commit git hook. 

## How to use

1. If you don't have 'cocoapods-githooks' plugin installed, run

```
$ gem install cocoapods-githooks
```

2. Checkout the project and run 

```
$ pod install 
```
 
3. Now you should see that git hooks from .git-hooks directory synchronized with git hooks in git repository (.git/hooks)

4. Try to make some changes in ViewController.swift and commit it. You should see SwiftLint validation warning. It happens because pre-commit git hook runs SwiftLint validation before commiting.

5. After fixing SwiftLint validation warnings you will be able to commit. 