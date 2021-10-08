# bilibililive_checker.json

通过配置 bilibililive_checker.json，您可以让 AkashicQQ 在指定直播间开播时向群内发送提醒。

    {
        "enable": false,
        "group": [
            123456789
        ],
        "liveroom": [
            123456
        ]
    }

+ `enable`

    是否开启此功能。

+ `group`

    开播提醒向哪些群发送。

+ `liveroom`

    监控哪些直播间。

    > 注意：此项为主播的 UID 而非房间号。