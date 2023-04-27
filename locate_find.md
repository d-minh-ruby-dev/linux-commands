# Tìm kiếm file

> Trong Linux, để tìm kiếm file, ta dùng command `locate` hoặc `find`

## Sử dụng `find` command

```bash
$ find "path-thư-mục-cha" -type f -name "tên-file-cần-tìm"
$ find "path-thư-mục-cha" -type d -name "tên-thư-mục-cần-tìm"
```

## Sử dụng `locate` command

Để sử dụng command `locate`, thì ta cần phải cập nhật file `mlocate.db` bằng command dưới đây:

```bash
$ updatedb
```

Tìm kiếm file bằng command locate

```bash
$ locate "tên-file-cần-tìm" 

# Ví dụ
$ locate config.ru
/usr/local/bundle/gems/draper-4.0.2/spec/dummy/config.ru
/usr/local/bundle/gems/pry-rails-0.3.9/spec/config/config.ru
...
```
