## 思维导航

* [前言](https://github.com)
* [.NET常见的几种项目架构模式](https://github.com)
* [整洁架构](https://github.com)
* [.NET 整洁架构模板](https://github.com)
* [项目源代码](https://github.com)
* [环境准备](https://github.com)
* [.NET 整洁架构模板安装](https://github.com)
* [项目源码地址](https://github.com)
* [优秀项目和框架精选](https://github.com)

## 前言


项目架构模式在软件开发中扮演着至关重要的角色，它们为开发者提供了一套组织和管理代码的指导原则，以提高软件的可维护性、可扩展性、可重用性和可测试性。今天大姚给大家分享一个适用于 .NET 的开源整洁架构项目模板。


:[milou云加速器官网](https://jiechuangmoxing.com)## .NET常见的几种项目架构模式


[https://mp.weixin.qq.com/s/kr1vlt4tj3dSyXyRv\-GqOw](https://github.com)


![](https://img2024.cnblogs.com/blog/1336199/202501/1336199-20250110131517531-491450127.png)


## 整洁架构


整洁架构（Clean Architecture）是一种软件架构设计原则，由罗伯特·C·马丁（Robert C. Martin）提出，它旨在使软件系统更加灵活、可维护和可测试，其核心目标是构建一种简洁、灵活且易于维护的系统结构。


![](https://img2024.cnblogs.com/blog/1336199/202501/1336199-20250110131530161-636876451.png)


### 分层职责


* 实体层（Entities）：实体层代表了系统中的核心业务概念和对象。这一层包含了那些在整个系统的生命周期中持续存在且具有明确业务含义的实体。
* 用例层（Use Cases）：用例层包含了系统的具体业务逻辑和用例。它协调实体层和其他层之间的交互，以实现特定的业务功能。
* 接口适配器层（Interface Adapters）：接口适配器层将用例层与外部系统（如数据库、用户界面、外部服务等）进行连接。它将外部系统的接口转换为用例层可以理解的形式，并将用例层的输出转换为适合外部系统的格式。
* 框架与驱动层（Frameworks and Drivers）：框架与驱动层包含了外部的框架和工具，如数据库、Web 框架、消息队列等。这一层通常是由具体的技术实现组成，为上层提供基础设施支持。


## .NET 整洁架构模板


`CleanArchitecture`是一个适用于 .NET 的开源整洁架构项目模板，此模板的目标是利用 Clean Architecture 和 ASP.NET Core 的强大功能，为企业应用程序开发提供一种简单而有效的方法。使用此模板，您可以毫不费力地使用 ASP.NET Core 和 Angular 或 React 创建单页应用程序 （SPA），同时遵守 Clean Architecture 的原则。入门非常简单，只需安装 .NET 模板。


## 项目源代码


![](https://img2024.cnblogs.com/blog/1336199/202501/1336199-20250110131545329-1440800780.png)


## 环境准备


### .NET 9\.0 SDK


* https://dotnet.microsoft.com/zh\-cn/download/dotnet/9\.0


![](https://img2024.cnblogs.com/blog/1336199/202501/1336199-20250110131600648-1201627287.png)


### Node.js


* https://nodejs.org


![](https://img2024.cnblogs.com/blog/1336199/202501/1336199-20250110131612912-1681996602.png)


## .NET 整洁架构模板安装


Clean.Architecture.Solution.Template：


* https://www.nuget.org/packages/Clean.Architecture.Solution.Template



```
dotnet new install Clean.Architecture.Solution.Template::9.0.8

```

整洁架构模板安装后，使用模板创建新的解决方案。您可以选择使用 Angular、React 或创建仅限 Web API 的解决方案。使用 \-cf 或 \-\-client\-framework 选项指定客户端框架，并提供将在其中创建项目的输出目录。以下是一些示例：


要使用 Angular 和 ASP.NET Core 创建单页应用程序 （SPA）：



```
dotnet new ca-sln --client-framework Angular --output YourProjectName

```

要使用 React 和 ASP.NET Core 创建 SPA，请执行以下操作：



```
dotnet new ca-sln -cf React -o YourProjectName

```

若要创建仅限 ASP.NET Core Web API 的解决方案，请执行以下操作：



```
dotnet new ca-sln -cf None -o YourProjectName

```

启动应用程序：



```
cd src/Web
dotnet run

```

## 项目源码地址


更多项目实用功能和特性欢迎前往项目开源地址查看👀，别忘了给项目一个Star支持💖。


* GitHub开源地址：[https://github.com/jasontaylordev/CleanArchitecture](https://github.com)


## 优秀项目和框架精选


该项目已收录到C\#/.NET/.NET Core优秀项目和框架精选中，关注优秀项目和框架精选能让你及时了解C\#、.NET和.NET Core领域的最新动态和最佳实践，提高开发工作效率和质量。坑已挖，欢迎大家踊跃提交PR推荐或自荐（让优秀的项目和框架不被埋没🤞）。


* GitHub开源地址：[https://github.com/YSGStudyHards/DotNetGuide/blob/main/docs/DotNet/DotNetProjectPicks.md](https://github.com)
* Gitee开源地址：[https://gitee.com/ysgdaydayup/DotNetGuide/blob/main/docs/DotNet/DotNetProjectPicks.md](https://github.com)


 
