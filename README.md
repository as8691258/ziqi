笔记项目
1、改变npm的库路径

npm config set registry https://registry.npm.taobao.org --global

npm config set disturl https://npm.taobao.org/dist --global

2、react native遇到的错误

react-native run-android 报错集合

1、 Could not create ADB Bridge.  ADB端口被占用，本人电脑是金山毒霸，解决方法：关闭后在重新编译即可

2、 Failed to execute aapt，保证build.gradle里面的 compileSdkVersion buildToolsVersion  dependencies三个地方有版本号的要一致

3、xxx.52.0错误为JDk版本不对，需要1.8的，环境变量也需要设置为1.8

4、Could not get BatchedBridge, make sure your bundle is packaged correctly   解决方法如下：
   
   http://www.open-open.com/lib/view/open1477469117948.html

react-native bundle --platform android --dev false --entry-file index.android.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res/ 

先创建assets目录


darwin-x64-48_binding.node安装不成功的解决方案
还有一种方式，先将darwin-x64-48_binding.node下载下来

再把它放到本地的服务器下，假设端口是8080, 通过http://localhost:8080/v3.10.0/darwin-x64-48_binding.node 能访问到就行
然后运行
npm install node-sass --save-dev --sass-binary-site=http://localhost:8080/ --registry=https://registry.npm.taobao.org

注意是–sass-binary-site=http://localhost:8080/
不用加后面的v3.10.0/darwin-x64-48_binding.node

react学习资料
http://huziketang.com/books/react/lesson1

