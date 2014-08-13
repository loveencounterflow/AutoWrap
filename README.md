Auto (Hard) Wrap for Sublime Text 2/3
====================
Automatic hard wrap when the cursor is beyond wrap width (default 80).  It is very useful for text documents.

![](https://raw.githubusercontent.com/randy3k/AutoWrap/master/screenshot.gif)

### Installation
[Package Control](http://wbond.net/sublime_packages/package_control)


### Usage

#### To toggle Auto Wrap
Type `Auto Wrap` in command palette or Go to menu `Edit -> Auto Wrap`.

#### Control wrap width

Wrap width is detected in the following order

1. `auto_wrap_width`
2. `wrap_width`
3. `rulers`
4. default 80

### Settings

#### To activate Auto Wrap for a specific syntax at start up

Put the following in your syntax specific preference.<br>
Menu -> Preference -> Settings - More -> Syntax Specific - User

    {
        "auto_wrap" : true
    }

#### You can also change `auto_wrap_width` by

    {
        "auto_wrap_width" : 100
    }

#### Long words

In default, long word will break into a new line.
To disable this behavior, consider

    {
        "auto_wrap_break_long_word" : false
    }

#### Punctuations

To avoid a punctuation mark at the wrap width to break alone, the following setting was used. You can change default setting below by adding more punctuation.

    {
        "auto_wrap_end_chars" : ",.?;:'\""
    }
