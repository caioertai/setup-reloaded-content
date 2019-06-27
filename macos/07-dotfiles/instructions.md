# Dotfiles (Standard configuration)

> Dotfiles are a set of files used to configure basic tools that we're using. Every developer has their own dotfiles, setting up their own plugins, keyboard shortcut, etc. We'll use standard dotfiles, that you will be able to update as much as you need.

We'll start with a great default configuration provided by [Le Wagon](http://github.com/lewagon/dotfiles), stored on GitHub.

As your configuration is personal, you need your own repository (a repository is like a folder on your github account where you can store files) to store it.

So we'll make you fork standard dotfiles of Le Wagon. The act of "forking" on GitHub is like cloning the content of a folder from a place to another. In this case, you'll clone the content of the folder `dotfiles` from Le Wagon to another folder dotfiles on your GitHub account.

👉🏻 [Click here to **fork**](https://github.com/lewagon/dotfiles/fork) the `lewagon/dotfiles` repository to your account. Forking means that it will create a new repo in your GitHub account, identical to the original one. You'll have a new repository on your GitHub account, `your_github_username/dotfiles`. We need to fork because each of you will need to put specific information (e.g. your name) in those files.

--------------------

Once your forked `dotfiles` on your GitHub account, we'll grab the content of the whole folder from GitHub to your laptop, and launch some scripts that will automatically install some plugins for zsh, some shortcuts to open sublime text, etc.

Open your terminal. **Don't blindly copy paste this line**, replace `replace_this_with_your_github_username` with *your*
own github username (not your email, your username).

`export GITHUB_USERNAME=replace_this_with_your_github_username`

Example: `export GITHUB_USERNAME=ssaunier`

Now copy/paste this very long line in your terminal. Do **not** change this one.

`mkdir -p ~/code/$GITHUB_USERNAME && cd $_ && git clone git@github.com:$GITHUB_USERNAME/dotfiles.git`

<script id="asciicast-ks0iILrMVv7kvmJ1STqKiwFWR" src="https://asciinema.org/a/ks0iILrMVv7kvmJ1STqKiwFWR.js" async></script>

After that, the content of the "dotfiles" folder should be present on your laptop. We now just have to launch 2 commands to configure zsh and git.

Run the `dotfiles` installer.

```bash
cd ~/code/$GITHUB_USERNAME/dotfiles
zsh install.sh
```

Then run the git installer:

```bash
cd ~/code/$GITHUB_USERNAME/dotfiles
zsh git_setup.sh
```

:point_up: This will **prompt** you for your name (`Firstname Lastname`) and your email.

Be careful, you **need** to put the **same** email as the one you sign up with on GitHub.

Please now **quit** all your opened terminal windows.
