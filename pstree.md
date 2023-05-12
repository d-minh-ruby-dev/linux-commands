# pstree – list processes as a tree

> pstree - Hiển thị list các process dạng tree.

```bash
$ pstree
```

### Ví dụ

Show các nhánh của process chứa httpd, hiển thị dạng graphic VT100:

```bash
$ pstree -g 2 -s httpd
```

Show process number "15495" và hậu duệ của nó:

```bash
$ pstree 15495
```

Show process number "15495" và cha cả hậu duệ của nó:

     
```bash
$ pstree -p 15495
```