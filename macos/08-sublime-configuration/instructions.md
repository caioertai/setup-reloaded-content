# Sublime Text auto-configuration

> Sublime, as all text editors, are fully configurable. We can add some plugins to enhance capabilities of it. In the previous step, a file containing a list of plugin has been created for sublime.

Open a new terminal and type run

```bash
stt
```

It will **open Sublime Text in the context of your current folder**. That's how we'll use it.

**Close Sublime text** and open it again:

```bash
stt
```

**Wait 1 minute** for additional packages to be automatically installed (New tabs with text will automatically open, containing documentation for each new package installed). TO follow package installation, you can go to `View > Show console`.

To check if plugins are installed, open the Command Palette (`⌘` + `⇧` + `P`), type in `Packlist` and then `Enter`, you should see a couple of packages installed (like [Emmet](http://emmet.io/)).

If you don't, you can still install them manually. To do that, open Command Palette again (`⌘` + `⇧` + `P`), type `install package`, and then, one by one install :

* AdvancedNewFile
* All Autocomplete
* Babel
* Emmet
* ERB Snippets
* Git
* GitGutter
* SCSS
* SublimeLinter
* SublimeLinter-rubocop

When it's done, you can close Sublime Text.
