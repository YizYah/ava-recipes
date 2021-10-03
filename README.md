# ava-recipes README

A set of snippets intended for the free [crash course webinar](https://youtu.be/i0NsmEfn0XU) on unit testing  a node typescript application using ava.  Check out the [Repo for the class](https://github.com/YizYah/testingWebinar) and its [wiki](https://github.com/YizYah/testingWebinar/wiki) which gives an explanation of all of the recipes.

It's intended for students there, but in truth it could be useful for anyone.

## Features

There are two sets of snippets for typescript test files:

1. For versions that insert as comments the step in a recipe, the prefix (what you have to type) starts with "learn".  For instance, `learn-throws-expect`.  The "learn" versions specify the step numbers for a given recipe as comments.
2. For any others, the prefix is just the name of the recipe.

Both do all of the Recipes below, except for the `test-no-content` which does not exist with a `learn` prefix.

### Recipes

#### Assertions

1. **result-is** sets a result constant and then asserts equality to something.
2. **throws-expect** sets an error constant and then asserts a regex match to the error message.

#### Testing

1. **new-normal-test** a basic sync test.  Set up with a default result-is.
2. **new-async-test** a basic async test. Set up with a default result-is.
3. **new-test-no-content** a basic test with no content added yet.  Lets you select normal or async.

#### Stubbing

1. **stub-constant** stub a function or other constant in the file to test.
2. **stub-private** stub an imported module in the file to test.

#### AVA specs for Typescript

For convenience, inside of a package.json the **ava** snippet will pop in recommended ava settings for a ts project.

## Limitations

These are not intended to be perfect, just to save some time.  You can expect to have to move things around in your test and make modifications at times.  What's intended here is a best guess at what you are likely to need.

## Release Notes

Check out the [Change Log](CHANGELOG.md)
