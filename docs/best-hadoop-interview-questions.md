# 2023 年 50 个最佳 Hadoop 面试问答[更新]

> 原文：<https://hackr.io/blog/best-hadoop-interview-questions>

Apache Hadoop 是最受欢迎的生产大数据的开源项目之一。它是一项强大的技术，允许组织和个人以高效的方式从大量数据(尤其是非结构化数据)中挖掘出意义，同时保持成本效益。

IT 部门中与大数据相关的几个职位要求对 Apache Hadoop 有很好的理解。

## 热门 Hadoop 面试问题和答案

如果你正在准备这样的面试，这里有一些最好的 Hadoop 面试问题，可以帮助你做同样的准备，或者评估你到目前为止的进步:

#### **问题:什么是 Hadoop？说出它的组成部分。**

**回答** : Apache Hadoop 是一个开源软件框架，提供大量工具和服务来存储和处理大数据。决策者利用 Hadoop 来分析大数据，并做出合适的业务决策。Hadoop 具有以下组件:

*   处理框架

*   故事
*   资源管理器
*   节点管理器

*   存储单元

#### **问题:C** **比较关系数据库管理系统和 HDFS (Hadoop 分布式文件系统)？**

**回答**:以下是 HDFS 和 RDBMS 的各种区别:

*   **数据存储** -在 RDBMS 中，数据的模式总是已知的，并且只存储结构化数据。相反，Hadoop 可以存储结构化、半结构化甚至非结构化的数据。
*   **处理能力**-RDBMS 几乎没有处理能力。另一方面，Hadoop 允许处理跨 Hadoop 集群并行分布的数据。
*   模式方法——HDFS 和 RDBMS 的另一个主要区别是模式方法。RDBMS 遵循传统的写模式方法，即在加载数据之前验证模式，而 HDFS 遵循现代的读模式方法。
*   **读/写速度**-RDBMS 中的读取速度很快，因为模式是已知的。Hadoop 有助于加快写入速度，因为在 HDFS 写入过程中没有模式验证。
*   **定价** -大多数 RDBMSs 都是付费软件。相反，Hadoop 是一个开源框架，有一个广泛的社区和大量的附加软件，如工具和库。
*   **理想用途**-RDBMS 的使用仅限于 OLTP 系统。然而，Hadoop 可以用于数据发现、分析、 [OLAP 系统](https://hackr.io/blog/olap-vs-oltp)等。

#### **问题:** **请解释一下 HDFS 和纱？**

**回答** : HDFS 或 Hadoop 分布式文件系统是 Apache Hadoop 的存储单元。按照主/从拓扑结构，HDFS 在分布式环境中将多种形式的数据存储为数据块。它有两个组成部分:

1.  **NameNode** -它是维护与存储的数据块相关的元数据的主节点。
2.  **DataNodes** -在 HDFS 中存储数据的从节点。所有 DataNodes 都由 NameNode 管理。

另一个资源协商者或 YARN 是在 Hadoop 2 中引入的 Apache Hadoop 的处理框架。它负责管理资源，并为流程提供执行环境。纱线由两部分组成:

1.  **resource manager**——接收处理请求，然后将请求部分地传递给相关的节点管理器。还根据应用程序的需求为其分配资源。
2.  **node manager**——安装在每个 DataNode 上，负责执行任务。

#### **问题:E** **解释各种 Hadoop 守护进程？**

**回答**:一个 Hadoop 集群中共有 6 个 Hadoop 守护进程:

1.  **NameNode****——这是存储 Hadoop 集群所有目录和文件元数据的主节点。包含有关块及其在群集中的位置的信息。**
***   **DataNode(s)** -存储实际数据的从节点。数量上的倍数。*   **二级 NameNode** -定期将更改-编辑日志-与 NameNode 中的 FsImage 合并。由次命名节点存储在永久存储器中的修改后的 FsImage 可以用在涉及命名节点故障的场景中。*   **ResourceManager** -负责管理资源以及调度运行在 YARN 上的应用程序。*   **节点管理器** -负责:

1.  启动应用程序的容器
2.  监控前述的资源使用情况
3.  向 ResourceManager 报告其状态和监视细节

*   **JobHistoryServer** -在应用程序主服务器终止后维护有关 MapReduce 作业的信息**

 **NameNode、DataNode 和辅助 NameNode 是 HDFS 守护程序，而 ResourceManager 和 NodeManager 是 YARN 守护程序。

### 推荐课程

[Hadoop 的终极实践:驯服您的大数据！](https://click.linksynergy.com/deeplink?id=jU79Zysihs4&mid=39197&murl=https%3A%2F%2Fwww.udemy.com%2Fcourse%2Fthe-ultimate-hands-on-hadoop-tame-your-big-data%2F)

#### **问题:** **简单解释一下** **Hadoop 架构** **？**

**回答** : [Apache Hadoop 架构](https://hackr.io/blog/hadoop-architecture)，又名 Hadoop 分布式文件系统或 HDFS 遵循主/从架构。这里，一个集群包含一个 NameNode 或主节点，所有剩余的节点都是 DataNodes 或从节点。

NameNode 包含有关存储数据的信息，即元数据，而 DataNodes 是数据在 Hadoop 集群中的实际存储位置。

#### **问题:****HDFS 和 NAS(网络附加存储)有什么区别？**

**回答**:以下是 HDFS 和 NAS 的重要区别点:

**1。定义**

网络附加存储是连接到某个计算机网络的文件级计算机数据存储服务器。简单地说，NAS 可以是一些提供存储和访问数据文件服务的软件或硬件。

另一方面，Hadoop 分布式文件系统是一种通过商用硬件存储数据的分布式文件系统。

**2。数据存储**

虽然数据存储在 NAS 的专用硬件上，但 HDFS 以数据块的形式存储数据，这些数据块分布在组成 Hadoop 集群的所有机器上。

**3。设计**

HDFS 的设计便于使用 MapReduce 范式。这里，计算转移到数据上。NAS 与 MapReduce 范式不兼容，因为这里的数据是与计算实际发生的地方分开存储的。

**4。成本**

由于 HDFS 使用商用硬件，与 NAS 所需的昂贵的专用高端存储设备相比，使用 HDFS 是一种经济高效的解决方案。

#### **问题:****Hadoop 1 和 2 的主要区别是什么？**

**回答** : Hadoop 最初发布于 2006 年 4 月。第一个成熟的 Hadoop 版本，Hadoop 1.0.0 于 2011 年 12 月发布，Hadoop 2.0.0 于 2013 年 10 月发布。Hadoop 2 添加了 YARN 作为 Hadoop 1 中 MapReduce 引擎(MRv1)的替代。

中央资源管理器 YARN 支持在 Hadoop 中运行多个应用，同时所有应用共享一个公共资源。Hadoop 2 使用 Mr v2——一种独特的分布式应用程序——在 YARN 之上执行 MapReduce 框架。

#### **问题:** **请比较一下 Hadoop 2 和 3？**

**答案** : Hadoop 3 发布于 2017 年 12 月 13 日。以下是 Hadoop 2.x.x 和 Hadoop 3.x.x 版本之间的重要区别:

**1。故障点**

在 Hadoop 2 中，NameNode 是单点故障。这给实现高可用性带来了很大的问题。Hadoop 3 通过引入主动和被动命名节点解决了这个问题。当主动 NameNode 出现故障时，被动 NameNode 之一可以接管控制权。

**2。应用开发**

Hadoop 3 中的容器工作原理是 Docker。它有助于减少应用程序开发所需的总时间。

**3。[擦除编码](https://en.wikipedia.org/wiki/Erasure_code)**

Hadoop 3 中擦除编码的实施降低了存储开销。

**4。GPU 硬件使用情况**

在 Hadoop 2 中，无法在集群上执行 DL(深度学习)算法。这是 Hadoop 3 中的附加功能，可以在 Hadoop 集群中使用 GPU 硬件。

#### **问题:** **简单解释主动和被动 NameNodes。**

**回答**:主动 NameNode 工作运行在一个集群中。被动 NameNode 具有与主动 NameNode 相似的数据。仅当出现故障时，它才替换活动的 NameNode。因此，它的目的是实现高度的可用性。

#### **问题:** **为什么频繁地在 Hadoop 集群中添加或删除 DataNodes？**

**回答**:频繁添加(试运行)和/或移除(退役)数据节点有两个原因:

1.  利用商用硬件
2.  扩展，即适应数据量的快速增长

#### **问题:** **如果两个用户试图在 HDFS 访问同一个文件会发生什么？**

**回答**:NameNode 收到打开文件的请求后，将租约授予第一个用户。当另一个用户尝试这样做时，NameNode 会注意到租约已经被授予，然后会拒绝访问请求。

#### **问题:** **请解释 NameNode 如何管理 DataNode 故障？**

**回答**:NameNode 从 Hadoop 集群中的每个 DataNodes 接收到一个周期性的心跳消息，暗示其正常运行。当 DataNode 未能发送心跳消息时，NameNode 会在一段时间后将其标记为 dead。

#### **问题:** **你对检查点有什么理解？**

**回答**:由二级 NameNode 执行，检查点减少 NameNode 启动时间。本质上，这个过程包括将 FsImage 与编辑日志结合起来，并将两者压缩成一个新的 FsImage。

检查点允许 NameNode 直接从 FsImage 加载最终的内存状态。

#### **问题:** **请解释一下 HDFS 是如何实现容错的？**

**答**:为了实现容错，HDFS 有一种叫做复制因子的东西。它是 NameNode 将一个 DataNode 的数据复制到其他一些 DataNode 的次数。

默认情况下，复制因子为 3，即 NameNode 存储单个 DataNode 上存储的数据的 3 个额外副本。在 DataNode 失败的情况下，NameNode 从这些副本之一复制数据，从而使数据随时可用。

#### **问题:****Apache Hadoop 与 Apache Spark 有何不同？**

**回答**:有几种强大的集群计算框架可以应对大数据挑战。当优先考虑高效处理批处理时，Apache Hadoop 是分析大数据的合适解决方案。

然而，当优先级是有效地处理实时数据时，我们就有了 Apache Spark。与 Hadoop 不同，Spark 是一个能够交互处理数据的低延迟计算框架。

虽然 Apache Hadoop 和 Apache Spark 都是流行的集群计算框架。然而，这并不意味着两者完全相同。实际上，两者都迎合了大数据的不同分析需求。以下是两者之间的各种差异:

*   **引擎类型** -虽然 Hadoop 只是一个基本的数据处理引擎，但 Spark 是一个专门的[数据分析](https://hackr.io/tutorials/learn-apache-spark?ref=blog-post)引擎。
*   **面向** - Hadoop 旨在处理海量数据的批处理。另一方面，Spark 的目的是处理实时事件(如社交媒体)产生的实时数据。
*   **延迟** -在计算中，延迟表示给出数据传输指令的时间和数据传输实际开始的时间之间的差异。Hadoop 是一个高延迟计算框架，而 Spark 是一个低延迟计算框架。
*   **数据处理** - Spark 交互处理数据，Hadoop 不能。在 Hadoop 中，数据以批处理模式处理。
*   **复杂性/易用性** - Spark 由于采用了抽象模型而更易于使用。用户可以很容易地用高水平的操作员处理数据。Hadoop 的 MapReduce 模型很复杂。
*   **作业调度器** **需求** - Spark 特性内存计算。与 Hadoop 不同，Spark 不需要外部作业调度程序。
*   **安全级别**——Hadoop 和 Spark 都是安全的。但是，虽然 Spark 只是受到保护，但 Hadoop 却受到了严密保护。
*   **成本** -由于 MapReduce 模型提供了一种更便宜的策略，Hadoop 与 Spark 相比成本更低，而 Spark 由于拥有内存计算解决方案而成本更高。

更多关于这个的？查看这个深入的 [Hadoop 与 Spark](https://hackr.io/blog/hadoop-vs-spark) 对比。

#### **问题:** **大数据的五个 V 是什么？**

**回答**:大数据的五个 V 是价值、多样性、速度、准确性、体量。每一种解释如下:

*   价值——除非处理大数据能够产生改善业务流程或收入的结果，否则它毫无用处。价值是指大数据带来的生产力。
*   多样性——指数据类型的异构性。大数据有多种格式，如音频文件、CSV 和视频。这些格式代表了大数据的多样性。
*   速度——指大数据增长的速度。
*   准确性——指由于数据的不一致和不完整，数据的可用性受到怀疑或不确定。
*   卷—指大数据量，通常以 EB 和 Pb 为单位。

#### **问题:****NameNode 和 DataNodes 的理想存储是什么？**

**回答**:处理大数据需要大量存储空间来存储海量数据。因此，商用硬件，如 PC 和笔记本电脑，是 DataNodes 的理想选择。

由于 NameNode 是存储 Hadoop 集群中所有数据块的元数据的主节点，因此它需要较高的内存空间，即 RAM。所以，对于 NameNode 来说，一台具有良好 RAM 的高端机器是理想的。

#### **问题:** **请解释一下 NameNode 的恢复过程？**

**答**:NameNode 恢复过程包括以下两个步骤:

*   步骤 1 -使用文件系统元数据副本(即 FsImage)启动新的 NameNode。
*   步骤 2 -配置 DataNodes 和客户机，使它们能够识别新的 NameNode。

一旦新的 NameNode 完成加载最后一个检查点 FsImage 并从 DataNodes 收到足够的块报告，它将开始为客户端提供服务。

#### **问题:** **为什么我们不应该使用 HDFS 来存储大量小文件？**

**回答** : HDFS 更适合在单个文件中存储海量数据，而不是在多个文件中存储少量数据。

如果您使用 HDFS 存储大量小文件，那么这些文件的元数据与所有这些文件中的完整数据相比将非常重要。因此，这将不必要地需要更多的内存，使整个过程效率低下。

#### **问题:****Hadoop 1、2、3 中默认的块大小是多少？怎么才能改变呢？**

**回答**:Hadoop 1 中默认的块大小是 64MB，Hadoop 2 和 Hadoop 3 中同样是 128MB。为了根据要求设置块的大小，使用 hdfs-site.xml 文件中的 dfs.block.size 参数。

#### **问题:** **我们如何检查 Hadoop 守护进程是否正在运行？**

**回答**:为了检查 Hadoop 守护进程是否在运行，我们使用 jps (Java 虚拟机进程状态工具)命令。它显示了所有正在运行的 Hadoop 守护进程的列表。

#### **问题:****Hadoop 中什么是机架感知？**

**答**:NameNode 作出决定的算法，一般来说，决定如何放置块和副本，具体来说，称为机架感知。NameNode 根据机架定义做出决定，目的是最小化同一机架中的数据节点之间的网络流量。

Hadoop 集群的默认复制因子是 3。这意味着对于每个数据块，将有三个拷贝可用。两个副本将存在于一个机架中，另一个存在于另一个机架中。它被称为副本放置策略。

#### **问题:** **请解释一下 Hadoop 中的推测执行？**

**答**:当发现一个节点执行任务的速度较慢时，主节点会在其他节点上执行同一任务的另一个实例。在这两个任务中，第一个完成的任务被接受，而另一个被杀死。这在 Hadoop 中称为推测执行。

#### **问题:** **请解释一下 HDFS 块和输入拆分的区别？**

**回答**:HDFS 数据块是 Hadoop 集群中存储数据的物理分区。相反，输入拆分是相同的逻辑划分。

HDFS 将存储的数据划分为块以便以高效的方式存储，而 MapReduce 将数据划分为输入拆分，并将其分配给 mapper 函数以供进一步处理。

#### **问题:****Apache Hadoop 运行的各种模式有哪些？**

**回答** : Apache Hadoop 运行在三种模式下:

1.  **独立/本地模式-** 这是 Hadoop 中的默认模式。在这种模式下，所有 Hadoop 组件都作为一个 Java 进程运行，并使用本地文件系统。
2.  **伪分布式模式-** 单节点 Hadoop 部署在伪分布式模式下运行。在这种模式下，所有 Hadoop 服务都在单个计算节点上执行。
3.  **完全分布式模式-** 在完全分布式模式下，Hadoop 主服务和从服务分别在不同的节点上运行。

#### **问题:** **你将如何重启 NameNode 或者所有的 Hadoop 守护进程？**

**回答**:重启 NameNode:

*   步骤 1 -首先，输入/sbin/Hadoop-daemon . sh stop namenode 命令来停止 NameNode。
*   步骤 2 -现在，输入/sbin/Hadoop-daemon . sh start namenode 命令来启动 NameNode。

要重新启动所有 Hadoop 守护进程:

*   步骤 1 -要停止所有 Hadoop 守护进程，请使用/sbin/stop-all.sh 命令。
*   步骤 2 -要再次启动所有 Hadoop 守护进程，请使用/sbin/start-all.sh 命令。

#### **问题:** **定义 MapReduce。运行 MapReduce 程序的语法是什么？**

**答** : MapReduce 是一种编程模型，也是一种关联实现，用于在 Hadoop 集群上用并行分布式算法生成大数据集。MapReduce 程序包括:

1.  **映射过程-** 执行过滤和[排序](https://medium.com/hackr-io/what-are-different-types-of-sorting-used-in-c-programming-compsmag-aa5a36ca0fde)
2.  **归约方法-** 执行汇总操作

运行 MapReduce 程序的语法是:

```
hadoop_jar_file.jar/input_path/output_path
```

#### **问题:** **列举一个 MapReduce 程序中需要指定的各种配置参数？**

**答**:以下是用户在 MapReduce 程序中需要指定的各种配置参数:

*   数据的输入格式
*   分布式文件系统中作业的输入位置
*   分布式文件系统中作业的输出位置
*   数据的输出格式
*   包含地图函数的类
*   包含 reduce 函数的类
*   包含映射器、缩减器和驱动程序类的 JAR 文件

#### **问题:** **为什么不能在映射器中执行聚合？为什么我们同样需要减速器？**

**答**:以下是无法在 mapper 中执行聚合的各种原因:

*   聚合需要所有映射器函数的输出，这可能无法在映射阶段收集，因为映射器可能运行在不同于包含数据块的机器上。
*   没有排序就无法进行聚合，而且聚合也不会发生在 mapper 函数中。
*   尝试在映射器上聚合数据，然后需要在所有映射器功能之间进行通信。由于不同的映射器功能可能在不同的机器上运行，因此需要高网络带宽，这可能会导致[网络瓶颈](https://en.wikipedia.org/wiki/Bottleneck_(network))。

分类只发生在 reducer 端，我们需要 reducer 函数来完成聚合。

#### **问题:** **为什么我们在 Hadoop 中需要 RecordReader？在哪里定义的？**

**答**:输入拆分是任务的一部分，对其访问方式没有任何描述。RecordReader 类负责从数据源加载数据，并将其转换为适合 Mapper 任务读取的 K，V(键，值)对。输入格式定义了 RecordReader 的一个实例。

问:请解释一下 MapReduce 框架中的分布式缓存？

**答**:分布式缓存是 MapReduce 框架提供的一个实用工具，用于缓存应用程序所需的文件。一旦用户缓存了某个作业的文件，Hadoop 框架就会在运行 map/reduce 任务的所有数据节点上提供该文件。缓存文件可以作为映射器或缩减器作业中的本地文件进行访问。

#### **问题:****MapReduce 编程模型允许 reducers 相互通信吗？**

**回答**:reducer 在 MapReduce 框架中是孤立运行的。没有办法建立彼此之间的通信。

#### **问题:** **请解释一下 MapReduce 的划分器？**

**答**:MapReduce 分割器有助于将地图输出均匀地分布在各个减速器上。这是通过确保一个键的所有值都进入同一个 reducer 来实现的。

MapReduce 分区器通过确定哪个缩减器负责特定的键，将映射器输出重定向到缩减器。

#### **问题:** **能否解释一下用 Apache Hadoop 编写自定义分区器的步骤？**

**回答**:下面是在 Hadoop 中编写自定义分区器的一步一步的过程:

*   步骤 1 -创建一个新类来扩展 Partitioner 类
*   步骤 2 -接下来，在 MapReduce 中运行的包装类中覆盖 getPartition 方法
*   步骤 3 -现在，您可以将自定义分区器作为配置文件添加到作业中，或者使用 Set Partitioner 方法。

#### **问题:** **你对 Hadoop 中的合并器有什么理解？**

**答**:合并器通过减少发送给 reducers 的数据来提高 MapReduce 框架的效率。组合器是一个小型的归约器，负责执行局部归约任务。

组合器从特定节点上的映射器接收输入，并将输出发送给缩减器。

#### **问题:** **能否解释一下 SequenceFileInputFormat？**

**答**:序列文件是数据从一个 MapReduce 作业传递到另一个作业的有效中间表示。它们可以作为其他 MapReduce 任务的输出生成。

SequenceFileInputFormat 是一种压缩的二进制文件格式，针对在一个 MapReduce 作业的输出和其他 MapReduce 作业的输入之间传递数据进行了优化。这是一种用于在序列文件中读取的输入格式。

#### **问题:** **列举一些 Apache Hadoop 最值得注意的应用？**

**回答** : Apache Hadoop 是一个开源平台，用于实现大量数据的可扩展和分布式计算。它为分析结构化、半结构化和非结构化数据提供了一种快速、高效且经济高效的方法。以下是 Apache Hadoop 的一些最佳使用案例:

*   实时分析客户数据
*   存档电子邮件
*   捕获和分析点击流、社交媒体、交易和视频数据
*   内容管理
*   欺诈检测和防范
*   交通管理
*   让非结构化数据变得有意义
*   管理社交媒体平台上的内容和媒体
*   科学研究
*   流式处理

#### **问题:** **使用分布式缓存有什么好处？**

**回答**:使用分布式缓存有以下好处:

1.  它可以分发任何内容，从简单的只读文本文件到复杂的文件，如档案。
2.  它跟踪缓存文件的修改时间戳。

#### **问题:** **什么是备份节点和检查点命名节点？**

**回答**:检查点 NameNode 每隔一段时间为命名空间创建检查点。它通过下载 FsImage、编辑文件并将其合并到本地目录中来实现。合并后，新的 FsImage 被上传到 NameNode。它具有与 NameNode 相同的目录结构。

备份节点在功能上类似于检查点命名节点。尽管它维护文件系统名称空间的最新内存副本，但它不需要定期记录变化。简而言之，备份节点将内存中的当前状态保存到映像文件中，以便创建新的检查点。

#### **问题:****Apache Hadoop 中常见的输入格式有哪些？**

**回答** : Apache Hadoop 有三种常见的输入格式:

1.  **键值输入格式** -适用于纯文本文件，其中文件被分成若干行
2.  **顺序文件输入格式** -用于顺序读取文件
3.  **文本输入格式**——这是 Hadoop 中的默认输入格式

#### **问题:** **解释一下减速器的核心方法？**

**答**:减速器有三种核心方法，解释如下:

1.  **cleanup()** -仅在任务结束时使用一次，用于清理临时文件。
2.  **reduce()** -对于相关的简化任务，每个键总是调用一次。
3.  **setup()** -用于配置各种参数，如分布式缓存、输入数据大小等。

#### **问题:** **请解释一下 JobTracker 在 Hadoop 中的作用？**

**答**:Hadoop 集群中的一个 JobTracker 负责:

*   资源管理，即管理任务跟踪器
*   任务生命周期管理，即跟踪任务进度和任务容错能力
*   跟踪资源可用性

#### **问题:** **映射端连接和缩减端连接有什么不同？**

**回答**:地图端连接需要严格的结构。当数据到达地图且输入数据集必须结构化时，执行此操作。Reduce-side 连接更简单，因为不要求对输入数据集进行结构化。Reduce 端连接比 Map 端连接效率低，因为它需要经过排序和洗牌阶段。

#### **问题:** **你知道如何调试 Hadoop 代码吗？**

**回答**:从检查当前正在运行的 MapReduce 作业列表开始。此后，检查是否有一个或多个孤立作业正在运行。如果有，则需要确定 RM 日志的位置。这可以通过以下方式完成:

*   步骤 1 -使用 ps -ef | grep -I ResourceManager 命令在结果中查找日志目录。找出作业 ID，并检查孤立作业是否有错误消息。
*   步骤 2 -使用 RM 日志来识别与孤立作业相关的任务执行中涉及的工作节点。
*   步骤 3 -登录到受影响的节点并运行以下代码:

```
ps -ef | grep -iNodeManager
```

*   步骤 4 -检查节点管理器日志。大多数错误来自每个 MapReduce 作业的用户级日志。

## 结论

这总结了我们的顶级 Hadoop 面试问题列表。希望这些对你准备即将到来的面试或检查你学习 Hadoop 的进度有所帮助。另外，不要忘记查看这些最好的 Hadoop 教程来[学习 Hadoop](https://hackr.io/tutorials/learn-hadoop-big-data?ref=blog-post) 。

准备 Apache Spark 面试？看看这些[重要的星火面试问题](https://hackr.io/blog/apache-spark-interview-questions)。

**人也在读:****