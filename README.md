---
title: '錄音辨識指令控制PPT'
disqus: hackmd
---

錄音變識指令控制PPT
===

## 內容

[TOC]

### 1. 架構圖
![](https://i.imgur.com/Kax8pcV.png)



### 2.開發環境介紹
分為以下兩端
#### APP端：
```gherkin=
發開語言：kotlin
Android studio 模擬器版本：如下圖
```
![](https://i.imgur.com/yBfvuXu.png)
#### 控制PPT service：
```gherkin=
發開語言：python
```
若要製作出.exe請按照下列步驟
```gherkin=
$ pip install pyinstaller  
$ ./build_exe.sh
注意：各作業系統編譯出來的.exe不能相容
```


## 2.開發環境介紹
程式碼下載
(1) 直接使用repo 下載整包專案
```gherkin=
$ mkdir project
$ cd project
$ repo init -u git@github.com:masteree108/Voice_test_plane.git -b main
$ repo sync 
$ repo start main --all
```
(2) 各別下載,請致下列的github
#### APP端：
```gherkin=
https://github.com/masteree108/OS_MediaRecorder
$ git clone https://github.com/masteree108/OS_MediaRecorder.git
```
#### 控制PPT service：
```gherkin=
https://github.com/masteree108/OS_PPT_control
$ git clone https://github.com/masteree108/OS_PPT_control.git
```