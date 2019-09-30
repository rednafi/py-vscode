# Settings

All your settings and preferences are kept in `settings.json` file. You can directly manipulate that file to set your preference locally or globally. Locally the settings file can be found in `.vscode/settings.json` folder in your current project location. To see the global `settings.json`, head over to `$HOME/.config/Code/User/settings.json` and open it in VS Code. If you haven't changed any of the default settings, the file should be empty or almost empty.


## Syncing Your Settings & Extensions
You don't want to set up VS Code from scratch every time you change your machine or do a fresh installation of your OS. In such scenarios, `Settings Sync` comes to rescue. You can set it up once, sync your settings and restore the settings with a few click. This will restore all of your settings, extensions, themes and other preferences. To do so,
* Search and install `Settings Sync` from the extension panel
* Login with your github credentials
* Press `ctrl+Shift+P` to open the command prompt and select `Sync: Update/Upload Settings` option to upload your settings and save to a github gist
* If you are restoring the settings to a freshly installed VS Code, just select `Sync:Download Settings` and you should see your VS Code getting restored


## Shut up & Let Me Replicate Your Settings

If you don't want to go through the hassle of manually installing all these extensions and like my settings. You can replicate my settings with the help of `Settings Sync` too. To do so:
* Go to the settings panel and search `setting sync`
* Find `Sync:Gist` option and replace it with `eec019bccd9c49388eaf9eeaf08c19ec` (This is the gist id of my settings)
* Then go to command prompt and select `Sync:Download Settings` option
* It will take some time to restore all the settings and you should see a setup similar to the following screenshots:

![Imgur](https://i.imgur.com/esscMKH.png)
![Imgur](https://i.imgur.com/TtYbXeI.png)




**P.S.:** This settings is a modified version of [Kenneth Reitz's](https://www.kennethreitz.org/) VS Code settings. Special thanks to him open sourcing that on twitter.

## Customizing the Settings According to Your Need

After you've synced the above settings, you can easily change the themes, font sizes according to your liking. However, if you want to sync the settings via `Settings Sync`, you have to change back the github gist id and replace that with your own id. To do so:

* Go go to [https://gist.github.com](https://gist.github.com) and find the gist name `cloudSettings`
* Check you url bar which should show something like this:
    ```
    git.github.com/<username>/gist_id
    ```
* Copy your own gist id and replace that in `Sync:Gist` (In settings)

Now you can customize the workspace with your heart's content and sync accordingly.

**A few Points to Note:**
If you have replicated my settings, you have to:
* Replace my github credentials with yours in the `settings.json` file
* Change and add your own `Flake8` and `Black` path for them to work (See it [here.](https://py-vscode.readthedocs.io/en/latest/files/linting.html#setting-up-linters-in-vs-code))
