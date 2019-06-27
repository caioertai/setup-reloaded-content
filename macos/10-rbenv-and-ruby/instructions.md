# Installing Ruby (with [rbenv](https://github.com/sstephenson/rbenv))

> Ruby is the programming language that we choose to teach in Le Wagon. MacOS has ruby by default, but an old version. Also, developers want to have multiple versions of ruby on their laptop, because we usually work on severals different projects, which have different ruby version. To handle multiple ruby version, there is 2 tools : rbenv and rvm. We'll use rbenv.

We start by cleaning any version ruby that you might have, removing rbenv and rvm if it's already installed.

```bash
rvm implode && sudo rm -rf ~/.rvm
# If you got "zsh: command not found: rvm", carry on. It means `rvm` is not
# on your computer, that's what we want!

sudo rm -rf $HOME/.rbenv /usr/local/rbenv /opt/rbenv /usr/local/opt/rbenv
brew uninstall --force rbenv ruby-build
```

Now we're going to install [`rbenv`](https://github.com/rbenv/rbenv) and `ruby-build` using our beloved homebrew ;)

Then quit **all your opened terminal windows** (Cmd + Q) and restart one. Then run:

```bash
brew install rbenv ruby-build
```

Again, quit all your terminal windows and restart.

Now, rbenv is installed, and we'll use rbenv to install the last stable version of ruby (2.6.3).

Run this command, it will **take a while (5-10 minutes)**

```bash
  rbenv install 2.6.3
```

Since rbenv is able to manage multiple versions of ruby, it's better to set the default one that rbenv should use if it doesn't know which one should be used for a given project.

So, run

```bash
  rbenv global 2.6.3
```

Then **restart** your Terminal again (close it and reopen it).

```bash
  ruby -v
```

You should see something starting with `ruby 2.6.3p`. If not, ask a teacher.
