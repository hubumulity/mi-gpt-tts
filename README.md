# MiGPT-TTS

适用于 [MiGPT](https://github.com/idootop/mi-gpt) 的 TTS 模块，提供以下接口：

## GET /api/tts.mp3

文字合成音频，请求示例：

`/api/tts.mp3?speaker=BV700_streaming&text=很高兴认识你`

> 注意：`speaker` 是音色名称或标识（key）可选。

## GET /api/speakers

获取音色列表

| 属性    | 说明     | 示例              |
| ------- | -------- | ----------------- |
| name    | 音色名称 | `灿灿`            |
| gender  | 性别     | `女`              |
| speaker | 音色标识 | `BV700_streaming` |

返回值示例

```json
[
  {
    "name": "广西老表",
    "gender": "男",
    "speaker": "BV213_streaming"
  },
  {
    "name": "甜美台妹",
    "gender": "女",
    "speaker": "BV025_streaming"
  }
]
```

## License

[MIT](https://github.com/idootop/mi-gpt/blob/main/LICENSE) License © 2024-PRESENT Del Wang
