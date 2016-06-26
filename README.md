<div align = "center">
<img src="https://github.com/RamonGilabert/Terminal/blob/master/Resources/header.png" />
</div>
# Theme

Hey there!

If you just want to install the theme of colors just download this repository and double click in the file `Gilabert.terminal`! That should open it and you'll have it there. :)

# Commands

I have some commands preinstalled that I'll keep pushing here as I have more, an example can be seen in this image, where I use the command `gcp`:

<div align = "center">
<img src="https://github.com/RamonGilabert/Terminal/blob/master/Resources/terminal.png" />
</div>

In order to do this I use the **[fish](https://fishshell.com)** shell.

With the fish shell, by simply editing the file located at `~/.config/fish`, you'll be able to enter your personal commands.

For instance to say hello to me I use:

```shell
set fish_greeting Welcome\x20\x1b\x5b32mRamon!
```

Or for some Git related stuff I use:

```shell
function gp
  set branch (git rev-parse --abbrev-ref HEAD)

  if test (echo $argv | wc -w) -ge 1
    git push -u origin $argv
  else
    git push -u origin $branch
  end
end

function gcp
  git add --all; git commit -m "$argv";gp
end
```

You can do much more stuff with it, like editing the prompt, add more commands, autocompletion, etc.

Finally, I use something to show the terminal with a command as it was a [curtain](https://github.com/RamonGilabert/Terminal/blob/master/Resources/curtain.png)! That is done with **[TotalTerminal](http://totalterminal.binaryage.com)** and even though it's not compatible with OS X 10.11, there are some tricks to make it work. Contact me if you want to learn more! :)

I'll tidy some of the commands I have and post it here once I have more! :)

# Contact

Don't hesitate to **[contact me](https://www.twitter.com/RamonGilabert)!**, I love to read tweets!
