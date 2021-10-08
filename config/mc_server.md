# mc_server.json

    {
        "main_server_tag": "主服",
        "server": [
            {
                "tag": "主服",
                "url": "http://127.0.0.1:8520"
            },
            {
                "tag": "游戏服",
                "url": "http://192.168.1.2:8520"
            }
        ]
    }

+ `main_server_tag`

    `main_server_tag` 项应配置为您主要服务器的 tag。

    > 注意：此处的 tag 即为您在 Prism Console 中的配置的 tag。请务必保持一致。

+ `server`

    `server` 项为您每一个服务器的具体配置。

    + `tag`：服务器 Prism Console 的 tag
    + `url`：服务器 Prism Console API 对应的 url 地址，即 `http://{host}:{port}`