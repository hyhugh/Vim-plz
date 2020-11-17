# Hey Welcome

### A Vim Crash Course

# Overview

    - Vim 101
    - Cursor Movement
    - Basic Operations
    - Macros

## Vim 101

### What's that?

    - A very old and powerful editor
    - Not an IDE

## Vim 101

### Why VIM?

    - No need to move your hand when editing

## Vim 101

### Why VIM?

    - No need to move your hand when editing

   (You don't even need to move your hands to the arrow keys)


## Vim 101

### Modes
    Normal Mode
    - hjkl to move the cursor
    - the mode which you should stay in for most of the time

## Vim 101

### Modes
    Normal Mode

    Insert Mode
    - enter this mode only when you want to insert some text and exit ASAP
    - use <esc> <c-c> <c-[> or custom keybindings to exit insert mode


## Vim 101

### Modes
    Normal Mode
    Insert Mode

    Visual Mode
    - select things (when is this useful?)

## Vim 101

### Modes
    Normal Mode
    Visual Mode
    Insert Mode

    Replace Mode
    - replace things (useful when drawing)

## Vim 101

### Modes
    Normal Mode
    Visual Mode
    Insert Mode
    Replace Mode

    Ex Mode/Command Mode
    - ed -> sed -> ex -> vi -> vim

## Vim 101

### Modes
    *Normal Mode
    *Visual Mode
    *Insert Mode
    Replace Mode
    Ex Mode/Command Mode

    [*: most commonly used]

## Cursor Movement (in Normal mode)
    Character level navigation
        h -> left
        j -> down
        k -> up
        l -> right

     30 j -> go down 30 lines

## Cursor Movement (in Normal mode)
    Character level navigation
    Block level navigation
        w      -> word (naturally delimited)
        b      -> reverse w

        W      -> consecutive-sequence-of-characters
        B      -> reverse W

        e      -> end-of-word (naturally delimited)
        ge     -> reverse e

        E      -> end-of-consecutive-sequence-of-characters
        gE     -> reverse E

        { or } -> previous/next paragraph (empty line delimited)
        ( or ) -> previous/next sentence (naturally delimited: [. ! ?])

        0      -> beginning of line
        ^      -> first non-empty character of the line

        $      -> end of line
        g_     -> first non-empty character from the back of the line   

        %      -> ({Jump to matching} pair)


## Cursor Movement (in Normal mode)
    Character level navigation
    Block level navigation
    Page level navigation
        gg         -> beginning of the file
        G          -> end of the file

        <Ctrl-d/u> -> half page up/down
        <Ctrl-f/b> -> page up/down

        M          -> move cursor to the to the middle of the screen
        L          -> move cursor to the to the bottom of the screen
        H          -> move cursor to the to the top of the screen

        zz         -> move current line to the middle of the screen

## Cursor Movement (in Normal mode)
    Character level navigation
    Block level navigation
    Page level navigation
    Search navigation
        / -> search forward
        ? -> search backward

        * -> select current word and search forward
        # -> select current word and search backward

        f/t -> find/till in line

## Cursor Movement (in Normal mode)
    Character level navigation
    Block level navigation
    Page level navigation
    Search navigation
    Jump navigation
        <Ctrl-i> -> move cursor to the next loc in the jump list
        <Ctrl-o> -> move cursor to the prev loc in the jump list
        <Ctrl-^> -> switch between two recent files

## Basic Operations (in Normal mode)
    Mode switch to insert mode:
        i -> enter insert mode before current cursor block
        I -> enter insert mode at the beginning of the line
        a -> enter insert mode after current cursor block
        A -> enter insert mode at the end of the line
        o -> create a new line below and enter insert mode
        O -> create a new line above and enter insert mode

    Mode switch to visual mode:
        v -> enter visual mode

    Mode switch to replace mode:
        R -> enter replace mode

## Basic Operations (in Normal mode)
    Cut/Copy Paste: there is no deletion in normal mode
        x         -> cut a character
        s         -> cut a character and enter insert mode
        dd        -> cut a line
        yy        -> yank a line

        p         -> paste after cursor
        P         -> paste before cursor

## Basic Operations (in Normal mode)
    Cut/Copy Paste: there is no deletion in normal mode
        x         -> cut a character
        s         -> cut a character and enter insert mode
        dd        -> cut a line
        yy        -> yank a line

        d[action] -> cut by action
        c[action] -> cut by action and enter insert mode
        y[action] -> yank(copy) by action

        p         -> paste after cursor
        P         -> paste before cursor

    Text Objects
        w    -> word
        t    -> the text inside tag(xml tag)
        {or} -> the text inside {}
        (or) -> the text inside ()
        [or] -> the text inside []
        "    -> the text inside ""

    Text Object Operation Modifier
        a -> around
        i -> within

## Macros (in Normal mode)
    q[reg] -> record
    @[reg] -> replay

## Let's combine the things we just learnt

### Convert list of words to list of classes

### Add default constructor to list of files

## Quiz time: How to exit vim??

## Quiz time: How to exit vim??
<del>Press power button and hold for 5 seconds</del>

:q please

# The End

### Thanks!
