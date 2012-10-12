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

```
"trim_trailing_white_space_on_save": true,
```

> "DEATH TO ALL WHITESPACE" - *An angry man*

### Unix line ending

```
"default_line_ending": "LF",
```

### Encoding

```
"default_encoding": "UTF-8",
```

## How to install packages

There are two ways to install ST plugins:

### Classic install

Download a plugins and copy it in `Preferences > Browse Packages ...` directory

### Install with package control (the best way)

Install the *wbond Sublime Package Control* plugin that provide a full-featured package manager that helps discovering, installing, updating and removing packages for Sublime Text 2. It features an automatic upgrader and supports GitHub, BitBucket and a full channel/repository system.

* Install the package control by coping these line into the console (View > Show console):
```
import urllib2,os; pf='Package Control.sublime-package'; ipp=sublime.installed_packages_path(); os.makedirs(ipp) if not os.path.exists(ipp) else None; urllib2.install_opener(urllib2.build_opener(urllib2.ProxyHandler())); open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read()); print 'Please restart Sublime Text to finish installation'
```

* Restart ST
* Now you can install plugins by typing `package install` in the command panel (ctrl+shift+p)

## Must have plugins

### SublimeCodeIntel - Code completion

Code intelligence plugin ported from Open Komodo Editor to Sublime Text 2.

Supports all the languages Komodo Editor supports for Code Intelligence (CIX, CodeIntel2):

    PHP, Python, RHTML, JavaScript, Smarty, Mason, Node.js, XBL, Tcl, HTML, HTML5, TemplateToolkit, XUL, Django, Perl, Ruby, Python3.

Provides the following features:

    Jump to Symbol Definition - Jump to the file and line of the definition of a symbol.
    Imports autocomplete - Shows autocomplete with the available modules/symbols in real time.
    Function Call tooltips - Displays information in the status bar about the working function.

### DocBlockr - PHP Documentation

The DocBlockr plugin makes it very quick and easy to create doc blocks for your classes, attributes, and methods. It is available via Package Control.

To use it, open a new doc block as normal by typing `/**` and then pressing ENTER. The plugin will create a template doc block for you to fill out to suit.

### SublimeLinter - Real-Time Syntax Checking

SublimeLinter uses the ‘php -l’ command behind the screens – PHP’s built-in linter, and is simply reporting back exactly what the PHP runtime thinks is wrong.

### Nettuts+ Fetch - Fetch remote files easily

Fetch latest version of remote files and zip packages.

* Just type `fetch` in the command panel (ctrl+shift+p) and select "Fetch: Manage remote files" to add your remote files.
* And now you can use the command Fetch. It will show you the list of files/packages to grab.

When you fetch a single file, the content of this file will be copied there your cursior is.

You can use this starting list of files [Nettuts+ Fetch base file] (https://github.com/devster/nettuts-fetch-base)

### AdvancedNewFile - Lightning Fast Folder and File Creation

Just hit `ctrl+alt+n` and see what happening

### PlainTasks - Pretty Task Management

See Nettuts video for more infos! -> https://tutsplus.com/lesson/pretty-task-management/

### HTTP Requester

Just copy an url and type `ctrl+alt+r`