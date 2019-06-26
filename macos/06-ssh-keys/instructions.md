## GitHub

> An SSH Key is a key that we generate for each device, that we'll be used to automatically authenticate you when using remote services, such as GitHub. Without SSH Key, you would need to enter your login and password each time you want to push code from your laptop to GitHub. With SSH Key, you authenticate once, and that's good.

So, here, we are going to generate an SSH Key for your laptop, and give that key to GitHub, to let it be able to know you when you want to push code from your laptop to GitHub without having to authenticate again. 🔑

Open a terminal and type this, **replacing the email with the email you used to sign up with GitHub**.

```bash
mkdir -p ~/.ssh && ssh-keygen -t ed25519 -o -a 100 -f ~/.ssh/id_ed25519 -C "TYPE_YOUR_EMAIL@HERE.com"
```

It will prompt for information. Just press enter until it asks for a **passphrase**. At that time, put something you want (and that you'll remember). It's like a password to protect your private key. As earlier, the characters that you're typing won't show up, and that's normal. When you're done, press `Enter`.

Now, your SSH Key is generated. We can show the public part (there is private part too) and copy / paste it to GitHub.

To show the public part, run

```bash
  cat ~/.ssh/id_ed25519.pub
```

It will prompt on the screen the content of the `id_ed25519.pub` file (which is the public part of the key).

**Copy that text**

Then go to [github.com/settings/ssh](https://github.com/settings/ssh). Click on add SSH key, fill in the title with your computer name, **and paste the key**.
Finish by clicking on the add key green button.

To check that this step is completed, in the terminal run

```bash
ssh -T git@github.com
```

You will be prompted a warning, type `yes` then `Enter`.

If you see something like this, you're done!

```bash
# Hi --------! You've successfully authenticated, but GitHub does not provide shell access
```

If it does not work, try running this before trying again the `ssh -T` command:

```bash
ssh-add ~/.ssh/id_ed25519
```

ℹ️ Don't be in a rush, take time to [read this article](http://sebastien.saunier.me/blog/2015/05/10/github-public-key-authentication.html) to get a better understanding of what those keys are used for.
