# fortune - print a random, hopefully interesting, adage

> fortune - in ngẫu nhiên một câu ngạn ngữ

```bash
# Install
$ sudo apt install fortune # ubuntu
$ brew install fortune # macos

# Run
$ fortune
The last thing one knows in constructing a work is what to put first.
-- Blaise Pascal
```

# cowsay/cowthink - configurable speaking/thinking cow (and a bit more)

> Hiển thị text cùng với con bò đang nói hoặc suy nghĩ.

```bash
# Install
$ sudo apt install cowsay # ubuntu
$ brew install cowsay # macos

# Run
$ cowsay I love you
 ____________
< I love you >
 ------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

# Kết hợp 2 command trên với nhau

```bash
$ fortune | cowsay
 _________________________________________
/ Nasrudin returned to his village from   \
| the imperial capital, and the villagers |
| gathered around to hear what had        |
| passed. "At this time," said Nasrudin,  |
| "I only want to say that the King spoke |
| to me." All the villagers but the       |
| stupidest ran off to spread the         |
| wonderful news. The remaining villager  |
| asked, "What did the King say to you?"  |
| "What he said -- and quite distinctly,  |
| for everyone to hear -- was 'Get out of |
| my way!'" The simpleton was overjoyed;  |
| he had heard words actually spoken by   |
| the King, and seen the very man they    |
\ were spoken to.                         /
 -----------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```
