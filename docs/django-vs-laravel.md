# Django Vs Laravel:选择哪个框架？

> 原文：<https://hackr.io/blog/django-vs-laravel>

尽管移动开发越来越流行，需求也越来越大，但是 web 开发已经得到了极大的关注，技术也在快速发展。Javascript 的迅速流行带来了很多东西，特别是随着新的开发概念的兴起，如渐进式 Web 应用程序、加速移动页面和单页面应用程序。然而，事情开始变得越来越复杂，尤其是对于刚刚起步的年轻开发人员。

可供选择的技术数量之多，它们提供的不同功能，每种技术的差异，以及 web 开发中没有圣杯，也没有适合所有人的解决方案的事实，所有这些都使得开始学习之旅变得非常可怕。

这就是为什么我们将试图揭开这个过程的神秘面纱，并在这里阐明这些不同的技术。web 开发世界中两个常见的技术是 Django 和 Laravel，它们是后端开发框架。

但是让我们慢下来，讨论一下什么是框架。

## 结构

框架是软件的抽象。抽象是缺乏复杂性和细节的核心概念。我们实际上在日常生活中处理抽象概念，而不仅仅是在软件中。例如，如果你想驾驶你的汽车，你不需要了解发动机的热力学和内部的能量循环，甚至不需要了解汽车的复杂力学，你只需要简单地控制方向盘。

在软件中使用这种抽象的好处是，它帮助年轻的开发人员快速进入游戏，并根据自己的需要使用专业开发人员创建的通用工具，因此他们不必在他们可能拥有的每个功能上重新发明轮子。

两个著名的软件抽象是库和框架。库是一组产生特定功能的方法/对象，你可以按照你认为合适的方式来使用，没有一种方法可以使用它。另一方面，框架是更严格的结构，是应用程序的骨架。

框架可以帮助您跳过开发底层基础设施的麻烦，直接进入应用程序的业务逻辑，从而得到更整洁、更专业的应用程序。

web 开发中基本上有两类框架:

### 前端框架

