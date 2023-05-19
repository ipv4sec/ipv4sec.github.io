---
title: "Flutter之路"
date: 2023-04-26T22:43:32+08:00
draft: true
---

### 安卓平台图片加载顺序

1. `/android/app/src/main/res/`路径下, 如果手机版本为`7.0`, 则优先`drawable-v24`路径下查找, 其次`drawable-v21`, 再`drawable`
2. 优先当前手机分辨率`xxhdpi`,先查找当前`drawable-xxhdpi`, 再更高`drawable-xxxhdpi`, 再无`drawable-nodpi`, 再更低`drawable-xhdpi`,`drawable-hdpi`,`drawable-mdpi`,`drawable-ldpi` 

### 安卓平台打包之路

待整理

### 视窗平台打包之路

1. 构建`flutter build windows`
2. 产出`<project>/..build/windows/runner/release/`
3. 下载[Inno Setup](https://jrsoftware.org/isdl.php)
4. 打包教程 [链接](https://web.archive.org/web/20221128124401/https://protocoderspoint.com/how-to-create-exe-installation-file-of-flutter-windows-application/)

### 常用的依赖库

1. [](https://pub.flutter-io.cn/packages/flutter_launcher_icons)
2. [](https://pub.flutter-io.cn/packages/flutter_launcher_name)
3. [](https://pub.dev/packages/easy_permission)
4. [](https://pub.dev/packages/permission_handler)


### 常见操作

1. [向应用添加启动页](https://flutter.cn/docs/development/ui/advanced/splash-screen)