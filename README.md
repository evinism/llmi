# llmi

`llmi` is a speculative CLI for interacting with large language models 
through a CLI interface.

This is prospective interface!

## Basic Interactive Usage:

Prompting with the first argument for a question asks the question.

```
llmi "What do birds eat?"
Birds often eat seeds, berries, and many other things.
```

The raw command brings up a conversational agent in interactive mode.

```
$ llmi
>>> What is 4 + 6
Adding 4 and 6 results in 10
>>> Is that an even number?
Yes, 10 is divisible by 2 which makes it an even number.
```

This is an alias for `llmi -i`
```
$ llmi -i
>>> Are you a conversational agent?
Yes I am.
```

Piping a file into llmi produces a continuation on the file.

```
$ echo "It was a dark and stormy night." | llmi

The wind howled like [...]
```

Passing a question into the first argument initializes the 

```
$ llmi "how are you?"
I'm good thanks!
$
```

## Configuration
Configuration of `llmi` is done either by:
* Specifying an `.llmirc`
* running `llmi --configure`
