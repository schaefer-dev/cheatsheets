# nice Latex Stuff
    ysiw$ - in Wort mit Dollar ummanteln

# Verbs / Operations
    d - delete
    c - change
    y - yank
    v - visually select
    > - indent

# Nouns - Motions
    w - word
    W - WORD
    b - back a word
    B - back a WORD
    2j - down 2 line   
    iw - "inner word" (works from anywhere in a word)
    it - "inner tag" (content of html tag)
    i" - inner quotes
    i[ - inner brackets
    ip - inner paragraph
    as - a sentence

# Nouns - Parameterized
    f,F - find the next character
    t,T - find the next character (up to but not including that character)
    / - search (up to the match)

# Most important Commands
    :noh - undo markings in text (from search, ...)
    . - repeat your last (atomic) command (including the insertion when using c for example)
    zz - put the current line in the middle of the vim window

# Split management
    ctrl+hjkl - Switch vim Split in this direction

# Custom Operators
## Surround.vim
Plugin to create, change or delete surroundings of lines and whole text-objects

    cs*^ - change existing surrounding * to ^

    ds* - remove surrounding entirely

    yss* - surround entire line in *
        ) - for brackets without space
        ( - for brackets with space
        } - for braces without space
        { - for braces with space 
        etc.

    ys^* - surround text-object ^ with *
        iw - for the word
        etc.

      Example:
      "Hello world"

      $cs"'
      'Hello world'

      $ds'
      Hello world

      $yss{
      { Hello world }

      $ysiw) ( (with cursor on Hello)
      { (Hello) world }
  
    cst<h1> - change the surrounding tag to <h1>

Github-Link: https://github.com/tpope/vim-surround

## Commentary.vim
Plugin to comment whole lines or text-objects in vim.
    cml - comments over the line
    cmj - comments line and line below
    cmip - comments entire paragraph i am in
Every command toggles comments so I can undo it exactly like I enabled it!

Github-Link: https://github.com/tpope/vim-commentary

## SystemCopy
Plugin providing mappings for copying/ pasting text to the set os specific clipboard (usual pbcopy/ pbpaste for MacOS)
    cpiw - copy word into system clipboard
    cpi' - copy inside ' into system clipboard
    cP - copy the current line into system clipboard

Github-Link: https://github.com/christoomey/vim-system-copy

## Sort Motion.vim
    Plugin to sort paragraphs or text-objects in general in vim (alphabetical, after numbers etc.)

    gs* - sort the text-object/ motion *
    gs2j - sort down two lines (including the current line)
    gsip - sort the current paragraph
    gsi( - sort in paranthesis

Github-Link: https://github.com/christoomey/vim-sort-motion



## indent-Object
defines an indent as a Text Object in vim
    cmii - comments this indent (using Commentary.vim
    <count>ai         (A)n (I)ndentation level and line above.
    <count>ii         (I)nner (I)ndentation level (no line above).
    <count>aI         (A)n (I)ndentation level and lines above/below.
    <count>iI         (I)nner (I)ndentation level (no lines above/below). 

# a bit more into detail now:

## Move
### move cursor in line
    ^ - beginning of line (first not whitespace)
    0 - beginning of line (first column)
    $ - last character of line

### move cursor in words
    w - next word
    W - next WORD
    b - last word
    B - last WORD
    e - end of word
    E - end of WORD

### jump to next appearance of character x
    T• - backwards until character •
    t• - forward until character •

### move cursor in current view
    H - move cursor to top screen
    M - move cursor to middle of screen
    L - move cursor to bottom screen

### move and scroll
    ^d - move half a page down
    ^u - move half a page up
    ^b - move one page up
    ^f - move one page down
    ^y - scroll up
    ^e - scroll down

### mark and jump to mark
    m• - mark current position with character •
    `• - jump to position marked with character •


## Insert
    i - Insert in front of current character
    I - Insert in front of current line
    O - open newline over current line
    o - open newline below current line
    A - append after current line
    a - append after current character


## Visual
    p - paste yanked
    y - yank marked
    Y - yank current line
    d - delete marked
    < - unindent marked
    > - indent marked


## Commands
    u - undo anything
    U - undo whole line 
    ^r - redo change (undo the last undo)
    . - repeat the last command


## Macros
    q• - start recording macro in register • and stop again with q
    @• - run macro saved in register •    
    @@ - run last ran macro again

## Difference word/WORD
Foo(src,_dst,_len);    (_ = space)

word:

* foo
* (
* src
* ,
* dst
* ,
* len
* );


## WORD:
* Foo(src,
* dst,
* len);




## Latex-Suite
    ^j - jump to the next placeholder
    _ll - compile latex (_ = Space)
    F5 - make the last word you typed to a new environment

## Folding
    zo - open fold
    zc - close fold
    za - toggle fold
    zO - open fold on all levels
    zC - close fold on all levels
    zA - toggle fold on all levels
    zr - reduces folding by opening one more level of folds throughout the whole buffer
    zR - open all folds
    zM - close all folds
     
# Additional Vim Text-Objects

### Python Text-Objects
    af - a function
    if - inner function
    ac - a class
    ic - inner class

    new motions:
    [pf - move to next function
    ]pf - move to previous function
    [pc - move to next class
    ]pc - move to previous class

Github-Link: https://github.com/bps/vim-textobj-python

### Latex Text-Objects
    a\ and i\ - Inline math surrounded by \\( and \\)
    a$ and i$ - Inline math surrounded by dollar signs
    aq and iq - Single-quoted text
    aQ and iQ - Double-quoted text
    ae and ie - Environment surrounded by \begin{...} and \end{...}

Github-Link: https://github.com/rbonvall/vim-textobj-latex

### Entire Text-objects
    ae - entire content of the current buffer
    ie - same as ae without leading and trailing empty lines

Github-Link: https://github.com/kana/vim-textobj-entire



