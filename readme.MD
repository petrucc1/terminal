## <!-- Shortcuts -->
- **Up - Down:** see your previous commands;
- **Ctrl + arrows:** skip words (Mac option + arrows);
- **Ctrl + A:** go to the beginning of the line;
- **Ctrl + E:** go to the end of the line;
- **Ctrl + U:** clear the line;
- **Ctrl + K:** erases everything on the line up to where the cursor is positioned;
- **Ctrl + L:** clear, clear the terminal (CMD + K for Mac).

## <!-- Files and directories -->
- **man <command>**
    open the manual
- **pwd**
    shows the current directory
- **cd - cd .**
    change directory
- **cd ..**
    back directories
- **cd -**
    back where you came from
- **ls**
    list files and folders
- **-l**
    more information
- **-a**
    all, show hidden files
- **-h**
    human, shows byte, kilobyte, megabyte and gigabyte
- **-R**
    recursive, shows folders and files in an organized way
- **-S**
    sort by size

## <!-- Getting file information -->
- **file <file name>**
    show full file information
- **stat <file name>**
    show file permissions and modifications

## <!-- Creating directories with mkdir -->
- **mkdir**
    create directories
- **-p**
    parents, create multiple folders, example: `site/src/adm site/src/public site/src/assets`
- **touch**
    change timestamp or create files
- **cp**
    copy files and folders, to copy files `cp`: file1.txt file2.txt, to copy directories `cp -r`: `site1 site 2 site3 sites`, the last file or the last folder is where the content will be copied
- **mv**
    move and rename files and folders
- **rm**
    permanently remove files and folders `rm -r`, if you want to forcibly remove it you can use `-f` too
- **wildcards**
    are * and ?, in the case of *, all files with the first letters fil, would be moved to the Directory folder, that is, if I had 3 files with names file1 file2 and file3, or even 500 files with the first 3 letters in their name being `fil*`, would be moved to the Directory folder.
    In the case of ?, we would be moving only the folders with a number at the end, making the command ignore the site folder and the site67 folder, as only one digit after the wildcard is passed.
    Example *: `mv fil* directory`
    Example ?: `mv -r site? directory`
- **find**
    find files or folders, `find .` will search in the current directory, `-type` select the type of file `f`/directory `d` to search, `-name` select what I want to have in the name of the file/folder I'm looking for. Full example:
    `find . -type f -name "*.jpg"`
- **cat and less**
    show the contents of files, less has the same idea as the manual, that is, you can press h and see how to use less in more detail and cat will print the file content directly on the screen, making it possible to move up and down the content with the mouse scroll
- **nano and vim**
    both edit files, it's a text editor, however, you can't use your mouse, to navigate use the keyboard arrows, and below is the legend of what can be done, through the Ctrl key and some more letters. For example, the combination 'Ctrl + O' would save this file, but first you would be asked if you want to save the file with the same name, if you answer no, you will be shown a screen to change the file name. To close nano, the shortcut is 'Ctrl + X'.
    Vim is much more complex than nano, and you can insert plugins into it, making it more powerful. To exit vim, use the `:q` command. However, if you have made any changes, it will need either the `:wq` command, to confirm, write these changes and exit, or the `:q!` command, which cancels the changes
