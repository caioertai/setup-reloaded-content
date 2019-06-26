## Common problems

### 1. `ssh-add` command not persisted

Added SSH key to ssh-agent using `ssh-add` command, but when student restarts the computer, it seems that the passphrase is not being stored into the ssh-agent, and the student needs to the run `ssh-add` again.

#### Possible solutions

- TO DO

### 2. Illegal option

When running `mkdir -p ~/.ssh && ssh-keygen -t ed25519 -o -a 100 -f ~/.ssh/id_ed25519 -C “TYPE_YOUR_EMAIL@HERE.com”`, the response is `illegal option --o` and then lists the available flags SSH keygen.

#### Possible solutions

Fallback to a [generic RSA key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

The computer might be having an old version of SSH and does not support the ed25519 protocol.
