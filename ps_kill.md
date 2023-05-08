# Display process (kill them if you want)

> Liệt kê các process đang chạy, xem được PID, STATE.

```
# Khi bạn chạy command ps không kèm options,
# nó sẽ hiển thị thông tin về tất cả các process đang chạy trong màn hình terminal của bạn
$ ps

# Nếu bạn chạy nhiều màn hình terminal với cùng 1 user, bạn muốn xem hết chúng thì cần thêm options x
# Option x này cũng sẽ hiển thị thêm thông tin cột STAT, ý nghĩa tham khảo thêm phần dưới
$ ps x

# Thường để tìm kiếm các process đang chạy với tên là "ruby" thì ta sẽ dùng command dưới đây
$ ps aux | grep ruby

# PROCESS STATE CODES
#   D    uninterruptible sleep (usually IO)
#   R    running or runnable (on run queue)
#   S    interruptible sleep (waiting for an event to complete)
#   T    stopped, either by a job control signal or because it is being traced.
#   W    paging (not valid since the 2.6.xx kernel)
#   X    dead (should never be seen)
#   Z    defunct ("zombie") process, terminated but not reaped by its parent.
# 
#   For BSD formats and when the stat keyword is used, additional characters may be displayed:
#   <    high-priority (not nice to other users)
#   N    low-priority (nice to other users)
#   L    has pages locked into memory (for real-time and custom IO)
#   s    is a session leader
#   l    is multi-threaded (using CLONE_THREAD, like NPTL pthreads do)
#   +    is in the foreground process group.
```

### KILL process mong muốn

> Đôi khi thì chúng ta cần phải stop các process đang chạy ngầm đi, thì chúng ta phải dùng `ps aux | grep "tên process"`, sau đó thì dùng lệnh kill để gửi tín hiệu đến process để dừng nó.

```bash
$ kill [-s signal_name] pid ...

# Some of the more commonly used signals:
# 1       HUP (hang up)
# 2       INT (interrupt)
# 3       QUIT (quit)
# 6       ABRT (abort)
# 9       KILL (non-catchable, non-ignorable kill)
# 14      ALRM (alarm clock)
# 15      TERM (software termination signal)
```

⚠️ Thường để process stop chuẩn thì nên gửi tín hiệu 15, thì nó sẽ thực thi các command cần thiết khi dừng chương trình. Khi chương trình có dấu hiệu bị treo, thì dùng tín hiệu 9, nó sẽ force close process.
