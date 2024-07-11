# Show git branch in your Ubuntu bash shell prompt by editing the PS1

What is PS1, you may ask? PS1 stands for "Prompt String 1". It's an environment variable that defines the primary prompt string in your shell. This is the prompt you see each time you're ready to type a command. It's a crucial part of customizing your shell prompt in Ubuntu (and other Unix-like systems).

A default PS1 looks something like this:
```
\u@\h:\w\$
```
Where:
- \u is the current usernae
- \h is the hostname
- \w is the current working directory
- $ is a $ for regular users, # for root.

### What to do...
Now we understand what we're working on, see the file `new_bashrc.sh` for the code.

You are to paste the code in your user home directory `~/.bashrc` file. But we will not only paste the code, we'll perform a few tweaks as well.

- Glance through your `~/.bashrc` file and within it find the portion of the code file (`new_bashrc.sh`) that reads "THE 6 LINES BELOW..."
- Once you've found it in your user home directory `~/.bashrc` file then comment it out.
- Paste the uncommented part of the code in `new_bashrc.sh` into your `~/.bashrc` file.
- source your `~/.bashrc` file to apply the changes in the shell. Use command:
```bash
source ~/.bashrc
```
- Now, you should be able to see your git branch name prepended in your shell prompt. Like so.
![show git branch in bash shell prompt](./show-git-branch-bash-sh-prompt.png)

Enjoy!

PS. You should know this solution causes some performance considerations. In large repositories, checking the git branch for every prompt can slow down your terminal. Some users opt for more optimized solutions or async prompts to mitigate this. Or they simply leave it as it came with Ubuntu (without seeing their git branch in shell prompt, unless they run `git branch` command in the terminal). Pick which works for you, but know the consequences.

Please raise an issue if you have questions. Thank you!
