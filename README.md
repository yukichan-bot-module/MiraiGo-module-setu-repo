# MiraiGo-module-seturepo

ID: `com.aimerneige.seturepo`

Module for [MiraiGo-Template](https://github.com/Logiase/MiraiGo-Template)

## 功能

- 在群聊中接受到指定消息时发送特定的消息，并通过私聊随机发送一张指定路径下的色图。
- 在私聊接受到指定消息时随机发送一张指定路径下的色图。

## 使用方法

在适当位置引用本包

```go
package example

imports (
    // ...

    _ "github.com/yukichan-bot-module/MiraiGo-module-seturepo"

    // ...
)

// ...
```

编辑你的配置文件 `seturepo.yaml`：

```yaml
"来点萝莉":
  - "太变态了！不可以!"
  - "/opt/img-data/luoli/"
"刻晴老婆":
  - "好耶，是刻晴"
  - "/opt/img-data/keqing/"
```

在你的 `application.yaml` 里填入配置：


```yaml
aimerneige:
  seturepo:
    path: "./config/seturepo.yaml" # 默认配置文件路径 `./seturepo.yaml`
    blacklist: # 黑名单
      - 1781924496
```
