dtc
===

Bash command to scan a directory for an expression.

In any directory, find where an expression occurs by calling

    dtc *expression*

from the command line. For example, to detect where your files contain "console.log", run

    dtc console.log

This will print the name of every file containing that expression followed by the line number of the occurence and the line itself.

To ignore a directory, add the "-not" flag.

    dtc console.log -not "node_modules"

For now you can only ignore one directory at a time. More to come!

===

To install, run

    curl https://raw.github.com/7imon7ays/dtc/master/lib >> ~/.bash_profile

Feel free to replace ".bash_profile" with any other bash configuration file.
