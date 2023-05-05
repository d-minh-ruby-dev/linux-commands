# wc - Hiển thị số dong, số từ, số byte của file

>　Đếm số dòng của file (sample.c)

```bash
$ wc sample.c
```

## Options

```
-c, --bytes # print the byte counts
-m, --chars # print the character counts
-l, --lines # print the newline counts
--files0-from=F # read input from the files specified by NUL-terminated names in file F; If F is - then read names from standard input
-L, --max-line-length # print the length of the longest line
-w, --words # print the word counts
```

## Tips

### Đếm số file, directory trong 1 thư mục

```bash
$ ls | wc -l
```