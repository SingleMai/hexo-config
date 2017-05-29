---
title: Atom配置
date: 2017-05-20 15:53:58
categories: 工具配置
tags:
   - atom
---
Atom是一个很好用的编辑软件，可以让自己添加各种插件来辅助自己写代码。然而，有时候配置多了可能就忘了。所以特意建一个来保存自己的基础信息。（虽然说有插件可以实现转移，不过还是不放心吧。)
<!-- more -->
## keymap的配置
实现vue中支持emmet，和快捷键打开浏览器(需要先安装`open-in-browser`)。
```
./keymap.cson

'atom-text-editor':
  'ctrl-F12' : 'open-in-browser:open'
# 让vue文件里面支持emmet语法
'atom-text-editor[data-grammar~="vue"]:not([mini])':
  'tab': 'emmet:expand-abbreviation-with-tab'
```
## 代码高亮显示
vue代码高亮：
`language-vue-componment`
jade高亮：
`atom-jade`

## 辅助插件
emmet
`emmet-atom`
颜料
`atom-pignments`
`color-picker`
缩略图
`minimap`
文件图标
`file-icon`

## markdown
集各种功能的markdown编辑插件
`markdown-preview-enhanced`
