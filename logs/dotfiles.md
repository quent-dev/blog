# dotfiles

As I have been starting to customize my ArchLinux and Neovim config, I have started to understand the importance of maintaining your config files and having a way to replicate and deploy them on another machine if needed.

As I am trying to use Neovim as my daily text editor, I had to face a challenge:

My daily driver for work is actually running on Windows 11 and I can't switch the OS there yet for a couple of reasons:

- I am not fully proficient in ArchLinux yet to be able to be comfortable using it for work yet.
- Even though most of my work is done in a browser (Gmail + GDrive, a little bit of Excel sometimes, some Acrobat Reader for PDF editing), I just don't want to impact my work yet by taking that big a leap of faith
- I could technically do a dual boot and not impact my workflow too much, might end up doing it later this year.

Anyway, I decided to install WSL2 + Neovim on my work computer to be able to use Neovim as my sole text editor across all machines and perfect my skills.

The problem I realized today is that stock Nvim is very ugly and not appealing to work on. I also will spend most of my time working on Markdown files for note taking and it is not the most enjoyable Markdown editor out of the shelf.

So I decided to save my dotfiles on my Github to be able to install the same config on my work computer.

As I was thinking about how to track your .config folder in Git without adding too many files/ only adding what you really want to upload, I ended up on this [Hacker News article](https://news.ycombinator.com/item?id=11071754) with an elegant solution, and one user actually detailed the steps really clearly in his [repo README](https://github.com/Siilwyn/my-dotfiles/tree/master/.my-dotfiles)

I will try to explain the solution (the article will do a way better job of explaining it than me, a noob in git), but here is my [repo](https://github.com/quent-dev/dotfiles) after using this method.
