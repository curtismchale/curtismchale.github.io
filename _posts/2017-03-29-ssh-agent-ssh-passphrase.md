It's tiring to **continually** get asked for your SSH passphrase for every operation you do with SSH. But as with everything security related, you're making a tradeoff between ease of use and security.

To that end I choose to use `ssh-agent` to handle my ssh key passphrases. You can add your passphrase to `ssh-agent` by typing `ssh-add` in your terminal. You should be prompted for your passphrase now so enter it.

After this, you'll need to enter your passphrase at the beginning of a terminal session, but not again till you start a new terminal session.

If you'd rather fall on the ease of use side then you should look at [Debian keychain](https://tracker.debian.org/pkg/keychain). By using this and giving it your passphrase for your ssh keys you no longer need to enter them every time you start a new terminal session.

That does mean that anyone who has your computer automatically has access to your ssh keys from the terminal. If someone has physical access to your computer then all bets are off, so the tradeoff doesn't seem to big a deal to me.
