# Thay thế text trong một file text

> Đổi chuỗi ký tự "taro" bằng chuỗi ký tự "hanako" trong file text "sample.txt"

```bash
$ sed -e 's/taro/hanako/g' sample.txt
```

### Cấu trúc command

`sed` là một command dùng để sửa text trong file (text stream editor).

```bash
$ sed 【options】 【regex pattern】 【file name】
```

### Khi bạn muốn delete từ dòng 30 đến 35

The following example deletes lines 30 to 35 in the input. 30,35 is an address range. d is the delete command:

```bash
sed '30,35d' input.txt > output.txt
```

### Xử lý nhiều process một lúc

```bash
sed '/^foo/d ; s/hello/world/' input.txt > output.txt
```

### (to be continue)