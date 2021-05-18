<p align="center"><img src="https://raw.githubusercontent.com/liangjingkanji/Net/master/docs/img/logo.gif" width="300"/>

<p align="center"><strong>不仅仅是网络请求的异步任务库</strong></p>

<p align="center"><a href="http://liangjingkanji.github.io/Net/">使用文档</a>
 | <a href="https://coding-pages-bucket-3558162-8706000-16642-587704-1252757332.cos-website.ap-shanghai.myqcloud.com/">备用访问</a>
 | <a href="https://coding-pages-bucket-3558162-8706000-17639-608061-1252757332.cos-website.ap-shanghai.myqcloud.com">Net2-文档</a>
</p>

<p align="center"><img src="https://i.imgur.com/X06J6fK.jpg" width="400"/></p>

<p align="center">
<a href="https://jitpack.io/#liangjingkanji/Net"><img src="https://jitpack.io/v/liangjingkanji/Net.svg"/></a>
<img src="https://img.shields.io/badge/language-kotlin-orange.svg"/>
<img src="https://img.shields.io/badge/license-Apache-blue"/>
<a href="http://liangjingkanji.github.io/Net/updates"><img src="https://img.shields.io/badge/updates-%E6%9B%B4%E6%96%B0%E6%97%A5%E5%BF%97-brightgreen"/></a>
<a href="https://jq.qq.com/?_wv=1027&k=vWsXSNBJ"><img src="https://img.shields.io/badge/QQ群-752854893-blue"/></a>
</p>

<p align="center"><img src="https://i.imgur.com/aBe7Ib2.png" align="center" width="30%;" /></p>

<br>

Android上不是最强网络任务库, 基于OkHttp且完美支持其所有函数组件, 支持协程高并发网络请求

<br>

Net 1.x 版本为RxJava实现 <br>
[Net 2.x](https://github.com/liangjingkanji/Net/tree/2.x) 版本为协程实现(开发者无需掌握协程也可以使用) <br>
Net 3.x 版本为OkHttp4.x实现

<br>
<p align="center"><strong>欢迎贡献代码/问题</strong></p>

<br>

主要功能

- Kotlin
- 协程(不懂协程也可上手)
- 并发网络请求
- 串行网络请求
- 快速切换线程
- DSL作用域编程
- 日志记录器(完美解决日志过长展示不清晰数据加密问题, 比抓包更强大)
- 并发请求返回最快请求结果
- 自动异常捕获
- 自动错误信息吐司
- 自动JSON解析
- 自动处理下拉刷新和上拉加载
- 自动处理分页加载
- 自动缺省页
- 自动处理生命周期
- 自动处理加载对话框
- 支持配合ViewModel
- 异常包含请求信息
- 数据转换器
- 请求存储键值对
- 请求支持Id/Group分组
- 全局手动取消请求/自动取消请求
- 协程作用域支持错误和结束回调
- 支持先强制读取缓存后网络请求二次刷新
- 内置超强轮循器(计时器)
- 解析JSON数组返回集合
- 监听上传/下载进度



<br>

在项目根目录的 build.gradle 添加仓库

```groovy
allprojects {
    repositories {
        // ...
        maven { url 'https://jitpack.io' }
    }
}
```

在 module 的 build.gradle 添加依赖

```groovy
// 协程库(版本可自定)
implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-core:1.3.9'
implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.3.9'

// OkHttp(版本可自定)
implementation "com.squareup.okhttp3:okhttp:4.9.1"

// Net
implementation 'com.github.liangjingkanji:Net:3.0.1'

// 支持自动下拉刷新和缺省页的(可选)
implementation 'com.github.liangjingkanji:BRV:1.3.19'
```

<br>

## Contribute

<img src="https://tva1.sinaimg.cn/large/006tNbRwgy1gaskr305czj30u00wjtcz.jpg" width="100"/> 

supported by [JetBrains](https://www.jetbrains.com/)


## License

```
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```