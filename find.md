#find

Tips and Trick find command

```bash

find . -type f -name "patar" // strict matched patar
find . -type f -name "*.txt" // only end with .txt
find . -type f -name "patar*" // begin with patar
find . -type f -iname "patar*" // begin with patar and uppercase or lettercase
find . -type f --mmin -10  //search modified file last ten minutes ago
find . -type f --mmin +10  //search modified file more than ten minutes ago
find . -type f --mmin +1 --mmin -5 // search modified more than 1 minutes ago and les 5 minutes

find . -type f --mtime +1 // search modified more than 1 days ago
find . -size +5M // search 5Mega Byte (M), 5 Gigabyte (G), 5 killobytes (k)
find . -empty // search empty file
find . -perm 777 // search permision 777

find . -type f -name ".jpg" -maxdepth 1 // dont forget maxdepth = 1 current folder



```
