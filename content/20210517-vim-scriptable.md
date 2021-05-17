# Vim is Scriptable
### qq more, literally

I have made an honest effort to start using other text editors for coding and other projects,
but I honestly can't get myself to stick with it and there's a glaring reason why.

Vim is the most scriptable text editor, and scripting is a powerful tool for working
with text, especially when you can visually watch it happen.

## The "Record command

If you open up vim and type the following

```
  :help record
```

It will pull up the help entry on "record".  This commands allows you to save a sequence of actions.
Now, other text editors may have macros, but it's generally pretty complicated, and you have to
learn a new system for transforming the text. Vim has been around forever, and

In vim, every action is already a command.

Initially it may seem like a downside, that you have to use commands to do everything, to move
between words, to cut and paste text, to even start typing, but because everything is a command
with the keyboard, it makes it so those commands can be recorded into a macro at any time.  You
don't even have to get complicated, if you know '0' for the start of line '$' for the end of line,
'w' for next word, or 'W' for next "full word", plus the basic "hjkl", then you can get started.

Simply press 'qq' and then start executing the sequence.  When you are done, press q again.
Now you can press '@q' to replay the sequence.  After replaying it once, you can simply
press a really quick '@@'.

My most common use case for this, is to combine it with the forward slash search '/pattern'
to do more complicated or nuanced line substitutions.  You can adjust indentation, change
line endings, all sorts of things, and do them one at a time.  It's extremely flexible and
useful.

This one command, despite all of the great things in vim, is the reason I use vim.  It's not
available anywhere else, because well, other text editors don't have command mode, and 
use the mouse, so it's just not possible.

## I still use the mouse in vim and gvim

Mice are great. As a minimalist, I wanted to migrate to another text editor, because vim
isn't really accessible to most people, even though I know it subconsciously at this point,
there's an argument to use tools that other people can use.  I think mice are a great tool.

You can use the mouse in many vim builds, at least for scrolling.  Gvim is nice, because
you can often drag and drop files from a file explorer to open them.  Graphical 
applications, imo, are simply a better way to browse filesystems.

But for text, scripting, and specifically macros, are king, and vim makes that easy in a way
no text editor can.
