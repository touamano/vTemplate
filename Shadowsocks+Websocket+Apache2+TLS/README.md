# 这是一个使用 V2Ray 作为 ss + v2ray plugin 服务端的示例

**config_server_redirect.json 和 config_server_domainsocket.json 选其一**

## shadowsocks windows 客户端关键部分示例如下：
```
Server IP: example.org
Server Port: 443
Passowrd: ifYouWantToKeepYourPassphraseSafeChangeThis!!
Encryption: chacha20-ietf-poly1305
Plugin Program: pathToYourV2ray-plugin_windows_arch.exe
Plugin Options: tls;mode=websocket;path=/michi;host=example.org
```
## shadowsocks Android plugin 关键部分示例如下：

**需安装 shadowsocks 和 v2ray plugin，并搭配一同使用**
```
Plugin: v2ray
Configure:
    Transport mode: websocket-tls
    Hostname: example.org
    Path: /michi
    Concurrent connections: 1
    Certificate for TLS verification: Not set
```