前端框架解决客户端开发问题，主要关注 CSS 或 JavaScript。现在的 [JavaScript 框架](https://hackr.io/blog/best-javascript-frameworks)比如 Vue。JS 和 Angular 是开发 web 应用的规范。

### 后端框架

后端框架负责服务器端的逻辑实现。发生在引擎盖下的魔法将你的网站凝聚在一起。如何处理数据，存储数据，如何管理响应等等。我们需要理解后端框架的一些核心功能。

路由:当你的服务器收到一个请求时，它会让某个资源或某个动作来处理它。如果你访问我的网站/产品，那么产品控制者应该用适当的资源回应，等等。

模板化:假设你不使用 Angular 和 Vue 之类的客户端框架。JS 然后你创建视图并用数据填充它们。视图基本上是用户在浏览器上看到的页面，模板化允许您根据控制器传递的数据动态地用数据填充页面。

请注意，还有许多其他的设计结构，每种结构都有自己处理视图及其数据的方式。

ORM: ORM 代表对象关系映射，它是模型和数据库之间的一层，充当虚拟对象数据库。

还有其他功能，如安全性、缓存、搭建和创建资源等等。

## 姜戈

Django 是一个用 python 构建的 MVT 或模型视图模板框架。这是一个免费的开源框架，鼓励快速开发，并帮助开发人员编写高效简洁的代码。这是一个非常强大的框架，被世界上一些最伟大的企业用作他们的后端基础设施。这些公司包括 Pinterest、Udemy、NASA 和 Instagram。

## 拉勒韦尔

Laravel 是用 PHP 构建的 MVC 或模型-视图-控制器框架，PHP 是最著名的 web 语言之一。这也是 9GAG，UNION，丰田名人堂使用的强大框架。

## Django vs Laravel 比较

让我们比较一下 Django 和 Laravel 的各种参数:

### 1.密码

让我们看看用两种语言编写的一些基本路由代码。乍一看，您可以注意到 Laravel 的代码相当直观。另一方面，Django 的代码看起来相当复杂，这是因为它在路由过程中使用了正则表达式，这不是最容易使用的，尤其是对于初学者。

例如:用两种语言对路由声明进行分页:

Php:

```
<? php Route:get('/', function() { return view('posts.index'); }); Route:get('/posts/create', function() { return view('posts.create'); }); ?>

```

Python:

```
urlptterns = [
 #ex: /polls/
 path('', view.index, name='index'),

 #ex: /polls/5/
 path('', view.detail, name='detail'),
 #ex: /polls/5/results/
]

```

Django 和 Laravel 社区都非常活跃，积极响应。这两个社区在 Github 上都有大量的贡献者，提交也非常频繁。如果您曾经在这些框架中的某个点上陷入困境，那么社区中的某个人肯定会把您带出来。

### 3.学习曲线

学习曲线有点神秘，因为它取决于个人。如果你对 Python 的语法相当熟悉，那么 Django 应该很容易掌握。它应该是开发人员友好的，不需要很长时间就能学会。如果你对 Django 感兴趣，这里有编程社区推荐的最好的 [Django 教程](https://hackr.io/tutorials/learn-django?ref=blog)。

据说 Laravel 的学习曲线很陡，但是有了 Laracasts 这样的工具和良好的文档，学习框架和掌握 PHP 语言应该一点也不困难。如果你对 Laravel 感兴趣，这里有编程社区推荐的最好的 [Laravel 教程](https://hackr.io/tutorials/learn-laravel?ref=blog)。

### 4.表演

Laravel 和 Django 在 2018 年针对 JSON 序列化进行了面对面的测试，因为 python 是一种非常快速的语言，所以它以压倒性的差异获胜。Django 每秒执行 69k JSON 响应，而 Laravel 每秒仅执行 8k 响应。在速度上，Laravel 比不上 Django，很遗憾。

[使用真实项目的 Fullstack Django 和 Python boot camp](https://click.linksynergy.com/link?id=jU79Zysihs4&offerid=1045023.2409312&type=2&murl=https%3A%2F%2Fwww.udemy.com%2Fcourse%2Ffullstack-django-and-python-bootcamp-with-real-life-projects%2F)

### 5.安全性

网络世界是一个充满敌意的环境，攻击和漏洞无时无刻不在被利用，这就是为什么框架需要针对不同的攻击采取措施，无论是 SQL 注入还是跨站点脚本。Django 非常重视安全性，帮助开发人员避免 web 开发中的常见错误，并实现一些安全最佳措施。虽然 Laravel 也涵盖了安全性的基础知识，但它没有达到 Django 的安全级别。这就是为什么，例如，美国宇航局使用 Django 作为他们的网站。

### 6.应用程序接口

您可能对后端框架必须提供的所有功能都不感兴趣，而更愿意用 RESTful API 构建一个客户端丰富的应用程序。Laravel 的美妙之处在于它内置了对 API 构建的支持，因为默认情况下查询会返回 JSON。Django 没有这个内置特性，你必须使用一个库来解决它并实现同样的特性。

## 总结一下:

| 技术 | 姜戈 | 拉勒韦尔 |
| 技术类型 | 用 python 构建的 MVT 框架 | 用 PHP 构建的 MVC 框架 |
| 安全性 | 高度安全的企业级应用 | 实现基本的安全功能 |
| GitHub Stars | 43,384 | 34,292 |
| 学习曲线 | 很容易学会 | 陡峭的学习曲线 |
| 表演 | 相当快 | 相对缓慢 |
| 网站数量 | 205,106 | 121,173 |
| 前端支持 | 用 Django 绑定前端 JS 框架相当复杂 | 支持 Vue。JS 开箱即用 |

请记住，这些框架支持大型网站，所以没有错误的选择。这完全取决于你的软件需求和你的设计。另外，[后端框架](https://hackr.io/blog/web-development-frameworks)在本质上非常相似，所以如果你想使用另一个框架，从一个框架转换到另一个框架并不困难。

无论您选择哪种框架，这里都有编程社区推荐的最佳教程和课程:

**人也在读:**