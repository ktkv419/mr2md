# MoonReader bookmarks/notes to Markdown converter

This is a script to convert notes and bookmarks from MoonReader+ into Markdown (specifically Obsidian's markdown spec)

### How to use

1. Export notes and bookmarks from MoonReader to txt
2. Copy script to `~/.local/bin` or folder with exported file
3. Run
   _Executing without arguments will result in converting all valid txt files inside that folder_
   `$ mr2md`
   _Executing with filename as an argument will convert only that file_
   `$ mr2md exported.txt`

###### Input file:

`exported.txt`

```
Book name - Author (Highlight: 1; Note: 1)

───────────────

◆ Chapter 1

▪️ Lorem ipsum dolor sit amet, consectetur adipiscing elit (Vivamus non mattis sapien, at sollicitudin eros). (This is a note)
```

###### Output file:

`Author - Book name.md`

```
Tags: #Author #BookName
# Chapter 1
## Lorem ipsum dolor sit amet, consectetur adipiscing elit (Vivamus non mattis sapien, at sollicitudin eros).
_This is a note_
```
