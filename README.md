Web Dev in Sublime-Text
================================

List all "must have" plugins or configuration for web dev in sublime text.

Sublime-Text can be call ST in the document below.

## Configure Sublime-Text

Each of these configurations below can be done either in `Preferences > Settings - User` or `Preferences > Settings - Default` depending on how you use ST.

### Set standard tabulations

```
// The number of spaces a tab is considered equal to
"tab_size": 4,

// Set to true to insert spaces when tab is pressed
"translate_tabs_to_spaces": true,
```

### Remove trailing white-space

ST can remove trailing white space on save.
Simply set `trim_trailing_white_space_on_save` to `true`

> "DEATH TO ALL WHITESPACE" - *An angry man*

## How to install packages

### DocBlockr - PHP Documentation

The DocBlockr plugin makes it very quick and easy to create doc blocks for your classes, attributes, and methods. It is available via Package Control.

To use it, open a new doc block as normal by typing `/**` and then pressing ENTER. The plugin will create a template doc block for you to fill out to suit.

### SublimeLinter - Real-Time Syntax Checking

SublimeLinter uses the ‘php -l’ command behind the screens – PHP’s built-in linter, and is simply reporting back exactly what the PHP runtime thinks is wrong.