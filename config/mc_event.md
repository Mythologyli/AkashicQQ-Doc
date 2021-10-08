# mc_event.json

mc_event.json 配置了哪些 Minecraft 事件将在群内广播。

    {
        "enable": {
            "server_start": true,
            "server_stop": true,
            "player_join": true,
            "player_advancement": true,
            "player_chat": true,
            "player_quit": true,
            "player_quit_private": true
        }
    }

+ `server_start`：服务器开启事件是否在群内广播。
+ `server_stop`：服务器关闭事件是否在群内广播。
+ `player_join`：玩家加入事件是否在群内广播。
+ `player_advancement`：玩家获得成就事件是否在群内广播。
+ `player_chat`：玩家聊天事件是否在群内广播。
+ `player_quit`：玩家退出事件是否在群内广播。
+ `player_quit_private`：玩家退出事件是否向玩家本人私发。通过配置此项，您可以实现掉线提醒功能。