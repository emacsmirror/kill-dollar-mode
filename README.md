# kill-dollar-mode

Remove leading `$` from shell-script-like text in documentation.

## Motivation

It's common to see documentation that describes how to run commands in a shell
formatted with `$` at the beginining of the line to represent the prompt:

``` shell
$ pwd
```

This minor mode removes the leading `$` and surrounding whitespace from the
text in the kill ring, so when yanked into a shell, it can be executed.

In the example above, if the line of code were killed and yanked, the yanked
text would be `pwd`.
