# text.json

通过配置 text.json，您可以自由配置各项文本，个性化 AkashicQQ。

    {
        "not_enable": "此功能未开启！",
        "bilibililive_checker": {
            "message": "主播<name>开播啦！\n房间标题：<title>\n直播分区：<area>\n快去<url>围观吧！\n"
        },
        "bind_qq": {
            "help": "#绑定 ID | 将游戏 ID 和 QQ 号绑定",
            "format_error": "发送格式错误！\n发送格式：#绑定 ID",
            "not_bind_msg_in_game": "§4<player>，看起来您尚未将游戏账号和QQ号绑定，请在群内使用 #绑定 <player> 绑定您的账号\n如果您对此消息感到疑惑，请联系管理员",
            "not_bind_when_send_msg": "请先通过 #绑定 ID 绑定您的游戏账号！",
            "already_bind": "您已经绑定过账号！如果您对此感到疑惑，请联系管理员",
            "player_not_exist": "您要绑定的玩家不存在！请确认曾登录过以及输入正确",
            "success": "绑定成功！"
        },
        "call_admin": {
            "help": "#呼叫管理员 内容 | 向管理员发送消息",
            "format_error": "发送格式错误！\n发送格式：#呼叫管理员 内容"
        },
        "cmd_register": {
            "help": "#在线排行 | 查询服务器在线排行\n#tps | 查询服务器 TPS",
            "no_permission": "您没有向服务器发送此命令的权限！",
            "extra_arg": "此命令不能添加参数！",
            "answer": "已执行！\n<res>"
        },
        "get_invitation": {
            "help": "#邀请码 | 索取皮肤站邀请码",
            "get_msg": "您的邀请码为：<code>",
            "no_chance": "您已耗尽邀请码次数！请联系管理员"
        },
        "help": {
            "help": "#帮助 | 查看机器人帮助"
        },
        "issue_cmd": {
            "no_permission": "您没有向服务器发送命令的权限！",
            "format_error": "发送格式错误！\n发送格式：#命令 命令,回传行数,等待执行时间,服务器tag",
            "server_tag_not_exist": "服务器不存在！",
            "answer": "已执行！\n<res>"
        },
        "mc_event": {
            "server_start": "<tag>已开启，用时<time>s",
            "server_stop": "<tag>已关闭",
            "player_join": "<player>加入了<tag>",
            "player_advancement": "<player>在<tag>中取得了进度[<advancement>]",
            "player_chat": "<tag>中的<player>:<message>",
            "player_quit": "<player>退出了<tag>",
            "player_quit_private": "你退出了<tag>，请检查是否为掉线"
        },
        "query_online": {
            "help": "#在线人数 | 查询服务器在线人数",
            "no_player": "当前<tag>无人在线",
            "list_player": "<tag>当前有<num>人在线：<list>"
        },
        "say_mc_msg": {
            "help": "#服务器 内容 | 向服务器发送消息",
            "format_error": "发送格式错误！\n发送格式：#服务器 内容",
            "msg_in_game": "§5[QQ] §f<bind_player> <msg>"
        },
        "tell_mc_msg": {
            "help": "#私聊 ID 内容 | 向服务器内玩家私发消息",
            "format_error": "发送格式错误！\n发送格式：#私聊 ID 内容",
            "msg_in_game": "§5[QQ] §f<bind_player> 向你私聊消息：<msg>"
        },
        "welcome": {
            "help": "#欢迎 @新人 | 欢迎新人",
            "message": "欢迎来到服务器！"
        }
    }

+ `not_enable`

    当一项功能未开启时，玩家收到的提示。

+ `bilibililive_checker`

    哔哩哔哩直播间检测功能的各项文本。

    + `message`

        直播间开播时在群内发送的提醒内容。

        以下字段将被替换为实际内容：

        + \<name\>：主播名称
        + \<title\>：直播间标题
        + \<area\>：直播间分区
        + \<url\>：直播间链接

        同时，直播间封面将被展示在消息末尾。

