# TF2 Single Key Trade Bind

This repo contains a simple script for TF2 that allows you to bind all of your trade messages to just one key.
With each press of your chosen key, the script will send one message from the cycle, repeating once it ends.

## Usage

1. Open trade_bind.cfg and edit the messages to your liking.
2. Edit the 'uparrow' in the last few lines to your chosen key. A full list of key names can be found [here](https://wiki.teamfortress.com/wiki/Scripting#List_of_key_names).
3. If you have more than the default 3 messages, make sure to edit the alias lines near the end of the file, like so:

```cfg
alias trade1 msg1; bind uparrow trade2
alias trade2 msg2; bind uparrow trade3
alias trade3 msg3; bind uparrow trade4
alias trade4 msg4; bind uparrow trade5
alias trade5 msg5; bind uparrow trade1
```

4. Once you are happy with your configuration, copy the contents of the file and paste them at the bottom of your `autoexec.cfg` file and save it.

* `autoexec.cfg` is located in `Steam\steamapps\common\Team Fortress 2\tf\cfg`.
* If you don't have an `autoexec.cfg` file, create one in this directory. Make sure the name is exact.

5. Launch TF2, or if run `exec autoexec` in the console if TF2 is already running.
6. Done!
