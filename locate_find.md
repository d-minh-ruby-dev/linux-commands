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
/usr/local/bundle/gems/rails-controller-testing-1.0.5/test/dummy/config.ru
/usr/local/bundle/gems/railties-6.1.4.6/lib/rails/generators/rails/app/templates/config.ru.tt
/usr/local/bundle/gems/redis-actionpack-5.2.0/test/dummy/config.ru
/usr/local/bundle/gems/slim-4.1.0/test/rails/config.ru
/usr/local/bundle/gems/webpacker-5.4.3/test/test_app/config.ru
/usr/local/bundle/ruby/3.0.0/gems/draper-4.0.2/spec/dummy/config.ru
/usr/local/bundle/ruby/3.0.0/gems/pry-rails-0.3.9/spec/config/config.ru
/usr/local/bundle/ruby/3.0.0/gems/rails-controller-testing-1.0.5/test/dummy/config.ru
/usr/local/bundle/ruby/3.0.0/gems/railties-6.1.4.6/lib/rails/generators/rails/app/templates/config.ru.tt
/usr/local/bundle/ruby/3.0.0/gems/redis-actionpack-5.2.0/test/dummy/config.ru
/usr/local/bundle/ruby/3.0.0/gems/redis-actionpack-5.3.0/test/dummy/config.ru
/usr/local/bundle/ruby/3.0.0/gems/slim-4.1.0/test/rails/config.ru
/usr/local/bundle/ruby/3.0.0/gems/slim-5.1.0/test/rails/config.ru
/usr/local/bundle/ruby/3.0.0/gems/webpacker-5.4.3/test/test_app/config.ru
```