+ `bind_qq`

    绑定 QQ 号功能的各项文本。

    + `help`

        功能命令帮助。此文本将在使用 #帮助 时展示。

        > 注意：后面的每个功能的 `help` 字段都与此类似，不再赘述。

    + `format_error`

        命令格式错误时返回的内容。

        > 注意：后面的每个功能的 `format_error` 字段都与此类似，不再赘述。

    + `not_bind_msg_in_game`

        玩家未绑定 QQ 号时，在进入游戏时收到的提示。

        以下字段将被替换为实际内容：

        + \<player\>：玩家游戏 ID
    
    + `not_bind_when_send_msg`

        玩家未绑定 QQ 号时，在使用需要绑定 QQ 号的功能时收到的提示。

    + `already_bind`

        已绑定过的玩家试图绑定 QQ 号时收到的提示。

    + `player_not_exist`

        玩家试图绑定不存在的游戏 ID 时收到的提示。

    + `success`

        玩家绑定成功时收到的提示。

+ `call_admin`

    呼叫管理员功能的各项文本。

+ `cmd_register`

    游戏命令注册器功能的各项文本。

    + `no_permission`

        玩家试图越权执行命令时收到的提示。

    + `extra_arg`

        玩家试图为禁止附加参数的命令附加参数时收到的提示。

    + `answer`

        玩家执行命令后收到的回复。

        以下字段将被替换为实际内容：

        + \<res\>：命令输出

+ `get_invitation`

    获取邀请码功能的各项文本。

    + `get_msg`

        成功获取邀请码后收到的回复。

        以下字段将被替换为实际内容：

        + \<code\>：邀请码

    + `no_chance`

        耗尽邀请码次数后收到的回复。

+ `help`

    帮助功能的各项文本。

+ `issue_cmd`

    向服务器发送任意命令功能的各项文本。

    + `no_permission`

        玩家试图越权执行命令时收到的提示。

    + `server_tag_not_exist`

        试图执行命令的服务器 tag 不存在时收到的提示。

    + `answer`

        执行命令后收到的回复。

        以下字段将被替换为实际内容：

        + \<res\>：命令输出

+ `mc_event`

    向 QQ 群提示服务器事件时的文本。

    + `server_start`

        服务器开启。

        以下字段将被替换为实际内容：

        + \<tag\>：服务器 tag
        + \<time\>：服务器启动用时

    + `server_stop`

        服务器关闭。

        以下字段将被替换为实际内容：

        + \<tag\>：服务器 tag

    + `player_join`

        玩家加入游戏。

        以下字段将被替换为实际内容：

        + \<player\>：玩家游戏 ID
        + \<tag\>：服务器 tag
        
    + `player_advancement`

        玩家获得成就。

        以下字段将被替换为实际内容：

        + \<player\>：玩家游戏 ID
        + \<tag\>：服务器 tag
        + \<advancement\>：进度名称

    + `player_chat`

        玩家聊天。

        以下字段将被替换为实际内容：

        + \<tag\>：服务器 tag
        + \<player\>：玩家游戏 ID
        + \<message\>：聊天内容

    + `player_quit`

        玩家退出游戏。

        以下字段将被替换为实际内容：

        + \<player\>：玩家游戏 ID
        + \<tag\>：服务器 tag

    + `player_quit_private`

        玩家退出游戏时向玩家私发的内容。

        以下字段将被替换为实际内容：

        + \<tag\>：服务器 tag

+ `query_online`

    查询各个服务器人数功能的各项文本。

    + `no_player`

        无人在线时返回的文本。

        以下字段将被替换为实际内容：

        + \<tag\>：服务器 tag

    + `list_player`

        有人在线时返回的文本。

        以下字段将被替换为实际内容：

        + \<tag\>：服务器 tag
        + \<num\>：服务器在线人数
        + \<list\>：服务器在线玩家列表

+ `say_mc_msg`

    向服务器发送消息功能的各项文本。

    + `msg_in_game`

        在游戏中的所有玩家看到的消息。支持颜色代码。

        以下字段将被替换为实际内容：

        + \<bind_player\>：发送消息的 QQ 号对应的游戏 ID
        + \<msg\>：消息

+ `tell_mc_msg`

    向服务器内玩家私聊消息功能的各项文本。

    + `msg_in_game`

        在游戏中的被私聊玩家看到的消息。支持颜色代码。

        以下字段将被替换为实际内容：

        + \<bind_player\>：发送消息的 QQ 号对应的游戏 ID
        + \<msg\>：消息

+ `welcome`

    入群欢迎功能的各项文本。

    + `message`

        入群欢迎消息。
