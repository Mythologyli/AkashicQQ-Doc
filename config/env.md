# .env .env.dev .env.prod

.env .env.dev .env.prod 三个文件位于您的根目录中。

在配置其他配置文件之前，您应该首先配置三个配置文件。

## .env 文件

    ENVIRONMENT=prod

+ `ENVIRONMENT`

    `ENVIRONMENT` 项取值：

    + prod
    + dev

    `ENVIRONMENT` 项决定了 AkashicQQ 运行在生产模式下还是调试模式下。

## .env.dev .env.prod 文件

这两个文件具有以下内容：

    HOST=0.0.0.0
    PORT=4399
    DEBUG=true # .env.prod 文件中此项为 false
    COMMAND_START=["#"]

+ `HOST` `PORT`

    `HOST` 项是您的 AkashicQQ 绑定的 IP，`PORT`项为绑定的端口。

    如果您的 AkashicQQ、Prism Console、cqhttp(onebot) 协议实现程序都在同一服务器上运行，您可以将 `HOST` 项设置为 127.0.0.1。

    > 注意：当 `HOST` 项设置为 0.0.0.0 时，AkashicQQ 可能暴露在公网上，请通过配置防火墙的方式确保安全。

+ `DEBUG`

    `DEBUG` 项无需更改。

+ `COMMAND_START`

    `COMMAND_START` 项配置您的 QQ 命令起始符。例如，当 `COMMAND_START` 项包含 '#' 时，类似 #在线人数 的消息将被识别为一条命令。您可以配置多个命令起始符。

    > 注意：不建议将命令起始符配置为 '/'。可能导致在 PC 端输入困难。

    建议配置 .env.dev .env.prod 两个文件。这样可以通过更改 .env 中的 `ENVIRONMENT` 项快捷地在生产模式和调试模式中切换。