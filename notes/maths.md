# Arithmetic Using expr

expr is a command used to evaluate arithmetic expressions in Bash.

**Example:**

expr 10 + 20

**Important rules:**

Spaces around operators are mandatory
expr prints the result to standard output

**Using expr with variables**

**Example:**

a=10
b=20
expr $a + $b

**Store the result:**

result=$(expr $a + $b)

**Escaping wildcards**

Some operators have special meaning in Bash and must be escaped.

**Example:**

expr 10 \* 2

* is a wildcard and must be escaped using \.

**Important notes**

expr is an older command
Arithmetic expansion $(( )) is preferred in modern scripts