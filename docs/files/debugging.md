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

### Adding Breakpoints to Your Script
Instead of peppering your code with multiple `breakpoint()` functions, you can use VS Code's built in breakpoint feature. Navigate to the line number of your script where you want to place a breakpoint and hover over the line number. You should be able to see a red dot appear. Click to place a breakpoint and click again to remove a breakpoint.

![Imgur](https://i.imgur.com/ryh8b7f.png)

### Running Script in Debugging Mode

To run your script in debugging mode,
* Click the debug icon on the left most stripe and at the top bar, look for a green icon with `DEBUG` written beside it.

    ![Imgur](https://i.imgur.com/Aj7bDpA.png)

* Click on the `Add Configuaration` beside the `DEBUG` button and select `Python: Current File option.

  ![Imgur](https://i.imgur.com/2AMGs7B.png)

* Click on the green `DEBUG` button to run the script in debugging mode. Alternatively, you can just press `F5` to run the current script in debugging mode.

* When you run your script in debugging mode, it stops at the first breakpoint. VS Code highlights the active breakpoint.

    ![Imgur](https://i.imgur.com/z5EWV5M.png)

* The left panel of debugging model has Four panels
    * Variables: While running your script in debugging mode, you can click the dropdown on the variable panel and inspect the variables and their corresponding values.

        ![Imgur](https://i.imgur.com/0m1jWvZ.png)

    * Watch:
    * Callstack:
    * Breakpoints:

* Using the debug toolbar for inspecting code line by line
* Using the `DEBUG CONSOLE` for evaluating variables and more experimentation
