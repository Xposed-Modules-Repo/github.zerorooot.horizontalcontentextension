# 横屏传送门

强行在横屏模式下启用miui传送门

# 如何使用

1、安装[Magisk](https://github.com/topjohnwu/Magisk)

2、安装[LSPosed](https://github.com/LSPosed/LSPosed)

3、安装[miui传送门](https://github.com/zerorooot/HorizontalContentextension/blob/main/util/%E4%BC%A0%E9%80%81%E9%97%A8_2.5.18.apk)

4、安装此[app](https://github.com/zerorooot/HorizontalContentextension/blob/main/util/app)，并在LSPosed中勾选

5、使用[创建快捷方式](https://github.com/zerorooot/HorizontalContentextension/blob/main/util/%E5%88%9B%E5%BB%BA%E5%BF%AB%E6%8D%B7%E6%96%B9%E5%BC%8F.apk)，启用传送门，确保在竖屏模式下能正常使用

6、重启传送门，横屏，测试能否使用

# 软件原理

通过拦截`com.miui.contentextension.services.TextContentExtensionService`

类中的`isScreenPortrait`方法，使其返回`true`，从而达到横屏使用传送门的目的

# 注意

- miui没有给传送门在横屏下做适配，所以绝大部分功能在横屏下无法使用，但文字识别勉强正常，介意者慎用。

- miui没有给传送门在横屏下做适配，所以绝大部分功能在横屏下无法使用，但文字识别勉强正常，介意者慎用。

- miui没有给传送门在横屏下做适配，所以绝大部分功能在横屏下无法使用，但文字识别勉强正常，介意者慎用。

# 截图

文字识别，勉强能用

![勉强能用](https://github.com/zerorooot/HorizontalContentextension/raw/main/util/text.jpg)

图片识别，无法正常使用

![图片识别](https://github.com/zerorooot/HorizontalContentextension/raw/main/util/photo.jpg)
