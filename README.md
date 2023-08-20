# Cool New GNU/Linux Apps

A list of cool new GNU/Linux apps.

Sure, you can stick to good old `find`, `sed`, `awk` and all those useful
utilities that have served us well so many years. If you're a sysadmin/devops or
a person who works with new machines all the time, you should stick to the
basis.

On the other hand, if you have full control of your set up and it doesn't change
regularly, maybe you should check this list of nice apps that sometimes bring
new functionality to the CLI, and on other cases expand, replace or ease old
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

- `locate` and `find` replacements:
  - [fzf](https://github.com/junegunn/fzf)
    CLI fuzz finder

  - [peco](https://github.com/peco/peco)
    CLI fuzz finder

  - [broot](https://github.com/Canop/broot)
    Search as-you-type files and folders. Press `ENTER` to launch associated
    viewer.

  - [fd](https://github.com/sharkdp/fd)
    Simple, fast and user-friendly alternative to find

  `fzf` and `peco` are more general utilities: basically you can pipe anything through them and use their features to search stuff.

- [diffoscope](https://diffoscope.org/)
  In-depth comparison of files, archives, and directories.

- [duf](https://github.com/muesli/duf) a replacement for `df`
  Colorfull output, arranged by type, and output JSON, and more.

- A couple of `du` replacements:
  - [ncdu](https://dev.yorhel.nl/ncdu)
    Provides an arrow-keys navigable interface.

  - [dust](https://github.com/bootandy/dust)
    Presents not only the raw information, but also a bar graph so you can visually see disk consumption.

- `top` replacements: (also see below the [Maybe unworthy](#maybe-unworthy) section)
  - [htop](https://htop.dev/)
    My go-to process lister for many years.

  - [btop](https://github.com/aristocratos/btop)
    Pretty cool: several display presets, highlighted hot-keys so you don't have to go to the help to recall how to use it, zoom into the information box you're more interested. The same author also built [bashtop](https://github.com/aristocratos/bashtop) and [bpytop](https://github.com/aristocratos/bpytop) which I didn't fully reviewed but seem to have the same set of features, only that `bashtop` is made in Bash, `bpytop` in Python and `btop` in C++.

  I'm an `htop` user, usually the only thing I want to look is which program is consuming all my CPU power or my RAM, so I don't think I'll be switching, however if I would, `btop` is the strongest candidate.

- `hexdump` replacement:
  - [hexyl](https://github.com/sharkdp/hexyl)
    Pretty cool: shows spaces and space-like characters in green, and more-than-one-byte unicode characters in yellow. Also shows the text version in a third column.

## Find & Replace

- [rg](https://github.com/BurntSushi/ripgrep) (aka ripgrep)
  A search tool that combines the usability of ag with the raw speed of grep.

  <details>
    <summary>Similar tools: `ag`, `ack`</summary>

    - [ag](https://github.com/ggreer/the_silver_searcher)
    - [ack](https://github.com/beyondgrep/ack3)

    Haven't tried any of those, I'm fine with ripgrep and didn't find any feature on those that made me want to try them.
  </details>

- [sd](https://github.com/chmln/sd)
  Intuitive find & replace CLI (sed alternative)

## Screen recording and alike

- [vhs](https://github.com/charmbracelet/vhs)
  Generates a GIF from a script. Useful to demo CLI tools.

## Git related

- [delta](https://github.com/dandavison/delta)
  A syntax-highlighting pager for git, diff, and grep output.

  <details>
    <summary>Similar tools: `diff-so-fancy`, `git-split-diffs`, `difftastic`</summary>

    I found `delta` better than:

    - [diff-so-fancy](https://github.com/so-fancy/diff-so-fancy)
    - [git-split-diffs](https://github.com/banga/git-split-diffs)
      This one [breaks my terminal](https://github.com/banga/git-split-diffs/issues/16)
    - [difft](https://github.com/Wilfred/difftastic) (aka difftastic)

  </details>

### Git <abbr title="User Interfaces">UIs</abbr>

**Untested, under review**

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
  for the [Maybe unworthy](#maybe-unworthy) section.

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

## Networking

- [sniffnet](https://github.com/GyulyVGC/sniffnet)
  Monitor your network traffic.

- [mosh](https://mosh.org/) an `ssh` replacement
  Several cool features, the main one: it stays connected.

## Markdown

- [glow](https://github.com/charmbracelet/glow)
  CLI markdown renderer and file navigator

- [typora](https://typora.io/)
  A minimal markdown editor and reader.

## Maybe unworthy

I put here commands that, in my humble opinion and for my use case, don't worth my time. As they don't add any significant improvement, new features or easyness compared to the usual old command. Having colors is cool, but redoing a whole application just to add some colors is... Unnecessary (to put it kindly).

- `ls` replacements:
  - [exa](https://the.exa.website/)
    Doesn't do anything useful that `ls` or `git status` doesn't already do.

  - [lsd](https://github.com/Peltoche/lsd)
    Doesn't do anything useful that `ls` doesn't already do. But looks cooler than `exa` to me.

- `cat` replacements:
  - [bat](https://github.com/sharkdp/bat)
    A cat clone with syntax highlighting and Git integration.

  - [most](https://www.jedsoft.org/most/index.html)
    This one's also colorful and can show images ANSI-converted.

    Besides syntax highlighting, I don't see real value to replace `cat`

- `dig` replacements:
  - [drill](https://www.nlnetlabs.nl/projects/ldns/about/)
    Utility from `ldns` C library.

  - [dog](https://github.com/ogham/dog)

    I don't do a heavy use of `dig`, so take this with a grain of salt: `drill` looks the same as `dig`, maybe its output a little bit different. `dog` on the other hand may be useful for scripting, as you can ask for specifics fields and also request the output in JSON.

- Other `top` replacements:
  - [glances](https://github.com/nicolargo/glances)
    Awful <abbr title="User Interface">UI</abbr>. Adds extra info `htop` doesn't have, but it's a nightmare to watch.

  - [zenith](https://github.com/bvaisvil/zenith)
    A little better than `glances`, but still far from the cool ones

  - [gtop](https://github.com/aksakalli/gtop)
    Smooth <abbr title="User Interface">UI</abbr>, but I think it wastes screen space with its memory, swap, disk usage, and network history boxes. Cause all of them use a big portion of the screen just to show a percentage. Also it doesn't show all my cores and the boxes are not real "windows" like in `bottom`.

  - [bottom](https://github.com/ClementTsang/bottom)
    Neat <abbr title="User Interface">UI</abbr> and also adds more information than `htop`, also can scroll over my CPU cores. However it didn't catch my eye.

- `traceroute` replacement:
  - [mtr](https://www.bitwizard.nl/mtr/)
    Didn't find it cool enough to replace good ol' `traceroute`.

- 'locate' replacement:
  - [plocate](https://plocate.sesse.net/)
    It claims to be faster, but I'm satisfied with `find`, `broot` or `fzf`.

- [fasd](https://github.com/clvv/fasd)
  A kind of command abbreviator, but I really didn't like the way it works. I prefer to be explicit in my command line. Also repo's currently (2023-08-19) archived without reason (I hate when they do that) and hasn't received any new commits since 2015. So totally unworthy, not maybe.

- `cd` replacements:
  - [z](https://github.com/rupa/z)
  - [zoxide](https://github.com/ajeetdsouza/zoxide)
  - [autojump](https://github.com/wting/autojump)

  None of these are my cup of tea. I don't like having to add folders into a database and I don't like writing obscure abbreviations on my command line. I'm fine working my way around pressing `TAB` key and autocompleting. If I'd expand `cd` functionality, I'll make it work like `fzf` or `broot`, greping through your folders and presenting the most likely one.

- `mc` replacements:
  - [nnn](https://github.com/jarun/nnn)
  - [ranger](https://github.com/ranger/ranger)

  I don't usually use file managers, and when I need some visual aid in my file navigation pursuits, I have more than enough with good ol' [Midnight Commander](https://midnight-commander.org/)

- [direnv](https://github.com/direnv/direnv)
  Yeah... I don't like this kind of magic. Loading environment variables when you require is just `. env-file`, so this is not worthy for me.

## References and similar works

While building this list I reviewed other people's work. Here are links to similar listings:

- Julia Evans's [List of Newish CLI tools](https://jvns.ca/blog/2022/04/12/a-list-of-new-ish--command-line-tools/)

- ibraheemdev's [Modern Unix Apps](https://github.com/ibraheemdev/modern-unix)

- Emre Sevinç's [CLI for the 21 Century](https://ileriseviye.wordpress.com/2018/10/30/command-line-for-the-21-century-the-low-hanging-fruit/amp/)
