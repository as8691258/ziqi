笔记项目
1、改变npm的库路径

npm config set registry https://registry.npm.taobao.org --global

npm config set disturl https://npm.taobao.org/dist --global

2、react native遇到的错误

react-native run-android 报错集合

1、 Could not create ADB Bridge.  ADB端口被占用，本人电脑是金山毒霸，解决方法：关闭后在重新编译即可

2、 Failed to execute aapt，保证build.gradle里面的 compileSdkVersion buildToolsVersion  dependencies三个地方有版本号的要一致

3、xxx.52.0错误为JDk版本不对，需要1.8的，环境变量也需要设置为1.8


