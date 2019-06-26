## Homebrew

> [Homebrew](http://brew.sh/) is an app store without visual interface. We interact with it only with command line in the terminal. We can download and install programs in a easy and quick way. Homebrew only exists for Mac 🍏. We call such a thing a **package manager**. All the programs that we download and install via homebrew doesn't have visual interface, so we'll interact with them using terminal.

Open your terminal and run

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

This will ask for your confirmation (hit `Enter`) and your laptop session password.

Once done, homebrew is installed 💪

We'll now install some useful software, using homebrew ;)

Run in the terminal

```bash
brew update
```

This will tell to homebrew to update its "catalog" of programs

Then, we'll install
 * `git`, that will let us to save code on our laptop and push it to GitHub
 * `wget`, that is a program that let us download files from terminal
 * `imagemagick`, which is a program to transform images (crop, resize, etc.)
 * `jq` (we'll see that later in the bootcamp for the usefulness)
 * `openssl`, which is used for example when you pay something on internet with your credit card number, openssl is used to encrypt / decrypt data to secure the data transmission)

You need to install all those things one by one

⚠️ A lot of lines will be printed on your terminal, check as much as you can that there is no error (look for the `ERROR` keyword). If you have any doubt, call a teacher.

```bash
brew install "git"
```

```bash
brew install "wget"
```

```bash
brew install "imagemagick"
```

```bash
brew install "jq"
```

```bash
brew install "openssl"
```
