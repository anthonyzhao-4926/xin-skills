---
name: xin-convert-file
description: 当需要进行文件格式转换时使用
argument-hint: [input_file] [output_format]
arguments: input_file output_format
disable-model-invocation: true
model: claude-haiku-4-5-20251001
---

# 文件转换

仅需要执行如下命令

```
echo "处理文件：$input_file"
echo "目标格式：$output_format"
```

