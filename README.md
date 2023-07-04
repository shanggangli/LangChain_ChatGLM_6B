---
license: openrail
title: 'Chinese-LangChain '
sdk: gradio
emoji: 🚀
colorFrom: yellow
colorTo: yellow
pinned: true
app_file: app.py
---

# LangChain ChatGLM_6B

> LangChain_ChatGLM_6B：基于ChatGLM-6b+langchain实现本地化知识库检索与智能答案生成

## 🔥 效果演示

![](https://github.com/shanggangli/LangChain_ChatGLM_6B/blob/main/images/knowledge.png)
![](https://github.com/shanggangli/LangChain_ChatGLM_6B/blob/main/images/web.png)

## 🚋 使用教程

- 选择知识库询问相关领域的问题

## 🏗️ 部署教程

### 运行配置

- 显存：12g，实际运行9g够了
- 运行内存：32g
- 本项目使用了两张T4显卡，模型并行运行
### 运行环境

```text
langchain
gradio
transformers
sentence_transformers
faiss-cpu
unstructured
duckduckgo_search
mdtex2html
chardet
cchardet
```

### 启动Gradio

```shell
python main.py
```

## 🧰 知识库

### 构建知识库

- Wikipedia-zh

> 详情见：corpus/zh_wikipedia/README.md

### 知识库向量索引

| 知识库数据                                                                         | FAISS向量                                                              |
|-------------------------------------------------------------------------------|----------------------------------------------------------------------|
| 中文维基百科截止4月份数据，45万                                                             | 链接：https://pan.baidu.com/s/1VQeA_dq92fxKOtLL3u3Zpg?pwd=l3pn 提取码：l3pn |
| 截止去年九月的130w条中文维基百科处理结果和对应faiss向量文件 @[yubuyuabc](https://github.com/yubuyuabc) | 链接：https://pan.baidu.com/s/1Yls_Qtg15W1gneNuFP9O_w?pwd=exij 提取码：exij |
| 💹 [大规模金融研报知识图谱](http://openkg.cn/dataset/fr2kg)                              | 链接：https://pan.baidu.com/s/1FcIH5Fi3EfpS346DnDu51Q?pwd=ujjv 提取码：ujjv |

## 🔨 TODO

* [x] 支持上下文
* [x] 支持知识增量更新
* [x] 支持加载不同知识库
* [x] 支持检索结果与LLM生成结果对比
* [ ] 支持检索生成结果与原始LLM生成结果对比
* [ ] 支持模型问答与检索问答
* [ ] 检索结果过滤与排序
* [x] 互联网检索结果接入
* [ ] 模型初始化有问题
* [ ] 增加非LangChain策略
* [ ] 显示当前对话策略
* [ ] 构建一个垂直业务场景知识库，非通用性



## ❤️引用
- Chinese_LangChain：https://github.com/yanqiangmiffy/Chinese-LangChain
- webui参考：https://github.com/thomas-yanxin/LangChain-ChatGLM-Webui
- knowledge问答参考：https://github.com/imClumsyPanda/langchain-ChatGLM
- LLM模型：https://github.com/THUDM/ChatGLM-6B
- CSS：https://huggingface.co/spaces/JohnSmith9982/ChuanhuChatGPT
