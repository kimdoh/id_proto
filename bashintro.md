If you visit the IP address associated with your instance, your web browser will report an error, as we have yet to install and setup web server software on the machine.

We'll need to access the machine to do so, and that requires a trip to your computer's terminal.

> On Macs or Linux machines, open `Terminal` from the Applications Folder. The directions will assume macOS from here on.

> On Windows, install [Cygwin](https://www.cygwin.com) and the [ssh daemon](http://www.howtogeek.com/howto/41560/how-to-get-ssh-command-line-access-to-windows-7-using-cygwin/)

The Terminal is a way of controlling your computer without any graphical user elements. You type in commands, and the machine responds with text back to you.

macOS uses a Terminal dialect called [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) which is derived from its Unix ancestry. The Bash language that we will be writing is [very concise](http://ss64.com/bash/).

After Terminal launches, it will present you with a prompt.

```
ComputerName:~ user$ 
```

After the `$` you can type in commands, for instance.

`echo hello`

Your computer will return

`hello`

The `echo` command is followed by a space and an `argument`. Spaces are semantic in Bash, and separate arguments from their inputs. Any argument that `echo` takes, it spits back out. Wrapping longer arguments in quotation marks ensures that the echo command speaks back all of its input.

 `echo "hello goodbye"`
 
Enter another Bash command 

`pwd` 

which returns something like

`/Users/zach`

`pwd` stands for 'print working directory,' and returns where your Bash shell is currently located in your computer's filesystem. Your Bash shell opens into your user home folder, which is often represented in Bash by the `~` (tilda) character.




 

