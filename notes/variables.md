# Variables

A variable is used to store a value to use later.

Example: userName="Mani"

Important rules:

There must be no spaces around =
Variable names are case sensitive
Quotes are recommended for strings

## Using a variable

To use a variable, we have to call it using '$'

Example: echo $userName
Best practice: echo "$userName"

## Command Substitution in Bash

$(...) executes a command and substitutes it's output into a variable.

Example: files=$(ls) 

In this example:

The command ls is executed
Its output is captured
The output is stored in the variable files

Usage:

echo "$files"

Important notes:

Command substitution stores text output, not files
Output is subject to word splitting and newlines
Using ls in scripts is generally unsafe for filenames with spaces