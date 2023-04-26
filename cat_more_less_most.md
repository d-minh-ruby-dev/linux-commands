# Các command để hiển thị nội dung file trong màn hình terminal

## TL;DR
`cat` để hiển thị toàn bộ file, thường chỉ dùng đối với file ngắn.\
`more`, `less` và `most` là 3 command để hiển thị file có phân trang:
* `less` nhiều chức năng hơn `more`
* `most` nhiều chức năng hơn `more`
* `less` và `most` là khác nhau, không có cái nào tốt hơn.

Trong MacOS, more và less giống nhau, không có sẵn lệnh most.

## What Less can do and Most can't 

* regex search (giống vim)
* Filter, with &: display only matching lines. It's a bit like a grep but you keep the same shortcuts you had before.
* less can display (at least) 256 colors, and most can display only 8 colors.
* less hiển thị nhiều màu hơn (256 màu), most chỉ hiển thị 8 màu.
* less hiển thị được chữ đậm (bold)

## What Most can do and Less can't
* chia dọc màn hình (không thể resize)
* config
* Binary mode, that looks like xxd.