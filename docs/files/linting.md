# Linting & Formatting
Linters perform static analysis of source codes and check for symantic discrepancies. When you lint your code, it's passed through a basic quality checking tool that provides instructions on how eliminate basic syntactic inconsistencies.

Formatters are similar tools that tries to restructure your code spacing, line length, argument positioning etc to ensure that your code looks consistent across different files or projects.

Python offers you a plethora of linters and formatters to choose from. Flake8, pyflakes, pycodestyle, pylint are some of the more widely used linters and black, yapf are two newer members in the code formatting space.
However, not to bombard you with a deluge of information, we are taking an opinionated route that gets the job done without a hitch. Let's talk about `Flake8` and `Black`.


## Flake8
Flake8 is a Python linting library that basically wraps three other linters, **PyFlakes**, **pycodestyle** and **Ned Batchelder's McCabe** Script. It's one of the better linters out there that has very low false positive rate.
It checks your code base against [PEP8](https://www.python.org/dev/peps/pep-0008/) programming style, programming errors (like “library imported but unused” and “Undefined name”) and [cyclomatic complexity](https://en.wikipedia.org/wiki/Cyclomatic_complexity).

![Imgur](https://imgur.com/wmhZevQ.png)

For more details on the nitty gritties of flake8, check out their github project [here.](https://github.com/PyCQA/flake8)


## Black
Black is known as the uncompromised Python code formatter. Unlike flake8 or pycodestyle, it doesn't nag you when there are style inconsistencies. It just fixes them for you. Black does not have a lot of options to tinker with and has a lot of opinion on how your code should look and feel. You might not always agree with the decisions that black takes for you but if you can get along with the style that black imposes on you, it can take care of the unnecessary hassles of formatting your codes to keep it conistent across multiple projects or organization.


![Imgur](https://imgur.com/b272FI5.png)
*Before formatting with black*


![Imgur](https://imgur.com/MqoKcqQ.png)
*After formatting with black*

## Setting Up Linters in VS Code
Luckily VS Code comes with both `flake8` and `black` formatter lurking in the settings. To set them up:

* Press `ctrl+,` to fire up the settings panel
* Search for `flake8` in the search panel
* Enable the option `Python>Linting:Flake8 Enabled`
* Search for black and select `black` from the dropdown called `Python>Formatting:Provider`

Doing the above will set `flake8` and `black` to lint and format your script on a project basis. You have to install `flake8` and `black` in your environment via `pip install flake8` and `pip install black` respectively. If you want to set them up globally and don't want to worry about formatting ever again, you have set up their global paths. To do so:

* Deactivate your environment
* Install `flake8` and `black` globally via `pip3 install flake8` and `pip3 install black`
* On the terminal write `whereis flake8` and `whereis black`
* You should see their global paths
    ![Imgur](https://i.imgur.com/mCyXVlj.png)
    
* Now go to the `settings` and search for `flake8` and paste your `flake8` path in `Python › Linting: Flake8 Path` option
    ![Imgur](https://i.imgur.com/YGceReL.png)
* Copy `black` path and paste them in `Python › Formatting: Black Path` option
    ![Imgur](https://i.imgur.com/Q8tX7Ro.png)
