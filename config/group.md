# group.json

> 注意：group.json 及其之后的配置文件均为 JSON 格式，位于根目录下的 config 文件夹中。请使用 UTF-8 编码编辑和保存配置文件，并确保配置文件符合 JSON 格式。

    {
        "main_group": 123456789,
        "op_user": [
            654321,
            123456
        ],
        "admin_user": [
            654321,
            123456,
            000123
        ]
    }

+ `main_group`

    `main_group` 项配置 QQ 群的群号。这应当是您的 Minecraft 服务器官方群的群号。请确认 AkashicQQ 使用的 QQ 号已加入此群并被设置为管理员。

+ `op_user`

    `op_user` 项配置了哪些 QQ 号具有 OP 权限，即远程向任意服务器执行任意命令。

    > 注意：请务必慎重配置此项。一般只建议将您自己配置为 `op_user`。

+ `admin_user`

    `admin_user` 项配置了哪些 QQ 号是您的管理员。管理员账号将会自动接收呼叫管理员等消息。请确认 AkashicQQ 使用的 QQ 号已和此配置项中的 QQ 号建立好友关系，否则将无法接收私聊消息。

    > 注意：将 QQ 号配置为 `op_user` 并不会使其自动成为 `admin_user`。一般来说，您应当在两项中同时配置自己的 QQ 号。
