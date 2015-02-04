## Code Review
Code review is great in concept but what is it?

- A lookover from my lead developer before the code reaches develop.
...what if they're busy? Why only share code with one person? Are you going to be able to refactor from scratch if there's a serious flaw?

## Paired Programming
Four eyes are better than two. Wear glasses.

Traditional paired programming has two roles:
- the **driver** codes as normal
- the **observer** continually assesses the code the driver does, providing direct feedback.

The developers should be switching roles fairly regularly.

### How to be an observer
The observer isn't looking to simply 'correct' the driver, though this is obviously a good point to provide feedback. The driver should be aware when the observer isn't sure what the driver is attempting to achieve with a section of code. Ask questions, big or small.

It's rubber duck debugging, with a very loud and nosey duck.

# Static Code Analysis

Automated tooling can often find inconsistencies in code at a syntax level, allowing us as developers to focus on inspecting the structure & logic of our code.

We have the tools to do this - but need to do it manually for now.
Git Precommit Hooks will make these integral parts of review a crucial part of the developer workflow.

## David, PHPCS is returning too many errors!

Yep, and that's why we need to start doing this now. We don't need to fix all the errors in the next .module file we open, we just need to make sure that we don't add any more, and if we feel nice, fix a few errors. There's usually a "badly formatted" comment PHPCS is complaining about, fixing a few of those will make sure we get to the important issues.

---

"If they're used, they should be integrated into the build process, otherwise they will be ignored." - http://stackoverflow.com/users/2603/aaron-maenpaa. Thanks, StackOverflow!