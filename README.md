## legado阅读3.0自动构建[![Android CI](https://github.com/10bits/gedoor-Build/workflows/Android%20CI/badge.svg)](https://github.com/10bits/gedoor-Build/actions)

> 默认从最新发布的tag构建,每次构建会自动清空18PlusList.txt

> 最新构建下载:[legado-3.21.032520.apk](https://github.com/10bits/gedoor-Build/releases/download/legado-3.21.032520/legado-3.21.032520.apk) 上次构建时间:2021-03-25 20:59:23
<!--start-->
> **2021/03/23**
> * 修复繁简转换“勐”“十”问题。使用了剥离HanLP简繁代码的民间库。APK减少6M左右
> * js添加一个并发访问的方法 java.ajaxAll(urlList: Array<String>) 返回 Array<StrResponse?>
> * 优化目录并发访问
> * 添加自定义epublib,支持epub v3解析目录。by ag2s20150909
<!--end-->
  
1. fork到你自己的仓库
2. 去你自己的仓库,点一下右上角star就会自动开始构建,已经star的点unstar,再点一下star就会进行新的构建,你的[Actions](https://github.com/10bits/gedoor-Build/actions)列表会有显示的
3. 每次构建完,apk会自动打包为`legado.apk.zip
`,去你自己的[Actions](https://github.com/10bits/gedoor-Build/actions)列表里找
4. 每次构建大概十几分钟,请耐心等待

## 如果你安装apk遇到以下问题

1. `安装失败(-102)`问题,给release apk增加了签名,已解决
2. `与已安装应用签名不同`问题,请卸载重新安装,已解决
3. `与已安装程序共存`问题,通过修改`applicationIdSuffix='.releaseA'`,已解决,不用卸载重装了
> 使用app过程中遇到问题,请到这里解决[gedoor/legado](https://github.com/gedoor/legado/issues)

