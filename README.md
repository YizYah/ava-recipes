# ava-recipes README

A set of snippets intended for the free [crash course webinar](https://youtu.be/i0NsmEfn0XU) on unit testing  a node typescript application using ava.  Check out the [Repo for the class](https://github.com/YizYah/testingWebinar) which gives an explanation of all of the recipes.

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

1. **test** a basic test.  That's all you need for a public function.
2. **test-private** Sets up a test for a private function using rewire.
3. **test-no-content** The same as test, but without the result-is. Can be combined better private tests.

#### Stubbing

1. **stub** stub a public function.
2. **stub-private** stub a private function.

#### AVA specs for Typescript

For convenience, inside of a package.json the **ava** snippet will pop in recommended ava settings for a ts project.

## Limitations

These are not intended to be perfect, just to save some time.  You can expect to have to move things around in your test and make modifications at times.  What's intended here is a best guess at what you are likely to need.

## Release Notes

### 1.0.0

Initial release.
