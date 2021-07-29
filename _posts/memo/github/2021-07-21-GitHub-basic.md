---
layout: page_memo_jp
title_jp: "GitHub 基本"
year: 2021
tag: memo
category: jp
cont: GitHub
---


---

---
## 特定のディレクトリを除外して push する方法
---
#### **目的**
あるプログラムの作成が終わり，試行錯誤をしていくうちに余分な解析結果が増えてきたため，余分なファイルを一つのディレクトリにまとめて，GitHubのレポジトリへ反映時にそのディレクトリを除外したい．

#### **方法：.gitignore の不可視ファイルを作る**

例えば，*~/githome* がディレクトリの一番上の階層だとして *~/githome/trash* を除外したい場合，*~/githome/.gitignore* を作成して，
~~~
trash
~~~
と書いておく．これで push すると，*trash* ディレクトリはレポジトリに反映されず，反対に，*.gitigore* のファイルがレポジトリの最上階層に反映されている．

[参考にしたサイト] 
[https://fantastech.net/gitignore](https://fantastech.net/gitignore)