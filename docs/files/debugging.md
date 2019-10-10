# Debugging

VS Code makes python debugging a breeze. The simplest python debugging workflow usually consists of the following steps:

* Setting breakpoints at the points of interest
* Inspecting the variables
* Stepping through code

Let's dive in to see how these can be achieved in VS Code.

## Debugging via PDB (Python Debugger)

From python 3.7 you can just write `breakpoint()` in places where you want to stop your script for inspecting. You can add multiple breakpoints to cater your specific debugging needs. Adding necessary breakpoints and running the script (Ctrl+Atl+N) will open up the native Pdb (python debugger) in the integrated terminal. To inspect variables, just type the name of the variable in the Pdb prompt.

![Imgur](https://i.imgur.com/DEyLFS6.png)

Your script will stop at the first breakpoint. You can either comment and uncomment your breakpoints or you can use Pdb specific commands for moving around and doing granular debugging. Here is a list of a few commands that can be used to inspect code in the Pdb prompt:

* `l` : The list(l) command will show you the code line that the Python interpreter is currently on. If you want to navigate to different lines of your code, the `l` command takes line number as an argument. For example, writing something like `l 10` will take you to near the 10th line of your code.

    ![Imgur](https://i.imgur.com/FQMsAvQ.png)

* `u` & `d` : Up(p) and down(d) are the two commands needed to navigate through the call stack. This commands can show you who is calling the current function or why the interpreter is going this way.

* `s` & `n` : Step(s) and Next(n) help you continue the execution line by line. However, `n` command can't go outside of a function but `s` command can go deeper.

* `b` : Break(b) command can help you to add new breakpoints without changing the source code.

* `pp` : Pretty prints the value of an expression

* `q` : Quits(q) or exits the program.

* `r` : Continues the execution until the function returns.

## Using VS Code's Built in Debugger
