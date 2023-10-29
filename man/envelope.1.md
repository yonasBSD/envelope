% envelope(1) v0.3.0

<!-- This is the envelope(1) man page, written in Markdown. -->
<!-- and the man page will appear in the ‘target’ directory. -->

NAME
====

envelope — a modern environment variables manager

SYNOPSIS
========

`envelope [command]`

*envelope* is a modern environment variables manager.

EXAMPLES
========

`cat .env | envelope`
: Pretty prints environment variables in the .env file

`envelope init`
: Creates and `.envelope` file in the current directory, needed by envelope to
store your enviroment variables

`envelope import dev .env`
: Imports variables from .env file into environment named 'dev'

`envelope list`
: Lists all enviroments in the tool

`envelope list dev`
: Lists all enviroment variables in the 'dev' enviroment

`envelope duplicate dev dev-local`
: Creates a new 'dev-local' environment with the same variables that are stored in 'dev'

`envelope check`
: Returns all the environments that are active by comparing active enviroment
varibles in the current process

EXIT STATUSES
=============

0
: If everything goes OK.

1
: If there was an I/O error during operation.

2
: If there was a problem with the command-line arguments.

AUTHOR
======

envelope is maintained by Mattia Righetti.

**Website:** `https://mattrighetti.com/` \
**Source code:** `https://github.com/mattrighetti/envelope`