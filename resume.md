- # 联系方式
  - 手机：18664605062
  - Email：loshine1992@gmail.com or 283946709@qq.com
  - QQ：283946709 （添加好友时请注明招聘）

  ---

  # 个人信息

  - 龙帅/男/1992 
  - 本科/长沙理工大学 
  - 工作年限：3年
  - 技术博客：https://loshine.xyz/
  - GitHub：http://github.com/loshine

  - 期望职位：Android工程师、移动端工程师
  - 期望薪资：税前月薪15k~25k
  - 期望城市：上海

  ---

# 工作经历

## 上海南花科技有限公司 （ 2017年5月 ~ 至今 ）

![](https://ws1.sinaimg.cn/large/006tKfTcgy1fpeth803xpj30ih0ihtd3.jpg)

职通车是基层岗位求职招聘服务平台，求职者和企业 HR 可以发送工作相关消息，直接聊天，火速入职。

本人加入项目时正是整个项目从 codova 向原生迁移之时，所以相当于使用 native 将现有的 app 重新实现了一遍。

因为是从零开始启动的项目，所以其技术栈统统采用了最新的 Android 技术，语言选择了特性更多的 Kotlin。

ui 层使用 MVVM 模式构建，将传统的集 View 和 Controller 为一体的 Activity 和 Fragment 抽象为普通的 View 层，在 ViewModel 中使用 RxJava 的 Subject 作为被观测的可变化数据，初始化时 View 监听 ViewModel 中的数据变化来改变 View 的状态，并在`onDestroy`时取消监听。

数据层采用 Repository 设计模式，在项目中作为一个 Android Library 引入主 app 项目。对外仅暴露方法而不暴露具体实现，实际 Repository 可能是 CloudRepository 或 DiskRepository，根据具体方法使用。数据的流动使用 Rxjava 传递，方便 ui 层的链式操作和线程切换。

网络访问使用 Rxjava、OkHttp、Retrofit、Gson 实现，使用拦截器注入了和后端约定好的请求头，使用 RxJava 处理了后端返回的逻辑、业务错误，并向上层传递。数据存储使用 Objectbox 非关系型数据库实现。

使用 Dagger 依赖注入实现了模块之间的解耦，把大多数可复用的对象使用`@Singleton`注解保证了其全局单例，减少了内存泄漏。使用了 Dagger-android 在 Android 组件内使用依赖注入，减少了 Dagger 模板代码。

使用 RxJava 封装了网易云信 sdk，使其返回数据为 RxJava 风格，并根据设计实现了即时通讯功能和界面，包括一对一聊天，自定义了多种消息类型，包括简历、确认接受简历、拒绝接受简历等等。

## 深圳华海乐盈网络科技有限公司 （ 2015年12月 ~ 2017年5月 ）

### 球苗社区客户端

![](http://ww3.sinaimg.cn/large/0060lm7Tgy1fctbaujf86j314h0hsq9s.jpg)

球苗社区客户端是一款体育IP社区APP。它主要包含了首页、视频、同城、我的四大模块，本人在项目创立之初就加入了项目团队，负责参与需求评审、商讨 API 细节、Android 客户端技术选型、搭建项目基本架构以及参与业务编码。

球苗社区采用 MVP + Databinding 架构实现，其 Data 模块使用 RxJava、Retrofit、OkHttp、Gson、Realm 实现，使用 Dagger2 依赖注入以实现各模块之间的解耦，Data 模块中的数据都以流的形式传输。

因为与服务端约定了在 HTTP 请求头中携带大量参数，自定义了 OkHttp 的 Interceptor（拦截器）实现了请求头参数的传递。为了优化网络情况，定义了一个缓存拦截器，使用 Cache-Control 请求头实现了网络请求的缓存。

UI 部分大量使用了 design 包的新控件，使用 CoordinatorLayout 作为基础布局，使用 RecyclerView 实现列表、网格、流式布局。

封装了 BaseActivity、BaseFragment、BasePresenter，定义了 IView、IPresenter 接口，各模块间使用 Contract（契约类）定义模块的 View、Presenter 方法，并使用 Dagger2 依赖注入。

UI 部分大量使用 Fragment，并使用 Databinding 实现数据绑定，减少大量代码。

仿照微信图片选择器实现了一个类似的图片选择器，方便了图片、视频的选择。

由于用户发帖时有视频压缩的需求，于是在开发期间查阅了大量资料，最后采用了 ffmpeg 的方式对视频质量、大小进行压缩，最终实现了功能。

开发了 RTMP 直播推流和播放功能，接入腾讯云直播 sdk，能够顺利推流和播放。

### 一比分

![](http://ww1.sinaimg.cn/large/0060lm7Tgy1fctb51frh5j314e0hsq92.jpg)

本人参与一比分开发的时候属于一比分的迭代期，主要负责新功能的开发以及现有模块的重构和维护。

参与开发期间把原来使用 Git 分支管理的多语言版本以及开发、测试、生产环境服务器都使用 Gradle 管理，使用 BuildTypes 以及 buildConfigField 管理不同 BuildType 的参数实现一次性打包不同环境的包。使用 productFlavors 实现多语言不同功能以及功能的实现。

重构了足球指数模块，将之前的 ListView 更换为 RecyclerView，并实现了 WebSocket 信息推送实时更新时只更新单条 Item，优化了 Fragment 内部逻辑，显著提升了页面滑动性能，不再卡顿。

编写了足球内页分析、情报、指数模块，根据 UI 的需求编写了自定义控件，其中碰到了一个文字不居中的问题，最终通过查阅资料发现是文字 top、ascent、descent、bottom 的差别导致的，然后顺利解决。

重构了篮球内页亚盘、欧赔、大小模块，渲染更迅速滑动更顺畅。

### 一比分 Material Design 版

![](http://ww2.sinaimg.cn/large/0060lm7Tgy1fctb0h0hexj314h0hsafx.jpg)

这是初入公司时分配的 Demo 项目，主要是为了展示 Material Design 用在 Android 客户端上的效果。

大量使用了 design 库的控件以及 CoordinatorLayout 与 Behavior 的使用，使用 github 上的兼容库实现了设置界面的低版本 Material 兼容。

## 武汉申氏传媒有限公司 （ 2014年10月 ~ 2015年11月 ）

### 众豆网 Android 客户端、众豆网后端

![](http://ww1.sinaimg.cn/large/0060lm7Tgy1fctaokt8sej30ue0hqqfc.jpg)

本项目是独立开发，由于项目需要快速开发快速迭代所以使用了 Android Annotations 框架。使用了 Retrofit + Fastjson + OkHttp 进行网络访问，由于 Retrofit 没有 fastjson 的 adapter，于是自己参照 GsonAdapter 自行实现了一个 FastjsonAdapter。

MainActivity 采用 Fragment + RadioGroup 的方式实现，项目使用 MVC 架构，用户登录 token 缓存在 SharedPreferences 中以保证移动端 always online。

由于公司后端开发人手不足，所以在此期间也参与了后端的开发，使用 Spring、Spring MVC、Mybatis 进行开发，API 使用了 Restful 风格。

在此期间也学习了 MySQL 的使用和 SQL 语句的编写，Spring MVC 以及 Spring 依赖注入，并理解了 IOC、AOP 的含义。能够熟练使用 SSI 框架进行 Web 开发。

# 其它项目经验

在业余时间参与了深圳大学大数据技术与应用研究所的项目，参与了其跨平台应用的开发。

## mekongchat

深圳大学大数据技术与应用研究所基于其 app-hybrid-core 开发的一款即时通讯项目，主要负责接入环信 SDK 并提供给 hybrid 调用的接口。

# 开源项目和作品

## 开源项目
- [retrofit_fastjson_converter](https://github.com/loshine/retrofit_fastjson_converter)：一个 fastjson 的 retrofit convertor factory
- [GalleryPicker](https://github.com/loshine/GalleryPicker)：仿微信图片选择器的实现

## 技术文章

- [Android开发最佳实践——1.接口设计](https://loshine.me/2016/09/01/android-best-practice-p1-interface-design/)
- [Android开发最佳实践——2.使用Kotlin开发Android](https://loshine.me/2016/09/06/android-best-practice-p2-language/)
- [Android开发最佳实践——3.项目架构篇](https://loshine.me/2016/11/17/android-best-practice-p3-project-architechture/)
- [Android开发最佳实践——4.Repository 层实现](https://loshine.me/2017/01/21/android-best-practice-p4-repository/)

# 技能清单

以下均为我熟练使用的技能

- 版本管理、文档和自动化部署工具：Svn/Git
- 单元测试：JUnit/Mockito/Robolectric
- 直播: RTMP 推流/播放

## 参考技能关键字

- android
- rxjava
- java
- kotlin
- javascript
- git
- sql

---

# 致谢

感谢您花时间阅读我的简历，期待能有机会和您共事。
