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

After the `$` you can type in commands and then hit `enter`, for instance.

`echo hello`

Your computer will return

`hello`

The `echo` command is followed by a space and an `argument`. Spaces are semantic in Bash, and separate arguments from their inputs. Any argument that `echo` takes, it spits back out. Wrapping longer arguments in quotation marks ensures that the echo command speaks back all of its input.

 `echo "hello goodbye"`
 `hello goodbye`
 
-----
 
Enter another Bash command 

`pwd` 

which returns something like

`/Users/zach`

`pwd` stands for 'print working directory,' and returns where your Bash shell is currently located in your computer's filesystem. Your Bash shell opens into your user home directory, which is often represented in Bash by the `~` (tilda) character. This is why your prompt includes the tilda character, it is showing you where you are currently located.

`ComputerName:~ user$ `

-----

We can see what is in the current working directory with `ls`.

`ls`

```
Applications
Desktop
Documents
Downloads
Library
Movies
Music
Pictures
```

-----

We can also maneuver around the file system `cd`, abbreviated from 'change directory.'

`cd Applications`

Typing the first few letters of where you want to go is usually enough, as the `tab` key will autocomplete. Note that Bash is case-sensitive.

`cd De` will autocomplete to `cd Desktop/` if you hit `tab`. You need to include the lowercase 'e' to disambiguate, as just capital letter 'D' would match `Desktop`, `Documents`, and `Downloads`.

Your prompt will update.

`ComputerName:Desktop user$` 

And then you can see the contents of your [presumably messy] Desktop with `ls`.

```
Untitled1.ai
Untitled1_Final.ai
Untitled1_Final_FINAL.ai
Untitled1_REALLY_FINAL.ai
Untitled3.ai
```

-----

We can make a folder in the working directory with `mkdir`.

`mkdir testing`

We can see the results with

`ls`

```
testing
Untitled1.ai
Untitled1_Final.ai
Untitled1_Final_FINAL.ai
Untitled1_REALLY_FINAL.ai
Untitled3.ai
```

-----

Change your working directory into this newly created folder

`cd testing/`

We can make a file in the working directory with `touch`.

`touch text.txt`

`ls` should return

`text.txt`

And we can remove files with `rm`.

`rm text.txt`

Use `ls` to ensure it is removed. Note that files are removed immediately, no 'empty trash' required!

-----

Use the `>` character to redirect output.