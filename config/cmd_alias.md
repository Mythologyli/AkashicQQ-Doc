# cmd_alias.json

cmd_alias.json 配置了每个命令的名称和别名。

> 注意：别名可以有多个，但必须为每个命令配置一个名称。玩家可以使用 #命令名称 或 #命令别名 触发命令。

    {
        "help": {
            "cmd": "帮助",
            "aliases": []
        },
        "bind_qq": {
            "cmd": "绑定",
            "aliases": [
                "绑定账号"
            ]
        },
        "call_admin": {
            "cmd": "呼叫管理员",
            "aliases": []
        },
        "get_invitation": {
            "cmd": "邀请码",
            "aliases": []
        },
        "issue_cmd": {
            "cmd": "命令",
            "aliases": []
        },
        "query_online": {
            "cmd": "在线人数",
            "aliases": []
        },
        "say_mc_msg": {
            "cmd": "服务器",
            "aliases": [
                "公聊"
            ]
        },
        "tell_mc_msg": {
            "cmd": "私聊",
            "aliases": []
        },
        "welcome": {
            "cmd": "欢迎",
            "aliases": []
        }
    }
