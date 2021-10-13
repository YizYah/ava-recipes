# ava-recipes README

A set of snippets intended for the free [crash course webinar](https://youtu.be/eqBW9q-KtVM) on unit testing  a node typescript application using ava.  Check out the [Repo for the class](https://github.com/YizYah/testingWebinar) and its [wiki](https://github.com/YizYah/testingWebinar/wiki) which gives an explanation of all of the recipes.

The goal of the Testing Recipes approach is to provide a simple yet robust and quick way of building tests.  Whether or not you use proper TDD, a test runner is a highly underutilized tool for confirming that new code is working as you develop it.  Part of the problem is confusion about the core concepts, which the webinar attempts to help.

To use them, you should at least check out the [wiki](https://github.com/YizYah/testingWebinar/wiki) mentioned above.
## Features

There are two sets of snippets for typescript test files:

1. For versions that insert as comments the step in a recipe, the prefix (what you have to type) starts with "learn".  For instance, `learn-throws-expect`.  The "learn" versions specify the step numbers for a given recipe as comments.
2. For any others, the prefix is normally just the name of the recipe. One exception is "new" instead of "test", 

Not every snippet has a `learn` version.

### Recipes

#### Assertions

1. **result-is** sets a result constant and then asserts equality to something.
2. **throws-expect** sets an error constant and then asserts a regex match to the error message.

#### Testing

1. **new-normal-test** a basic sync test.  Set up with a default 
2. **new-async-test** a basic async test. Set up with a default result-is.
3. **new-test-no-content** a basic test with no content added yet. Lets you select normal or async.

### Stubbing

**stub-constant** stub a function or other imported contant.

#### AVA specs for Typescript

For convenience, inside of a package.json the **ava** snippet will pop in recommended ava settings for a ts project.

## Limitations

These are not intended to be perfect, just to save some time.  You can expect to have to move things around in your test and make modifications at times.  What's intended here is a best guess at what you are likely to need.

It could be that if people like these we can develop a lot more.

Another limitation, but intentional, is that we sacrifice options for simplicity. The goal is that anyone can create robust tests with clarity from the beginning. So the recipes are intended to work all of the time, at the cost of not always being the ideal way to implement them.
* We don't use sinon for a lot of useful things such as spying.
* These snippets are only useful for testing public functions.  You can use a tool like rewire to test private functions, but then your tests will be brittle because if you refactor it may affect your tests.  One of the biggest gotchas for unit testing is overtesting and getting to a point where you are afraid to change things because you don't want to update your tests.  That is certainly not the goal!

## Release Notes

Check out the [Change Log](CHANGELOG.md)
