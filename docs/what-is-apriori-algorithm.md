# 数据挖掘中的 Apriori 算法是什么？

> 原文：<https://hackr.io/blog/what-is-apriori-algorithm>

在这个全球化和其他电子商务零售店变得越来越出名的进步时代，各种企业使用机器学习和人工智能来保持竞争领先地位变得势在必行。因此，在当今的环境中，数据分析和计算机科学在应对动态竞争方面有着巨大的空间。计算机语言中的数据挖掘方法多种多样，主要有关联、相关和聚类等。

## 什么是 Apriori 算法？

Apriori 算法通常包含或处理大量事务。例如，顾客从杂货店购买大量商品，通过应用这种算法方法，杂货店可以提高他们的销售业绩并可以有效地工作。它在医疗保健领域检测药物不良反应也非常有效。要执行这种算法，人们应该了解关联规则，因为它是了解大型数据库和信息中变量之间的弱关系或强关系的最重要和最成熟的方法。Apriori 算法具有通过缩小搜索空间来提高效率的特性。

## **Apriori 算法中使用的基本术语**

在我们进一步了解 Apriori 算法之前，我们应该了解一下该算法中使用的基本术语，那就是:

**数据挖掘:**指从大型数据库中寻找信息的过程。

**频繁项集:**它是指包含具有最小支持度的项的所有集合，对于第 I 个项集通常用 Li 表示。

**先验性质:**使用频繁集和子集。

**Join 操作:**寻找候选的开头。

**频繁挖掘模式:**通过算法应用的常规数据挖掘

## **Apriori 算法在现实世界中的应用**

### **1。** **教育领域**

众所周知，在学校学习的所有学生都有不同的特点和个性，就像每个学生都有不同的年龄、性别、不同的名字和不同的父母名字等。

### **2。医疗领域**

在每个医院，都有很多病人入院，每个病人都有不同的疾病，根据不同的疾病给予不同的治疗，他们都有不同类型的特征和不同的病史，所以这里有必要使用 Apriori 算法的计算机科学方法来分析病人数据库。因此不应该混淆不同患者的信息

### **3。林业**

在每一片森林里，都有几种动植物。自然地，有各种各样的树，它们有不同的特征，像它们的大小、质地、树木的季节等等。同样，有各种类型的动物具有各种各样的特征，这使它们彼此不同。为了分析所有这些细节，我们使用了 Apriori 算法的方法。

### **4。新技术企业**

Apriori 被很多公司使用，像 Flipkart，Amazon 等等。其中他们必须维护各种产品的记录，这些产品是由各种客户为推荐系统购买的，也是由 google 为自动完成功能购买的。

### **5。办公室**

这种计算机科学技术的最有效的用途之一是在办公室中，在那里他们必须记录与各种商品和服务的销售和购买相关的大量日常交易，例如记录债权人的交易、销售和购买，因此需要对所有这种交易进行分析，以便不应该有任何种类的混乱。

### **6。移动电子商务**

使用这种技术的主要目的是使移动电子商务购物变得简单、方便，并增加跨越国家和国际边界的客户群。实时性和推荐准确性的统一部署，使移动电子商务获得 Apriori 算法的最大效益。

[关联规则挖掘:基础理论&实践](https://click.linksynergy.com/deeplink?id=jU79Zysihs4&mid=39197&murl=https%3A%2F%2Fwww.udemy.com%2Fcourse%2Fassociation-rule-mining-basic-theory-practice%2F)

## **经典和高级 Apriori 算法的区别**

1.  在经典的 Apriori 算法中，当产生候选项集时，算法需要测试它们的出现频率，这需要耗费大量的时间，而在改进的 Apriori 算法中，这需要很少的时间
2.  经典 Apriori 算法中的数据库规模很大，而 Apriori 算法的改进版本中的数据库规模很小
3.  早期 Apriori 算法中的数据库扫描在不同的数据库服务器上进行 N 次。但是在高级技术中，它是 n 倍。
4.  高级模式比经典的 Apriori 算法更有效，因为它使用更少的时间和空间浪费。
5.  Apriori 算法的高级模型比经典模型需要更多的内存
6.  做功的速度比经典的要快得多

## **关于挖掘关联规则的讨论**

下面借助两步方法解释挖掘关联规则:

### **步骤 1:频繁项目集生成**

按照过程 w 找出支持度大于阈值支持度的所有项目集

### **第二步:规则生成**

使用频繁项集的二进制划分为每个频繁项集创建规则，并查找可信度高的规则。

## **Apriori 算法的例子**

考虑以下杂货店的数据库:

**数据库项目**

| 项目集 |
| (1,2,3,4) |
| (1,2,4) |
| (1,2) |
| (2,3,4) |
| (2,3) |
| (3,4) |
| (2,4) |

这里我们将尝试出现至少三个值为 3 的事务，这将支持阈值。

通过第一次扫描数据库，我们获得了以下结果

| 项目 | 支持 |
| (1) | 3 |
| (2) | 6 |
| (3) | 四 |
| (4) | 5 |

所有大小为 1 的项目集都有至少 3 的支持，因此它们都是频繁的:

| 项目 | 支持 |
| (1,2) | 3 |
| (1,3) | 一 |
| (1,4) | 2 |
| (2,3) | 3 |
| (2,4) | 4 |
| (3,4) | 3 |

对(1，2)、(2，3)、(2，4)和(3，4)都满足或超过 3 的最小支持度，因此它们是频繁的。

对(1，3)和(1，4)不是。因为(1，3)和(1，4)不是频繁的，所以任何包含(1，3)或(1，4)的大集合都不可能是频繁的。

## **结论**

我们已经看到了如何推断各种数据，并提高超市和杂货店的销售业绩。这是 Apriori 算法实用性的一个例子。不仅在超市，这个概念也广泛应用于其他关键行业，如医疗保健行业等。它使该行业能够根据患者的特点，捆绑产生最少 ADRS 的药物。尽管这是一个耗时的过程，但在涉及大型数据库的情况下，它仍然使工作变得更容易。

在您工作的地方实施大数据项目时需要帮助吗？ [ProjectPro](https://click.linksynergy.com/fs-bin/click?id=jU79Zysihs4&offerid=1038112.3&type=3&subid=0) 将您与专家联系起来，帮助您完成这一过程。当然，你自己也可以这么做。DataCamp 提供[数据科学课程](https://datacamp.pxf.io/DVGE65)，为您的投资组合提供有用的项目，并为数据专业人员提供行业认可的[认证](https://datacamp.pxf.io/P0ELDj)。

**人也在读:**