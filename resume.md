- ## 联系方式
  - 手机：17688758629
  - Email：loshine1992@gmail.com or 283946709@qq.com
  - QQ：283946709 （添加好友时请注明招聘）

  ---

  ## 个人信息

  - 龙帅/男/1992 
  - 本科/长沙理工大学 
  - 工作年限：10年
  - 技术博客：https://loshine.github.io/
  - GitHub：https://github.com/loshine

  - 期望职位：Android工程师、移动端工程师
  - 期望薪资：税前月薪30k~45k
  - 期望城市：上海
  - 额外技能：Rxjava, Kotlin, Flutter, Coroutines, Jetpack

  ---

## 工作经历

### 富乐康计算机（上海）有限公司 （ 2020年10月 ~ 至今 ）

LiveFuller 是富乐医疗 (Fullerton Health) 为新加坡当地客户提供的在线医疗解决方案，客户可以通过 LiveFuller 进行预约，在线问诊，处方开药，诊所查询等操作。

本人入职后主导了 LiveFuller App 三次较大的技术栈变化：

1. 从 Java MVP 迁移到 Kotlin MVVM，此阶段中本人参考现代化的 Kotlin Android 应用架构，设计了 MVVM 模式 + Repository 模式数据层的现代化 Android 应用，将 ARouter 多 Activity 跳转迁移到了按模块划分 Activity，模块内使用 Fragment 和 Jetpack Navigation 的路由方式。使用 Room 和 Retrofit 进行持久化存储和远程 API 访问，自定义 Interceptor 实现API鉴权等，此阶段主要解决 App 的技术债务，并引入流行的技术栈。
2. 尝试说服领导层使用 Flutter 来节约开发成本，并验证其可能性。该阶段本人在 LiveFuller App 内引入了 Flutter，使用 Flutter 引擎完成了业务较为独立的慢病管理模块的开发，在此阶段验证了其自定义UI和动画的便捷性、和原生互操作的能力、页面流畅不卡顿、并在开发速度上拥有一定的优势，在此阶段也解决了譬如原生和Flutter模块间数据同步的问题，原生和Flutter互跳转的问题，以及Flutter和原生互操作等问题。
3. 完全使用 Flutter 重构 LiveFuller，此阶段本人作为主开发和架构，设计了 LiveFuller Flutter 的架构，对业务模块进行了拆分，使用 Git 按模块开发的方式拆分业务和任务，使用 Riverpod 进行状态管理、dio 获取接口数据、flutter_hooks减少模板代码等。同时引入了stripe支付、fcm和hms(按手机品牌确定使用什么服务)、原生通知、Healthkit、Callkit 等插件和第三方库，并自行开发了如系统日历事件、Smart Future健康设备、android 通知、firebase 和 huawei 推送兼容库等第三方插件和库。该阶段使用四个月时间敏捷开发的模式，同时和原生应用并行，最终成功推进上线。

LFDoctor 是提供给诊所医生的在线接诊软件，此项目应用了 Jetpack Compose UI 重构界面层，将原项目中停止维护的 Android Router 库移除，大幅提升了项目的编译效率，并成功从命令式 UI 切换到了响应式 UI。项目数据层使用 Retrofit、Kotlin Serialization、Kotlin Coroutines、ViewModel、Flow、Coil、Room 等现代化库构建，使用 CompositionLocalProvider 实现了公司内部规范的主题以及控件，并接入了含RTC、IM、Firebase 等多项第三方服务，为医生提供了稳定、便捷的接诊和处方、发票开具方式。

