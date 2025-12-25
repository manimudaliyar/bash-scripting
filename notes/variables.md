# Variables

A variable is used to store a value to use later.

<u>**Example:**</u> userName="Mani"

<u>**Important rules:**</u>

There must be no spaces around =
Variable names are case sensitive
Quotes are recommended for strings

## Using a variable

To use a variable, we have to call it using '$'

<u>**Example:**</u> echo $userName
Best practice: echo "$userName"

## Command Substitution in Bash

$(...) executes a command and substitutes it's output into a variable.

<u>**Example:**</u> files=$(ls) 

**In this example:**

The command ls is executed
Its output is captured
The output is stored in the variable files

<u>**Usage:**</u>

echo "$files"

<u>**Important notes:**</u>

Command substitution stores text output, not files
Output is subject to word splitting and newlines
Using ls in scripts is generally unsafe for filenames with spaces