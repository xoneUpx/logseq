- how to yank part of some file into another:
  ```vim
  :r !sed -d :range:p  path/to/file
  ```