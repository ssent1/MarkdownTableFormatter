# Summary

query: [

    filenames: {
        [+] "MarkdownTableFormatter.sublime-settings >> tableMD.sublime-settings",
        [+] "mtf_show_off_small.gif >> tablemd.gif",
        [+] "markdown_table_formatter.py >> tablemd.py"
    },
    variables: {
        [✓] "Markdown Table Formatter >> tableMD",
        [✓] "MarkdownTableFormatter >> tableMD",
        [✓] "MarkdownTableFormat >> tableMD"
        [✓] "markdown_table_format >> tablemd_format"
    }
]

# Update filenames

query: {

        [✓] "MarkdownTableFormatter.sublime-settings >> tableMD.sublime-settings"
        [✓ "mtf_show_off_small.gif >> tablemd.gif",
        [✓ "markdown_table_formatter.py >> tablemd.py",
    }

# Update variables

query: [{

        [✓] "Markdown Table Formatter >> tableMD",

```
Searching 17 files for "Markdown Table Formatter" (regex)

/Users/syd/Code/MarkdownTableFormatter/Commands.sublime-commands:
    1  [
    2   {
    3:      "caption": "Markdown Table Formatter: Format Table",
    4       "command": "markdown_table_format"
    5      }

/Users/syd/Code/MarkdownTableFormatter/Main.sublime-menu:
    7               [
    8                   {
    9:                      "caption": "Markdown Table Formatter",
   10                       "command": "markdown_table_format"
   11                   }
   ..
   25                           [
   26                                   {
   27:                                          "caption": "Markdown Table Formatter",
   28                                           "children":
   29                                           [
   30                                                   {
   31                                                       "command": "edit_settings",
   32:                                                      "args": { "base_file": "${packages}/Markdown Table Formatter/tableMD.sublime-settings" },
   33                                                       "caption": "Settings"
   34                                                   },
   ..
   37                                                       "command": "open_file",
   38                                                       "args": {
   39:                                                              "file": "${packages}/Markdown Table Formatter/Default (OSX).sublime-keymap",
   40                                                               "platform": "OSX"
   41                                                       },
   ..
   45                                                       "command": "open_file",
   46                                                       "args": {
   47:                                                              "file": "${packages}/Markdown Table Formatter/Default (Linux).sublime-keymap",
   48                                                               "platform": "Linux"
   49                                                       },
   ..
   53                                                       "command": "open_file",
   54                                                       "args": {
   55:                                                              "file": "${packages}/Markdown Table Formatter/Default (Windows).sublime-keymap",
   56                                                               "platform": "Windows"
   57                                                       },

7 matches across 2 files

```


        [✓] "MarkdownTableFormatter >> tableMD",

```
Searching 2 files for "MarkdownTableFormatter" (regex)

/Users/syd/Code/MarkdownTableFormatter/Main.sublime-menu:
   30                                                   {
   31                                                       "command": "edit_settings",
   32:                                                      "args": { "base_file": "${packages}/Markdown Table Formatter/MarkdownTableFormatter.sublime-settings" },
   33                                                       "caption": "Settings"
   34                                                   },

/Users/syd/Code/MarkdownTableFormatter/markdown_table_formatter.py:
   16          logging.basicConfig(level=logging.DEBUG)
   17          settings = \
   18:             sublime.load_settings("MarkdownTableFormatter.sublime-settings")
   19          verbose = settings.get("verbose")
   20          margin = settings.get("margin")
   ..
   83  
   84  
   85: class MarkdownTableFormatterListener(sublime_plugin.EventListener):
   86      def on_pre_save(self, view):
   87          # restrict to markdown files
   ..
   90  
   91          settings = \
   92:             sublime.load_settings("MarkdownTableFormatter.sublime-settings")
   93          if not settings.get("autoformat_on_save"):
   94              return

4 matches across 2 files

```

        [✓] "markdown_table_format >> tablemd_format"


```
Searching 17 files for "markdown_table_format" (regex)

/Users/syd/Code/MarkdownTableFormatter/Commands.sublime-commands:
    2   {
    3       "caption": "tableMD: Format Table",
    4:      "command": "markdown_table_format"
    5      }
    6  ]

/Users/syd/Code/MarkdownTableFormatter/Default (Linux).sublime-keymap:
    2      {
    3          "keys": ["ctrl+alt+shift+t"],
    4:         "command": "markdown_table_format",
    5          "context": [
    6               {"key": "selector", "operator": "equal", "operand": "text.html.markdown"}

/Users/syd/Code/MarkdownTableFormatter/Default (OSX).sublime-keymap:
    2      {
    3          "keys": ["ctrl+alt+shift+t"],
    4:         "command": "markdown_table_format",
    5          "context": [
    6               {"key": "selector", "operator": "equal", "operand": "text.html.markdown"}

/Users/syd/Code/MarkdownTableFormatter/Default (Windows).sublime-keymap:
    2      {
    3          "keys": ["ctrl+alt+shift+t"],
    4:         "command": "markdown_table_format",
    5          "context": [
    6               {"key": "selector", "operator": "equal", "operand": "text.html.markdown"}

/Users/syd/Code/MarkdownTableFormatter/Main.sublime-menu:
    8                   {
    9                       "caption": "tableMD",
   10:                      "command": "markdown_table_format"
   11                   }
   12               ]

/Users/syd/Code/MarkdownTableFormatter/tablemd.py:
   93          if not settings.get("autoformat_on_save"):
   94              return
   95:         view.run_command("markdown_table_format", {"format_all": True})
   96  

6 matches across 6 files
```

```
Searching 17 files for "MarkdownTableFormatter" (regex)

/Users/syd/Code/MarkdownTableFormatter/Main.sublime-menu:
   30                                                   {
   31                                                       "command": "edit_settings",
   32:                                                      "args": { "base_file": "${packages}/Markdown Table Formatter/MarkdownTableFormatter.sublime-settings" },
   33                                                       "caption": "Settings"
   34                                                   },

/Users/syd/Code/MarkdownTableFormatter/markdown_table_formatter.py:
   16          logging.basicConfig(level=logging.DEBUG)
   17          settings = \
   18:             sublime.load_settings("MarkdownTableFormatter.sublime-settings")
   19          verbose = settings.get("verbose")
   20          margin = settings.get("margin")
   ..
   83  
   84  
   85: class MarkdownTableFormatterListener(sublime_plugin.EventListener):
   86      def on_pre_save(self, view):
   87          # restrict to markdown files
   ..
   90  
   91          settings = \
   92:             sublime.load_settings("MarkdownTableFormatter.sublime-settings")
   93          if not settings.get("autoformat_on_save"):
   94              return

/Users/syd/Code/MarkdownTableFormatter/README.md:
   31  
   32  ### CHANGES
   33: 1. Incorporates [code](https://github.com/bitwiser73/MarkdownTableFormatter/pull/17/files/) from [@sspkmnd](https://github.com/sspkmnd).
   34  2. File Δ {`tests/test.py`, `tests/test.md`, and `simple_markdown/table.py`}.
   35  3. Name Δ to `tableMD` to avoid conflict with simultaneously testing both versions; plus it's kinda nerdishly cool. Table + Markdown + M.D. (Doctor of Medicine). Plus, since it's been a long time since the original has received any love, if skill and passion rise to the level of voluteering to taking it to the next level, it may require updated branding.
   ..
   37  # Markdown Table Formatter 1.0
   38  
   39: [![travis][img-travis]](https://travis-ci.org/bitwiser73/MarkdownTableFormatter) [![MIT licensed][img-mit]](./LICENSE) [![Donate][img-paypal]][donate-paypal]
   40  
   41  Sublime Text 3 markdown plugin that offers table formatting.
   ..
   43  Inspired by the [Atom's version](https://atom.io/packages/markdown-table-formatter) from fcrespo82 (Fernando).
   44  
   45: markdowntableformatter[at]gmail[.]com
   46  
   47  ![Example](mtf_show_off_small.gif)
   ..
   93  
   94  [donate-paypal]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=WAQUTBM9K8246
   95: [img-travis]: https://travis-ci.org/bitwiser73/MarkdownTableFormatter.svg?branch=master
   96  [img-mit]: https://img.shields.io/badge/license-MIT-blue.svg
   97  [img-paypal]: https://img.shields.io/badge/Donate-PayPal-blue.svg

8 matches across 3 files

    },
    { [] "MarkdownTableFormat >> tableMD"


```
Searching 17 files for "MarkdownTableFormat" (regex)

/Users/syd/Code/MarkdownTableFormatter/tablemd.py:
   12  
   13  
   14: class MarkdownTableFormatCommand(sublime_plugin.TextCommand):
   15      def run(self, edit, format_all=False):
   16          logging.basicConfig(level=logging.DEBUG)

1 matches across 1 files
}
]
