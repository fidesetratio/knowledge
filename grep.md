# Tips & Trick Grep


```bash

grep -win -C 2 "patar" data.txt // only for files

grep -winr "patar" . // recursive in directory

grep -winrP "\d{3}-\d{3}-\d{3}" // searching with pattern regex perl like

grep -wirlP "\d{3}-\d{3}-\d{3}" // only display the name of folder

grep -wircP "\d{3}-\d{3}-\d{3}" // display file and also count of matched 

```

Detail:
* w = word
* i = uppercase or not uppercase
* C = context n lines from after, n lines before matched
* r = recursive for searching inside folder and sub folder
* P = Pattern regex searching using regex perl like (only on linux)
* l = only display the name of file consists of matched word
* c = count for matched word
