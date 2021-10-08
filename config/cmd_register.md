# cmd_register.json

通过将命令注册到 cmd_register.json，您可以在 QQ 内方便地向服务器内使用别名发送命令，而无需使用 #命令 命令内容。您借此配合其他插件实现在 QQ 中查看服务器 TPS 等功能。

    [
        {
            "cmd": "list",
            "aliases": [
                "在线列表"
            ],
            "no_arg": true,
            "num": 1,
            "wait_time": 1,
            "server_tag": "主服",
            "allow_member": [],
            "permission": "ALL"
        },
        {
            "cmd": "tps",
            "aliases": [
                "运行状态"
            ],
            "no_arg": true,
            "num": 1,
            "wait_time": 1,
            "server_tag": "主服",
            "allow_member": [],
            "permission": "ADMIN"
        },
        {
            "cmd": "op",
            "aliases": [],
            "no_arg": false,
            "num": 1,
            "wait_time": 1,
            "server_tag": "主服",
            "allow_member": [],
            "permission": "OP"
        },
        {
            "cmd": "deop",
            "aliases": [],
            "no_arg": false,
            "num": 1,
            "wait_time": 1,
            "server_tag": "主服",
            "allow_member": [],
            "permission": "OP"
        },
        {
            "cmd": "lp editor",
            "aliases": [
                "权限编辑"
            ],
            "no_arg": true,
            "num": 3,
            "wait_time": 5,
            "server_tag": "主服",
            "allow_member": [],
            "permission": "OP"
        }
    ]

+ `cmd`

    在 Minecraft 服务器控制台中执行的命令头。例如 whitelist op 等等。

+ `aliases`

    命令头的别名。设置别名后，可以用 #在线列表 代替 #list

+ `no_arg`

    配置为 true 是，命令将不接受任何参数。

    > 注意：允许命令附加参数可能造成意想不到的后果。如果您希望命令带有特定参数，您可以在 `cmd` 项中配置。例如，将 `cmd` 项配置为 whitelist list 并设置别名为“查看白名单”，您的玩家可以通过 #查看白名单 执行带有特定参数的命令。

+ `num`

    您期望向您返回**最多**几行的命令输出。通过配置此项，您可以完整地获取多行输出，而不用担心输出被截断（在其它类似插件中常出现此问题）。如果 `num` 多于实际的输出行数，Prism Console 将返回实际的输出行。

+ `wait_time`

    在命令执行后，Prism Console 将等待 `wait_time` 时间（单位为秒），然后捕获命令的输出。这适用与需要较长时间执行的命令，如 lp editor。

    > 注意：此项配置为 0 将不会获取任何命令输出，无论 `num` 项配置如何。这适用于一些无需获取命令输出的命令。同样，如果您要获取命令输出，您至少要将 `wait_time` 项配置为 1。

+ `server_tag`

    此项配置命令将在哪个服务器上执行。

+ `allow_member`

    哪些 QQ 号被赋予执行命令的权限。在此项中配置的 QQ 号将无视 `permission` 项获取执行命令的权限。

+ `permission`

    此项可配置为如下值：

    + "ALL"：所有人都可执行此命令
    + "ADMIN"：仅 ADMIN 和 OP 可以执行此命令
    + "OP"：仅 OP 可以执行此命令
