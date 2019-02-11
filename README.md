# Systemd unit file and configuration example for [9seconds/mtg](https://github.com/9seconds/mtg)

The [mtg](https://github.com/9seconds/mtg) application is the very tiny and bullshit-free MTProto proxy realization (useful if you need to chat in Telegram reliably in Russia). 

## How to use

1. Install tmux (you can control behaviour and status of ``mtg`` later using ``tmux attach -t mtproxy``.
2. Put pre-compiled binary of ``mtg`` on server as ``/usr/local/bin/mtproxy``.
3. Put the ``mtproxy.service`` file into ``/etc/systemd/system/``.
4. Write arguments that you want to pass to ``mtproxy`` binary into plain text file ``/etc/mtproxy/arguments``.

The example working file of my own looks like this:

```
<my-proxy-password> -b <my-ip> -s
```

For full list of available parameters see the documentation of original application.
