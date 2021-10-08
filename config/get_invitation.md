# get_invitation.json

通过配置 get_invitation.json，您可以将 AkashicQQ 和您的 [Blessing Skin Server](https://github.com/bs-community/blessing-skin-server) 对接，实现在 QQ 群中申请皮肤站的邀请码。

    {
        "enable": false,
        "blessing_skin_server_mysql": {
            "host": "127.0.0.1",
            "port": 3306,
            "user": "skin",
            "password": "",
            "db": "skin"
        },
        "initial_chance": 0
    }

+ `enable`

    是否启用此功能。

+ `blessing_skin_server_mysql`

    配置 Blessing Skin Server 的数据库。

    + `host`：数据库地址
    + `port`：数据库端口
    + `user`：用户名
    + `password`：密码
    + `db`：数据库名称

+ `initial_chance`

    每个 QQ 群成员默认拥有几次获取邀请码机会。
