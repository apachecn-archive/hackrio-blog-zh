# Docker 是什么？深入了解 Docker 容器

> 原文：<https://hackr.io/blog/what-is-docker>

容器变得越来越受欢迎。这导致了基于容器化的工具的出现，最著名的是 Docker 和 Kubernetes。

前者是一个用于开发容器的免费开源工具(以及一套 PaaS 产品),而后者是一个开源的容器编排系统，提供了一种自动化管理、扩展和部署应用程序的方法。

在这篇文章中，我们将重点关注 Docker。容器可以理解为标准化的可执行组件，它将应用程序源代码与所有必需的操作系统库和依赖项打包在一起，以便在某些环境中运行应用程序。

在深入研究 Docker 之前，让我们先了解一下集装箱化的概念。

## 什么是集装箱化？

在计算科学中，容器被定义为包含关于应用程序及其所有依赖项的代码的包。

这带来了几个好处，比如快速执行和增强的可靠性。然而，最大的好处来自于平台独立性和改进的可访问性。

容器几乎可以在任何平台上使用，不用太担心硬件配置。对于解决由来已久的平台依赖性问题来说，这是一个巨大的飞跃。

容器映像是可执行的、轻量级的、独立的包。它们包括运行应用程序所需的一切:代码、运行时环境、设置、系统工具和库。它们在运行时成为容器。

例如，Docker 容器图像一旦开始在 Docker 引擎上运行，就变成了容器。不考虑基础设施，容器化的软件应用程序运行相同。容器将应用程序与环境隔离开来，以确保它们统一执行。

机器虚拟化允许多个虚拟机共享一台硬件服务器的资源。类似地，几个应用程序组件使用称为虚拟化的过程共享一个操作系统内核实例的资源。在容器的情况下，这是在操作系统级完成的。

### **容器 vs 虚拟机**

与虚拟机一样，容器可以经济高效地扩展，独立运行，并且易于处置。然而，操作系统级的额外抽象层带来了更多的好处。这些是:

