---
title: "hugo集成utteranc"
date: 2022-01-28T14:01:38+08:00
draft: false
tags: ["hugo"]
categories: ["2022"]
---

### 使用
主页 https://utteranc.es/

- 使用github issue来管理用户的评论，无广告、干净
- 安装完之后只需要将下面的代码嵌入你的代码中即可

```
<script src="https://utteranc.es/client.js"
        repo="[ENTER REPO HERE]"
        issue-term="pathname"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>
```

- 若想删除评论，只需要去github删除对应的issue就行

### hugo even 主题集成
需要修改配置文件，指定你的仓库
```
  [params.utterances]       # https://utteranc.es/
    owner = "xxx"              # Your GitHub ID
    repo = "xxx.github.io"               # The repo to store comments
```