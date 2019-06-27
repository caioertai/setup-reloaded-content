# Oh-my-zsh - Fancy your Terminal

> Unix based operating system (such as Linux, Ubuntu, Mac OS, etc.) have all by default a terminal. A terminal is just a text shell where we can run command. In fact, the whole Visual Interface of your OS is just an abstraction of the terminal. When you double click on chrome for example, your OS launch a command in the terminal to launch chrome. Then, if you know the commands, you can launch programs without interacting with your OS graphical interface. By default, the terminal of MacOS is not customizable enough for us, then we'll use oh-my-zsh as the default terminal. We call it `zsh`

To install it, run this command in the terminal

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

⚠️ At the end of this script, it will prompt for your laptop password again. You have to write it correctly (**you will not see it when you type, it's normal**) and hit `Enter`. You should get something like:

```bash
         __                                     __
  ____  / /_     ____ ___  __  __   ____  _____/ /_
 / __ \/ __ \   / __ `__ \/ / / /  /_  / / ___/ __ \
/ /_/ / / / /  / / / / / / /_/ /    / /_(__  ) / / /
\____/_/ /_/  /_/ /_/ /_/\__, /    /___/____/_/ /_/
                        /____/                       ....is now installed!
```

👉🏻 Now **quit the Terminal** (`⌘` + `Q`), and restart it.

You should see something like this
![](https://raw.githubusercontent.com/kevcha/setup-reloaded-content/master/images/on-my-zsh.png)
If not, **stop right away** and call a teacher.

Once zsh is installed, we are going to customize a little bit it :

Open `Terminal > Preferences` and set the "Pro" theme as default in `Profiles` (*`Réglages`* in French).

![](https://raw.githubusercontent.com/kevcha/setup-reloaded-content/master/images/terminal-pro.png)

**Quit and relaunch the Terminal again**. It should now have a nice black background, more easy on the eyes. 🚀

You now have a powerful terminal, and we'll soon (in 2 steps) enhance it with plugins 💪
