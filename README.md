# rake-completion.zshplugin

A rake task tab completion plugin for zsh, suitable for use with antigen. It was converted
from a blog post at the [Ruby on Rails](http://weblog.rubyonrails.org/2006/3/9/fast-rake-task-completion-for-zsh/) blog, but I wanted it in a zsh plugin so I could use it now that I've switched to antigen.

For speed, this caches the output for later usage in a .rake_tasks file in the
same directory as the Rakefile. If the Rakefile is newer than .rake_tasks, it will
rebuild the cache.

# How to install
Add a bundle entry to your .zshrc
```bash
antigen bundle unixorn/rake-completion.zshplugin
```
Add `.rake_tasks` to your [global .gitignore](https://help.github.com/articles/ignoring-files#global-gitignore)
