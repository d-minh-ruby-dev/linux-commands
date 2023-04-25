# ファイル(sample.cgi)の改行コードをLinux用に変換する

>   Thay đổi mã code xuống dòng trong file (sample.cgi) từ Windows format sang Linux format.

```bash
$ dos2unix <file-path>
# Ví dụ
$ dos2unix sample.cgi
```

## Tình huống sử dụng
Khi bạn muốn chạy một script từ môi trường Windows.

Ở windows thì mã xuống dòng nó là [CR][LF], còn ở Linux thì là [LF].
Vì thế, những script mà đã tạo ở môi trường Windows, nếu giữ nguyên thì sẽ không chạy được ở môi trường Linux.
Để nó chạy được, thì 2 câu command `dos2unix` và `unix2dos` dùng để chuyển đổi file giữa 2 môi trường.