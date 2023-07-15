# AMLL TTML Database

作者特供给 AMLL 的 TTML 逐词歌词库，也欢迎大家前来建设本仓库！

如果需要制作逐词歌词，可以使用 [AMLL TTML Tools](https://github.com/Steve-xmh/amll-ttml-tool) 哦！

## 歌词要求

### 歌词内容要求

#### 硬性要求

- 不要在歌词主体里包含除歌词内容以外的信息（例如 作词、作曲 这类信息）
- 不要留空行，请善用结束时间来让歌词播放器自动生成间奏区域
- 单词时序不能有误（例如开始时间比结束时间晚的）
- 如果是英文歌曲，确保单词间隔不会超过一个空格

#### 优先审核要求

- 尽量是逐词歌词，会优先审核
- 尽量利用好 TTML 歌词特性，例如背景人声歌词和对唱人声歌词，会优先审核
- 尽可能提供翻译和音译（如果有），你可以在每行 `p` 元素中加入 `span[ttm:role=x-translation]` 作为翻译文本或者 `span[ttm:role=x-roman]` 作为音译文本。具体可以参考下方的歌词范例。

### 歌词提交要求

请提供和 Apple Music 所需 TTML 格式歌词要求一致的歌词文件，如果可以请尽量制作逐词歌词，并命名成 `歌曲在网易云上的音乐ID.ttml` 后存放于 `./lyrics` 文件夹后发送 Pull Request 提交歌词即可。

或者根据议题模板提交模板，Github Action 会自动检查歌词文件格式并为你创建合并请求。

## 歌词文件范例

- [YOASOBI - 群青 （含副唱歌词）](./lyrics/1472480890.ttml)
- [YOASOBI - 祝福 （含背景歌词）](./lyrics/1983292457.ttml)

（歌词文件非常标准的也可以在 PR 时给本列表增加项目）

## 共享协议

本仓库的外来数据部分遵循原数据提供方的共享协议共享，提交者自主编写的部分使用 CC0 1.0 共享协议共享。