![](https://i.imgur.com/9YVQYXq.png)

### 随机漫步（上海）体育科技有限公司 （2020年4月 ~ 2020年10月）

FREEBEAT 圆气健身是一款在线健身 App，用户可以使用它链接动感单车，蓝牙设备等观看在线课程并参与锻炼。

使用 Gradle 自定义插件和 ASM 字节码插桩技术，为公司实现了一套全埋点框架，使用注解可以静态或动态注入埋点统计参数。

优化了低功耗蓝牙连接，使用数据库缓存连接过的设备减少再次使用时的查找过程，优化用户连接流程。

参考 UI 设计绘制了大量自定义 UI 和动画效果。

### 上海厚翰科技有限公司 （ 2018年8月 ~ 2020年2月 ）

App 下载地址：

- Score: https://android.myapp.com/myapp/detail.htm?apkName=com.famulei.famulei
- We俱乐部: https://android.myapp.com/myapp/detail.htm?apkName=com.famulei.we
- iG俱乐部：https://android.myapp.com/myapp/detail.htm?apkName=com.famulei.ig
- OMG俱乐部：https://android.myapp.com/myapp/detail.htm?apkName=com.famulei.omg
- LNG俱乐部：https://android.myapp.com/myapp/detail.htm?apkName=com.famulei.snake
- 天霸电竞：http://zhushou.360.cn/detail/index/soft_id/4121841?recrefer=SE_D_%E5%A4%A9%E9%9C%B8%E7%94%B5%E7%AB%9E

Score 是电竞爱好者的粉丝社区，App 里提供了专业的英雄联盟、王者荣耀赛事数据，还可以在 App 里和同好一起观看赛事直播或赛事文字直播。

本人进入该公司时属于公司业务发展期，进入公司后本人组织了 Score 主版本和其它俱乐部单行版（WE俱乐部、iG俱乐部、OMG俱乐部、LNG俱乐部、滔博电竞、天霸电竞）的版本合并，使用`productFlavor`来管理不同单行版。

同时本人负责了项目架构改进，由传统的 MVC 架构调整为了较为容易学习使用的 MVP 架构，并引入了流行库如：Retrofit、RxJava 等。

后续本人和公司运维合作，使用 Jenkins 配合 Gradle 脚本实现了自动化打测试包，减少了开发人员的无效工作。后续使用 Gradle 脚本配合 360 加固实现了一键打包加固，大大减少了重复工作量，后续本人负责了Android发包工作，熟悉了国内绝大多数市场发包流程。

工作期间负责了多个模块的业务和代码重构，大幅提高了客户端稳定性，修复了多处隐藏的 bug 和逻辑漏洞。完全重构了发布贴子、文章页面，阅读贴子、文章页面以及赛事详情页面，优化了列表性能，提升了页面滚动流畅性。

在2019年引入了 Kotlin 技术栈，并实践 Kotlin 编码至今。

### 上海南花科技有限公司 （ 2017年5月 ~ 2018年7月 ）

![](https://s2.ax1x.com/2020/02/11/1TReVs.png)

职通车是基层岗位求职招聘服务平台，求职者和企业 HR 可以发送工作相关消息，直接聊天，火速入职。

本人加入项目时正是整个项目从 codova 向原生迁移之时，所以相当于使用 native 将现有的 app 重新实现了一遍。

因为是从零开始启动的项目，所以其技术栈统统采用了最新的 Android 技术，语言选择了特性更多的 Kotlin。

ui 层使用 MVVM 模式构建，将传统的集 View 和 Controller 为一体的 Activity 和 Fragment 抽象为普通的 View 层，在 ViewModel 中使用 RxJava 的 Subject 作为被观测的可变化数据，初始化时 View 监听 ViewModel 中的数据变化来改变 View 的状态，并在`onDestroy`时取消监听。

数据层采用 Repository 设计模式，在项目中作为一个 Android Library 引入主 app 项目。对外仅暴露方法而不暴露具体实现，实际 Repository 可能是 CloudRepository 或 DiskRepository，根据具体方法使用。数据的流动使用 Rxjava 传递，方便 ui 层的链式操作和线程切换。

网络访问使用 Rxjava、OkHttp、Retrofit、Gson 实现，使用拦截器注入了和后端约定好的请求头，使用 RxJava 处理了后端返回的逻辑、业务错误，并向上层传递。数据存储使用 Objectbox 非关系型数据库实现。

使用 Dagger 依赖注入实现了模块之间的解耦，把大多数可复用的对象使用`@Singleton`注解保证了其全局单例，减少了内存泄漏。使用了 Dagger-android 在 Android 组件内使用依赖注入，减少了 Dagger 模板代码。

使用 RxJava 封装了网易云信 sdk，使其返回数据为 RxJava 风格，并根据设计实现了即时通讯功能和界面，包括一对一聊天，自定义了多种消息类型，包括简历、确认接受简历、拒绝接受简历等等。

在内网搭建了 Jenkins 服务并部署了 Android 自动打包程序，在 github 上成功 push 代码之后触发 build，并在 build 成功之后发送邮件通知相关人员。失败之后将会发送错误日志到 Android 开发人员的邮箱。

### 深圳华海乐盈网络科技有限公司 （ 2014年10月 ~ 2017年5月 ）

#### 球苗社区客户端

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

#### 一比分

![](http://ww1.sinaimg.cn/large/0060lm7Tgy1fctb51frh5j314e0hsq92.jpg)

本人参与一比分开发的时候属于一比分的迭代期，主要负责新功能的开发以及现有模块的重构和维护。

参与开发期间把原来使用 Git 分支管理的多语言版本以及开发、测试、生产环境服务器都使用 Gradle 管理，使用 BuildTypes 以及 buildConfigField 管理不同 BuildType 的参数实现一次性打包不同环境的包。使用 productFlavors 实现多语言不同功能以及功能的实现。

重构了足球指数模块，将之前的 ListView 更换为 RecyclerView，并实现了 WebSocket 信息推送实时更新时只更新单条 Item，优化了 Fragment 内部逻辑，显著提升了页面滑动性能，不再卡顿。

编写了足球内页分析、情报、指数模块，根据 UI 的需求编写了自定义控件，其中碰到了一个文字不居中的问题，最终通过查阅资料发现是文字 top、ascent、descent、bottom 的差别导致的，然后顺利解决。

重构了篮球内页亚盘、欧赔、大小模块，渲染更迅速滑动更顺畅。

#### 一比分 Material Design 版

![](http://ww2.sinaimg.cn/large/0060lm7Tgy1fctb0h0hexj314h0hsafx.jpg)

这是初入公司时分配的 Demo 项目，主要是为了展示 Material Design 用在 Android 客户端上的效果。

大量使用了 design 库的控件以及 CoordinatorLayout 与 Behavior 的使用，使用 github 上的兼容库实现了设置界面的低版本 Material 兼容。

## 开源项目和作品

### 开源项目

- [flutter-nga](https://github.com/loshine/flutter-nga)：艾泽拉斯国家地理论坛 flutter 实现版，已停止维护
- [flutter-todo](https://github.com/loshine/flutter-todo)：一个学习 flutter 的 To-do 项目

## 技能清单

以下均为我熟练使用的技能

- 版本管理、文档和自动化部署工具：Svn/Git
- 单元测试：JUnit/Mockito/Robolectric
- 直播: RTMP 推流/播放

### 参考技能关键字

- Android
- Java
- Rxjava
- Kotlin
- Coroutines
- Jetpack Compose
- Flutter
- Dart
- Git
- SQL

---

## 致谢

感谢您花时间阅读我的简历，期待能有机会和您共事。
