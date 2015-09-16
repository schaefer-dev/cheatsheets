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


# WORD:
* Foo(src,
* dst,
* len);


# Move
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


# Insert
    i - Insert in front of current character
    I - Insert in front of current line
    O - open newline over current line
    o - open newline below current line
    A - append after current line
    a - append after current character


# Visual
    p - paste yanked
    y - yank marked
    Y - yank current line
    d - delete marked
    < - unindent marked
    > - indent marked


# Commands
    u - undo anything
    U - undo whole line 
    ^r - redo change (undo the last undo)


# Macros
    q• - start recording macro in register • and stop again with q
    @• - run macro saved in register •    
    @@ - run last ran macro again

# Latex-Suite
    ^j - jump to the next placeholder
    _ll - compile latex (_ = Space)

# Folding
    zo - open fold
    zc - close fold
    za - toggle fold
    zO - open fold on all levels
    zC - close fold on all levels
    zA - toggle fold on all levels
    zr - reduces folding by opening one more level of folds throughout the whole buffer
    zR - open all folds
    zM - close all folds
     