*   **更高的开发效率:** 与虚拟机相比，容器的部署、供应和重启更加简单快捷。因此，它们是使用 [CI(持续集成)](https://en.wikipedia.org/wiki/Continuous_integration) 和 CD(持续交付)管道的更好选择。对于基于敏捷和 DevOps 的过程，它们也是更好的选择。
*   **更轻量:** 容器只包含流程及其相关的依赖项。另一方面，虚拟机有一个额外的操作系统实例。因此，对于相同的应用程序进程，容器比其虚拟机对手的容器更轻。
*   **卓越的资源利用率:** 像虚拟机一样，容器允许在同一硬件上多次运行一个应用程序进程的多个副本。然而，它们更节省资源。

## **Docker 是什么？-集装箱化的黄金标准**

Docker 是 Docker 公司的一个容器化平台。通过利用操作系统级虚拟化，它允许开发人员将应用程序打包到容器中。Docker 有助于构建、部署、运行、更新和管理容器。

集装箱化工具的特点是简单的命令和省力的自动化，在使用集装箱时节省了大量的精力和时间。尽管 Docker 是免费使用的开源软件，但它也有商业版本。

尽管集装箱运输自 70 年代就已出现，但它只是在最近才变得如此普遍。Docker 公司推广这一技术功不可没。

Linux 容器，或称 LXC，于 2008 年在 Linux 内核中实现。这为一个 Linux 实例启用了虚拟化。虽然 Docker 的早期版本使用 LXC，但它能够开发出超越 LXC 的独特集装箱化技术。

因此，期待学习集装箱化时，学习码头工人 有利于 [。Docker 的受欢迎程度可以很容易地通过今天 Docker 和 containers 可以互换使用的事实来衡量。](https://hackr.io/tutorials/learn-docker)

## **为什么是 Docker？**

当需要使用容器时，有几个令人信服的理由说明为什么应该使用 Docker。最重要的是:

*   **自动创建容器:**Docker 根据应用源代码，自动构建相关的容器。

*   **行业标准的创建者:** Docker，负责创建和设定集装箱的行业标准。
*   **粒度更新:** 每个 Docker 容器只有一个进程。这允许相关应用保持运行，即使当它的一部分，即进程，正在接收更新或经历修复。

*   **Docker 图像的海量存储库:**Docker 的用户可以免费访问一个开源注册表，该注册表存储了数万张用户提交的 Docker 容器图像。

*   轻量级——Docker 容器共享一台机器的操作系统内核，因此，不像虚拟机那样，每个应用程序都需要一个操作系统映像。这将提高服务器效率，并降低服务器和许可费用。

*   **最安全**——容器内的应用程序是安全的。Docker 提供了最强大的默认隔离功能。

*   **便携:** Docker 集装箱可以在任何地方使用。它们可以在任何云、桌面或移动环境中运行，无需任何修改。

*   **高级版本:** Docker 能够:

*   回滚到以前版本的容器映像。
*   跟踪 Docker 容器映像的版本是如何构建的以及是谁构建的。
*   跟踪 Docker 容器图像的版本。
*   仅上传 Docker 容器映像的现有版本和最新版本之间的差异。

*   **新容器的模板:** Docker 允许使用现有的 Docker 容器作为基础映像，即用于开发新容器的模板。

[Docker & Kubernetes:实用指南【2023 年版】](https://click.linksynergy.com/deeplink?id=jU79Zysihs4&mid=39197&murl=https%3A%2F%2Fwww.udemy.com%2Fcourse%2Fdocker-kubernetes-the-practical-guide%2F)

## **Docker 词汇表**

Docker 涉及很多专业术语和概念。为了充分理解 Docker 的概念，我们需要理解它们。以下是各种 Docker 术语的简要说明:

### **1。码头集装箱**

Docker 容器映像的运行实例是 Docker 容器。与容器映像不同，Docker 容器是瞬时的、实时的，并且具有可执行的内容。

关于 Docker 容器的条件和设置由管理员管理。这使得用户与相同的交互成为可能。

### **2。Docker 容器图像**

Docker 容器映像将可执行的应用程序源代码与所有的依赖项打包在一起，例如运行“包含的”应用程序所必需的工具和库。它是一个只读实体。

一旦 Docker 映像开始运行，它就成为容器的一个实例。同一 Docker 容器可以有一个或多个实例同时运行。

虽然从虚无中开发一个 Docker 映像很容易，但是从一个基础映像中创建一个要容易得多。甚至可以用一个基础映像创建多个 Docker 映像。在这种情况下，所有生成的 Docker 图像将共享其堆栈的几个特征。

这种易于开发的特性促使许多开发人员从开源/公共 Docker 库(如 Docker Hub)中提取基础映像。这些库被称为 Docker 注册表。

通常，一个 Docker 图像填充几层。每一层对应于开发人员进行更改的时间。因此，顶层对应于对 Docker 容器映像所做的最新更改。

的确，这是一个非常有用的功能，可以在不愉快的情况下回滚到 Docker 映像的先前版本，包括失败或者事情没有按照预期的方式发展。此外，也有可能在其他项目中使用它们。谈一石二鸟。

当 Docker 映像运行时，即形成 Docker 容器时，形成的最顶层被称为容器层。对容器所做的所有更改都保存在容器层中，并且只在容器的生命周期内存在，即直到它运行。

由于上述原因，从单个基础映像运行多个容器实例可以提高整体效率。

### **3。DockerFile**

Docker file是一个纯文本文件，包含构建 Docker 容器映像的指令。每个 Docker 容器都有一个 DockerFile 。它自动化了创建 Docker 映像的整个过程。

Docker 引擎负责组装 Docker 容器映像。相关的 DockerFile 有所有的命令和特定的序列，帮助 Docker 引擎建立 Docker 容器映像。

### **4 .码头枢纽〔t1〕**

Docker Hub 自称是最大的容器图片社区和图书馆，是 Docker 图片的最高储存库。回购的提交通常由:

*   商业软件厂商
*   开源项目团队
*   个人开发者

公共存储库还包含经 Docker 可信注册中心认证的 Docker 容器映像。由于它是一个公共的 Docker 库，用户可以随时随意地拉或推图片。

[Docker 认证助理:硕士课程【2023 版】](https://click.linksynergy.com/link?id=jU79Zysihs4&offerid=1045023.2074534&type=2&murl=https%3A%2F%2Fwww.udemy.com%2Fcourse%2Fdocker-certified-associate%2F)

## **Docker 组件**

码头工人 SaaS 有三个组成部分:

### **1。Docker 对象**

为了在 Docker 中组装应用程序，使用了 Docker 对象。Docker 对象主要有三类:

*   Docker 容器: 这些是运行应用程序的标准化隔离环境。Docker API 或 CLI 负责管理 Docker 容器。

*   **Docker 图片:** 用于构建 Docker 容器的只读模板。使用 Docker 映像来运输和存储应用程序。
*   **Docker 服务:** 允许跨多个 Docker 守护进程扩展 Docker 容器。一组通过 Docker API 进行通信的协作 Docker 守护进程被称为 群 。

### **2。码头登记处**

Docker 映像的存储库称为 Docker 注册表。这些可以是公共的(任何人都可以访问)，也可以是私有的(只有授权的人才能访问)。默认注册中心 Docker Hub 和 Docker Cloud 是两个领先的公共 Docker 注册中心。

Docker 客户端连接到 Docker 注册表，以获取(下载)或推送(上传)Docker 映像。也可以使用 Docker 注册表创建基于事件的通知。

### **3 .码头守护程式**

被称为的 Docker 守护进程是一个持久进程。它负责管理 Docker 容器和处理容器对象。它还监听通过 Docker 引擎 API 发送的请求。

用户和 Docker 守护进程之间的间隙是使用 Docker 客户端程序来实现的。它被标记为 Docker 并带有命令行界面。

## **坞站组成**

Docker Compose 是一款帮助定义和运行多容器应用的工具。它创建 YAML 文件，允许只使用一个命令部署和运行容器。这些还指定了相关应用程序中包含的服务。

docker-compose . yml文件有助于定义应用程序的服务，还包括配置选项。Docker Compose 适用于管理由驻留在几个容器中的进程构建的应用程序的架构，所有这些进程都存在于一个主机上。它允许:

*   定义持久存储卷，
*   记录和配置服务依赖关系，以及
*   指定基节点。

docker-compose CLI使用户能够同时在几个容器上运行命令。这些命令通常包括:

*   建筑图像
*   缩放容器
*   运行容器

在 Docker Compose 中，图像处理和用户交互选项等命令是不相关的。这是因为这些命令只对一个容器有效。

## **部署和协调**

当只有几个容器运行时，Docker 引擎足以管理一个应用程序。不需要额外工具。然而，当部署有数千甚至更多的容器和数百个服务时，就需要额外的工具。

在这样的场景中，需要一个编排工具。两个最流行的工具是 Docker 自己的 Docker Swarm 和管理多容器环境的最佳工具 Kubernetes。

Docker Swarm 为 Docker 容器提供本地集群功能，将多个 Docker 引擎合并为一个虚拟 Docker 引擎。群体模式集成在 Docker 引擎中。 docker swarm CLI 为一系列任务提供支持，包括:

*   创建发现令牌，
*   运行 Swarm 容器，以及
*   列出集群中的各个节点。

为了管理集群，即协作 Docker 守护进程的集合，Docker 利用了 Raft 一致性算法。它声明当大多数群节点同意更新时，执行更新。

Kubernetes 是一个开源的容器编排系统，可以自动化管理、扩展、路由等。集装箱。虽然最初是由科技巨头谷歌开发的，但它的进一步发展掌握在 CNCF(云计算原生计算基金会)手中。

尽管有 Docker Swarm，但 Kubernetes 是管理基于 Docker 容器化的多容器环境的最佳选择。开发者更喜欢一前一后地使用 [Kubernetes 和](https://hackr.io/blog/kubernetes-vs-docker#the-synergy-among-docker-and-kubernetes)Docker。Docker 桌面以其 Kubernetes 发行版为特色。

在 Docker-Kubernetes 系统中，Docker 是打包和发布应用程序的工具，而 Kubernetes 是部署和扩展应用程序的工具。

## **结论**

总结了这篇详细的文章。本质上，它是利用操作系统级虚拟化的最流行的容器化工具。集装箱化正成为最热门的 IT 技术之一。随着它的持续增长，对 Docker 的需求也在增长。

你认为集装箱化技术怎么样？值得你花时间吗？请通过下面的评论让我们知道。你认为你了解多克吗？用这些顶级 [Docker 面试题](https://hackr.io/blog/docker-interview-questions) 来考核你的知识。

**人也在读:**