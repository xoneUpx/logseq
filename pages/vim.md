- how to yank part of some file into current buffer:
  ```vim
  :r !sed -d :range:p  path/to/file
  ```