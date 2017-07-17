---
title: "Running and Quitting"
teaching: 15
exercises: 0
questions:
- "How can I run Python programs?"
objectives:
- "Launch the Python shell."
- "Launch the IPython shell."
- "Launch IDLE in interactive mode."
- "Launch IDLE, create a Python script, and run it."
keypoints:
- "`python`, `ipython` and `idle` commands all give an interactive Python shell (REPL)."
- "Python programs are plain text files."
- "You can use IDLE for creating and editing Python programs."
---
## Setup
*   Obtain an interactive session on the HPC cluster:
    ~~~
    qsub -X -I -q workshop -l walltime=8:00:00 -l ncpus=1 -l mem=1G
    ~~~
*   Once you're in, load the latest Python 3 environment:
    ~~~
    module load python/3.6.1
    ~~~

## Evaluate Python statements interactively
    
### With vanilla Python shell
*   Type `python` to invoke the Python shell. This is also known as a "Read-Evaluate-Print Loop" or REPL.
*   Try the following commands:
    ~~~ 
    print("hi there!")
    2 + 2
    exit()
    ~~~
    {: .python}

### With enhanced IPython shell
*   Type `ipython` to invoke IPython, an ''enhanced'' interactive shell.
*   Repeat the commands above.

### With IDLE
*   Type `idle` to invoke the Python Integrated Development and Learning Environment in interactive (shell) mode.
*   Repeat the commands above.

## Python programs are plain text files.

*   They have the `.py` extension to let everyone (including the operating system) 
    know it is a Python program. This is convention, not a requirement.
*   It's common to write them using a text editor but we are going to use [IDLE](https://docs.python.org/3/library/idle.html)
*   IDLE is an example of an Interactive Development Environment, or IDE, that provides code completion and other helpful features.

## Use IDLE for editing and running Python.

*   Type `idle my_script.py` to invoke IDLE in edit mode.
*   This will start IDLE as an editor, with `my_script.py` as the open file.
*   Paste the same three commands into the editor.
*   In the File menu, select `Save` (or Ctrl+S)
*   In the Run menu, select `Run Module` (or F5)

[ipython]: https://ipython.org/
[idle]: https://docs.python.org/3/library/idle.html
