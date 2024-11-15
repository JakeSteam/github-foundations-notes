https://learn.microsoft.com/en-us/training/modules/code-with-github-codespaces/

## Lifecycle

A codespace has 4 steps in its lifecycle:

1. **Creating**: Can be created from a template, branch, PR, etc.
   - Can have more than one per repo, or even per branch.
   - During creation, 4 processes occur:
     1. A virtual machine and storage are assigned to your Codespace.
     2. A container is created.
     3. A connection to the Codespace is made.
     4. A post-creation setup is made.
   - When accessing through the web, autosave is enabled.
2. **Rebuilding**: Typically only done when you've changed your Codespace's config, seems quite edge case. Some caching occurs.
3. **Stopping**: Codespaces time out after 30 mins of inactivity.
4. **Deleting**: Inactive Codespaces are deleted after 30 days (can be customised), and trying to delete any with unpushed / uncommitted changes will warn you.

## Customisation

Quoted verbatim:

> - Settings Sync: You can synchronize your Visual Studio Code (VS Code) settings between the desktop application and the VS Code web client.
> - Dotfiles: You can use a dotfiles repository to specify scripts, shell preferences, and other configurations.
> - Rename a Codespace: When you create a Codespace, an autogenerated display name is assigned to it. If you have multiple Codespaces, the display name helps you to differentiate between Codespaces. You can change the display name for your Codespace.
> - Change your shell: You can change your shell in a Codespace to keep the setup you're used to. When you're working in a Codespace, you can open a new terminal window with a shell of your choice, change your default shell for new terminal windows, or install a new shell. You can also use dotfiles to configure your shell.
> - Change the machine type: You can change the type of machine that's running your Codespace, so that you're using resources appropriate for the work you're doing.
> - Set the default editor: You can set your default editor for Codespaces in your personal settings page. Set your editor preference so that when you create a Codespace or open an existing Codespace, it opens to your default editor.
> - Visual Studio Code (desktop application)
> - Visual Studio Code (web client application)
> - JetBrains Gateway - for opening Codespaces in a JetBrains IDE
> - JupyterLab - the web interface for Project Jupyter
> - Set the default region: You can set your default region in the GitHub Codespaces profile settings page to personalize where your data is held.
> - Set the timeout: A Codespace will stop running after a period of inactivity. By default this period is 30 minutes, but you can specify a longer or shorter default timeout period in your personal settings on GitHub. The updated setting applies to any new Codespaces you create, or to existing Codespaces the next time you start them.
> - Configure automatic deletion: Inactive Codespaces are automatically deleted. You can choose how long your stopped Codespaces are retained, up to a maximum of 30 days.

## Codespaces vs GitHub.dev

It seems like GitHub have almost solved the same problem twice!

Essentially GitHub.dev is for basic file editing, it can't actually "run" anything (but can use some extensions), whereas Codespaces is a mini programming environment, complete with a terminal, most extnsions, a VM.

## Exercise

https://github.com/skills/code-with-codespaces

Interesting that you can run commands when Codespaces are triggered, and set default dot files across all your Codespaces.
