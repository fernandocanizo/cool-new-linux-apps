# Cool New GNU/Linux Apps

A list of cool new GNU/Linux apps.

Sure, you can stick to good old `find`, `sed`, `awk` and all those useful
utilities that have served us well so many years. If you're a sysadmin/devops or
a person who works with new machines all the time, you should stick to the
basis.

On the other hand, if you have full control of your set up and it doesn't change
regularly, maybe you should check this list of nice apps that sometimes bring
new functionality to the CLI, and on other cases expand or replace old
functionality.

I'll try to not spam with new stuff that may not really add anything useful to
my current workflow.

## Cheatsheets

- [cheat](https://github.com/cheat/cheat)
  `cheat` allows you to create and view interactive cheatsheets on the
  command-line. It was designed to help remind \*nix system administrators of
  options for commands that they use frequently, but not frequently enough to
  remember.

  There're already made [community sheets](https://github.com/cheat/cheatsheets).

- [tldr](https://github.com/tldr-pages/tldr-python-client)
  Python command-line client for [tldr pages](https://github.com/tldr-pages/tldr).

  In the same vein of `cheat`. Haven't used any of them enough to make a
  decision. So far I'm inclined for `cheat` because `cheat -l` shows all that's
  already saved, while `tldr -l` only shows commands I've already looked up and
  `tldr` has downloaded or somehow found the cheatsheet.

- [navi](https://github.com/denisidoro/navi)
  Looks more powerful than the previous, but I haven't tested it enough.

## Filesystem navigation and stuff

- [fzf](https://github.com/junegunn/fzf)
  CLI fuzz finder

- [broot](https://github.com/Canop/broot)
  Search as-you-type files and folders. Press `ENTER` to launch associated
  viewer.

  Haven't used it enough yet, but looks like it has several promising uses. I
  need to configure some keys that I have already mapped.

- [zoxide](https://github.com/ajeetdsouza/zoxide)
  A smarter cd command. Supports all major shells.

- [diffoscope](https://diffoscope.org/)
  In-depth comparison of files, archives, and directories.

## Find & Replace

- [rg](https://github.com/BurntSushi/ripgrep)
  A search tool that combines the usability of ag with the raw speed of grep.

- [sd](https://github.com/chmln/sd)
  Intuitive find & replace CLI (sed alternative)

- [fd](https://github.com/sharkdp/fd)
  Simple, fast and user-friendly alternative to find

## Git related

- [delta](https://github.com/dandavison/delta)
  A syntax-highlighting pager for git, diff, and grep output.

  I found it better than
  [diff-so-fancy](https://github.com/so-fancy/diff-so-fancy) and
  [git-split-diffs](https://github.com/banga/git-split-diffs). Also the second
  [breaks my terminal](https://github.com/banga/git-split-diffs/issues/16).


## Databases

- [pgcli](https://github.com/dbcli/pgcli)
  Great CLI tool to works with Postgresql databases. Check it's
  [site](https://www.pgcli.com/) too.

- [iredis](https://github.com/laixintao/iredis)
  Terminal client for Redis with auto-completion and syntax highlighting.


## Editing

- [vidir](https://joeyh.name/code/moreutils/)
  Allows to edit filenames from a folder with a vi-like UI.
  `vidir` is part of `moreutils` package, which have several other cool tools.


### Under review

I'm not fan of git UIs, but sometimes I use `gitg` to check the history. So
maybe these (`tig`, `gitui`, `lazygit`, `grv`) can make it into the usual apps
on my workflow.

- [grv](https://github.com/rgburke/grv)
  So far this is the one I like the most. But have to look into its feature set
  more closely to decide if it helps me or not.

- [tig](https://jonas.github.io/tig/)
  An ncurses-based text-mode interface for git. It functions mainly as a Git
  repository browser, but can also assist in staging changes for commit at chunk
  level and act as a pager for output from various Git commands.

- [gitui](https://github.com/extrawurst/gitui)
  Blazing fast terminal-ui for git written in rust.

  Claims to break `tig` and `lazygit` on being fast on big repos.

- [lazygit](https://github.com/jesseduffield/lazygit)
  I don't really like the motivations of the author. This is a serious candidate
  for the "Unworthy" section.

## JSON

- [gron](https://github.com/TomNomNom/gron)
  Transforms JSON into discrete assignments to make it easier to grep for what
  you want and see the absolute 'path' to it. It eases the exploration of APIs
  that return large blobs of JSON but have terrible documentation.

- [jq](https://stedolan.github.io/jq/)
  Command-line JSON processor.

- [jc](https://github.com/kellyjonbrazil/jc)
  CLI tool and python library that converts the output of popular command-line
  tools and file-types to JSON or Dictionaries. This allows piping of output to
  tools like jq and simplifying automation scripts.

- [jless](https://github.com/PaulJuliusMartinez/jless)
  A command-line pager for JSON data. Use it as a replacement for whatever
  combination of `less`, `jq`, `cat` and your editor you currently use for
  viewing JSON files.


## Requests / API exploration / Downloading

- [httpie](https://github.com/httpie/httpie)
  human-friendly CLI HTTP client for the API era

- [curlie](https://curlie.io)
  The power of curl, the ease of use of httpie.

## Markdown

- [glow](https://github.com/charmbracelet/glow)
  CLI markdown renderer and file navigator

- [typora](https://typora.io/)
  A minimal markdown editor and reader.

## To review

- [dog](https://github.com/ogham/dog)
  Command-line DNS client like dig.

  I don't do a heavy use of `dig`, so maybe this will stay here forever. From
  what I see in the README file, it seems its ability to output JSON may be the
  only distinctive feature that may stop me from putting under "Unworthy".

- [glances](https://github.com/nicolargo/glances)
  Glances an Eye on your system. A top/htop alternative for GNU/Linux, BSD, Mac
  OS and Windows operating systems.

  On a superficial review, I didn't see it better or clearer than `htop`. Also
  I'm not sure if it adds something. Strong candidate for the time being to
  become "Unworthy". Well, it has some extra information that `htop` doesn't
  have, like the "sensors", but I really didn't find it useful yet.

## Unworthy

Here I'll list new apps that claim to be cool but don't really add anything new.
You may choose to use them anyway... If you're a hipster :P

- [exa](https://the.exa.website/)
  Doesn't do anything useful that `ls` or `git status` doesn't already do.

- [lsd](https://github.com/Peltoche/lsd)
  Doesn't do anything useful that `ls` doesn't already do. But looks cooler than
  `exa` to me.

- [bat](https://github.com/sharkdp/bat)
  A cat clone with syntax highlighting and Git integration.

  Apart from syntax highlighting, I don't see real value to replace `cat`
