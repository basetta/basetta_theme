# Theme for Basetta's Website #
See [baseta.pupazzo.org](http://basetta.pupazzo.org) for a live demo.

It was inspired by [aijazansari.com](http://aijazansari.com/)

## How to install the theme
The theme is for the [Octopress](https://github.com/imathis/octopress) blogging
system.

### Download the theme

Dowload the [zip](https://github.com/basetta/basetta_theme/archive/master.zip) and unzip
in your `Octopress Folder/.themes`

### Add as git submodule

In your git octopress folder do the following:

```
~> git submodule add https://github.com/basetta/basetta_theme.git .themes/basetta_theme
~> git submodule update --init
```

### Install
You then need to tell Octopress to "use" the new theme.

```
~> rake install\[basetta_theme\]
```
On zsh shell those backslashes are required.

## Updating the Theme

### Git Submodule

```Shell
~> cd .themes/BlogTheme
git pull
~> cd ../..
~> rake update_source\[basetta_theme\]
~> rake update_style\[basetta_theme\]
```

Done, test it `rake generate && rake preview`.

### Manually Installed  Directory

1. [Download the [zip](https://github.com/basetta/basetta_theme/archive/master.zip)
2. Copy it into your `.themes` directory.
3. Update it

```Shell
~> rake update_source\[basetta_theme\]
~> rake update_style\[basetta_theme\]
```

Done, test it `rake generate && rake preview`.

## License
The theme is licensed under the "Simplified BSD license" (2-clause), for the exact terms please see the [_LICENSE_ file](https://github.com/rastersize/BlogTheme/blob/develop/LICENSE).bb