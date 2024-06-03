---
title: 'pythonで簡単にGUIが作れるFletを使ってみよう'
description: 'これ、最高です。'
slug: flet-tutorial
image: cover.jpeg
keywords: ["python","flet","GUI","解説"]
tags: ['こんにちは']
categories: ['Python']
date: 2024-06-04T06:43:47+09:00
draft: true
---
## PythonでのGUI
PythonでGUIを作る時、ライブラリの選択肢がまぁまぁあります。  
今回はfletを使用しますが、tkinterやPyQTとか。  
様々あるんですけどね、使っていて一番楽だったのがこのfletだったのでこれを布教しようっていう記事です。  

## Fletのインストール
```
pip install flet
```
です。  
まぁ簡単ですね。

## 基本の書き方
### ウィンドウを作ろう
```python
import flet as ft


def main(page: ft.Page):
    page.title = "Flet Demo"

    text = ft.Text("こんにちは")

    page.add(
        text
    )


ft.app(main)
```
これを実行すると  
![](2024-06-04-08-31-36.png)

こんな感じの見た目のウィンドウが作成できます。  
