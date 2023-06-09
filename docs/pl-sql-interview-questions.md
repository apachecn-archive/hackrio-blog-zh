# 2023 年 50 大 PL/SQL 面试问答[更新]

> 原文：<https://hackr.io/blog/pl-sql-interview-questions>

您是否正在准备 PL/SQL 面试，如果是，我们将在此列出一系列 PL/SQL 面试问题。

PL(过程语言)是 SQL(结构化查询语言)的扩展，开发人员可以使用过程、分支和迭代等控制结构、模块和函数编写复杂的数据库交互。它与 SQL 紧密集成，支持动态和静态 SQL。

在面试的其他问题中，了解 SQL 和 PL/SQL 的不同也很重要。与 SQL 相比，PL/SQL 的一些优势包括:

*   支持过程化处理、条件语句、循环和其他类似于高级语言的特性。
*   多个语句可以以过程的形式一次发送到数据库服务器，从而节省时间和网络流量。
*   定制的错误处理是可能的。
*   完全便携。

除了上述优点，PL/SQL 还有一些更吸引人的特性，如函数、过程、触发器、游标，这使它成为最通用的关系数据库之一。

## **简介**

PL/SQL 1.0 于 1992 年发布，Oracle 6 作为可选扩展。正是在 PL/SQL 2.0 中，引入了 [**存储过程**](https://hackr.io/blog/stored-procedures) 、函数、用户定义的记录类型、表、包以及 DBMS_*之类的扩展。最新的 PL/SQL 版本是 11.0，它随 Oracle 11g 一起发布，并附带了一些高级功能，如本机编译、PL/SQL 函数结果高速缓存和分钟相关性跟踪。

## **最佳 PL/SQL 面试问题&答案**

以下是一些常见的基本和高级 pl/sql 面试问题和答案，面试官在面试中会问这些问题和答案

#### **问题:什么是 PL/SQL？**

**A** **nswer:** A [程序语言](https://hackr.io/blog/procedural-programming)代码可以分块执行。它是 SQL 的扩展。

#### **问题:PL/SQL 和 SQL 有什么区别？**

**答案:**

| **SQL** | **PL/SQL** |
| SQL 是一种与数据库交互的查询语言。 | 它是 SQL 的扩展，支持过程、函数和更多特性。 |
| 仅支持可以对表执行插入、更新和删除操作的简单查询。 | 可以像高级编程语言一样执行复杂的任务，例如 while 循环、if-else 语句等… |
| SQL 语句一次只能执行一条，因此这是一个非常耗时的过程。 | 整个语句块被一次发送到数据库服务器执行，节省了时间，提高了效率。 |
| 不提供错误处理。 | 定制的错误处理是可能的。 |

#### **问题:PL/SQL 的基本结构是什么？**

**答案:**

```
[DECLARE]
--declaration statements (optional)
BEGIN
--execution statements
[EXCEPTION]
--exception handling statements
END;

```

#### **问题:定义光标及其用途。**

**答案:**游标是一个指针，指向 Oracle 为处理 SQL 语句而分配的内存区域。游标用于保存 SQL 查询返回的记录。有两种类型的游标-隐式和显式。

#### 问题:为什么我们要使用数据库触发器？给出触发器的语法。

**答:**触发器是一个存储过程，在事件发生时自动调用。事件可以是:插入、更新、删除等……语法–

```
create trigger [trigger_name]
[before | after]

on [table_name]
[for each row]
[trigger_body]

```

#### **问题:如何编译 PL/SQL 代码？**

**回答:**首先进行语法检查。当开发人员纠正任何语法错误时，Oracle 将所有保存数据的变量与存储地址绑定在一起。最后，执行 p 代码生成过程。

#### **问题:解释 PL/SQL 中的异常处理。**

**回答:** PL/SQL 提供定制的异常处理。当错误发生时，错误处理代码包含在程序本身中。有 3 种例外情况——

*   预定义异常–已经定义的常见错误。示例–未找到数据
*   未定义的异常–没有预定义名称的错误。
*   用户定义的异常–由用户编写的代码处理。

#### **问题:说说 PL/SQL 中的几种数据类型。**

**回答:**数据类型很多——

*   标量类型–原始数据类型，如 CHAR、DATE、LONG、VARCHAR2 等
*   复合数据–这些数据由其他数据类型组成，可以很容易地更新。示例、记录、表格等
*   引用数据类型，如游标
*   大型对象类型–BLOB、CLOB 等

#### **问题:%TYPE 和%ROWTYPE 有什么区别？举个例子。**

**答案:**

| **%类型** | **%行类型** |
| 声明与表列具有相同数据类型的变量的属性。 | 声明与表行具有相同结构的记录类型变量的属性。行是包含与表或视图的列具有相同数据类型和*名称*的字段的记录。 |
| 示例—

```
DECLARE studentId students.student_id%TYPE; 
```

 | 示例—

```
DECLARE stud_rec students.%ROWTYPE;
```

 |

#### 问题:PL/SQL 包是由什么组成的？

**答:**包是将函数、过程、变量等…放在一个地方的模式对象。包装应具有–

*   包装规格
*   包装体

#### **问题:列出一些使用 PL/SQL 创建的模式对象。**

**回答:**数据库链接、触发器、存储过程、函数和包、视图、同义词、外部过程库、序列等…

**查看这里:** [基本 SQL 命令清单](https://hackr.io/blog/sql-commands)

#### 问:各种预定义的异常是什么？

**答:**预定义异常是在程序执行过程中发生的内部定义的异常。例如，当 select 操作没有返回任何行时，PL/SQL 会引发 NO_DATA_FOUND，如果使用 select 语句返回了多行，则会生成 TOO_MANY_ROWS 错误。更多示例:

*   COLLECTION_IS_NULL:当集合为空时
*   CURSOR_ALREADY_OPEN:当游标已经打开时
*   LOGIN_DENIED:当登录不正确或没有权限时

有关预定义异常的完整列表，请查看 Oracle 文档。

#### **问题:语法错误和运行时错误有什么区别？**

**答案:**

| **语法错误** | **运行时错误** |
| 这些是编译器发现的编译时错误。 | 这些不会被编译器检测到，并导致程序给出不正确的结果。 |
| 在这些问题解决之前，代码不会构建和运行。 | 代码被编译并运行，如果出现错误，程序会中途停止。 |
| 一些例子是缺少分号或括号(；，{})，错误的类别拼写，关键字等。 | 例子有空指针异常、将一个数除以零、数组索引越界等。 |
| int x = 9 String name = null 在第一行中，缺少一个分号，编译器会捕捉到它 | 字符串名称= nullif(name . equals(" hackr . io "){…}因为 name 为空，所以在运行时执行代码时会捕获到异常 |

#### **问题:PL-SQL 开发人员可用的各种包有哪些？**

**回答:**可供 PL/SQL 开发人员使用的几个包是:

| DBMS_ALERT | 当特定数据库值发生变化时，使用触发器向应用程序发出警报。这些警报是基于事务的异步警报。 |
| 数据库管理系统 _ 输出 | 显示 PL/SQL 块、程序包、子程序和触发器的输出。主要用于显示 PL/SQL 调试信息。 |
| 数据库管理系统 _ 管道 | 不同的会话使用这个包通过命名管道进行通信。过程 PACK_MESSAGE 和 SEND_MESSAGE 将消息打包到管道中，然后将其发送到另一个会话。 |
| HTF 和 HTP | 允许 PL/SQL 程序生成 HTML 标记。 |
| UTL _ 文件 | 让 PL/SQL 程序读写操作系统文本文件。 |
| UTL_HTTP | 允许您的 PL/SQL 程序生成超文本传输协议(HTTP)标注。这个包有两个入口点，每个入口点接受一个 URL(统一资源定位符)字符串，联系指定的站点，并返回请求的数据，这些数据通常是 HTML 格式的。 |
| UTL_SMTP | 允许 PL/SQL 程序通过 SMTP 发送电子邮件。 |

来源:[甲骨文文件](https://docs.oracle.com/cd/B19306_01/appdev.102/b14261/packages.htm)

#### 问题:解释角色功能？

**答案:**字符函数是操纵字符数据的函数。这些函数通常被称为字符串函数。示例:

| 左边的 | 返回从字符串左侧开始的字符数。左(值，NoOfChars)。例子 | 左(' Hackr '，4)会给出 Hack。 |
| 正确 | 从右侧返回指定数量的字符。右(值，NoOfChars)。例子 | RIGHT('banker '，2)将返回 er。 |
| 子链 | 从字符串的任何部分选择数据。SUBSTRING(value，StartPosition，NoOfChars)。例子 | SUBSTRING('hackr.io '，0，4)将返回 hackr。 |
| LTRIM(即时通讯) | 从左侧修剪空白。例子 | LTRIM(' hackr.io ')将返回 hackr.io。 |
| RTRIM | 从右侧修剪空白。例子 | RTRIM('hackr.io ')将返回 hackr.io。 |
| 上面的 | 将所有字符转换为大写。例子 | UPPER('hackr.io ')返回 hackr.io。 |
| 降低 | 将所有字符转换成小写。例子 | 降低(' HACKR。IO’)返回 hackr.io。 |

#### **问题:SYSDATE 和用户关键字有什么用？举例说明。**

**答案:SYSDATE:** 返回本地数据库服务器上的当前日期和时间。语法是 SYSDATE。如果我们必须提取部分日期，那么我们使用 TO_CHAR 函数。示例:

```
SELECT SYSDATE FROM dual;
select customer_id, TO_CHAR(SYSDATE, 'yyyy/mm/dd') from customer where customer_id < 200;
```

**USER:** USER 返回当前会话的 user_id。

示例:

```
select USER from dual;
```

#### 问:SGA 和 PGA 有什么区别？

**回答:**

| **SGA** | **PGA** |
| 系统全局区域 | 程序全局区域 |
| 包含一个 Oracle 数据库实例的数据和控制信息 | 包含专用于单个 Oracle 进程的数据和控制信息 |
| 组件的共享内存区域 | 非共享存储区 |
| 示例:缓存的数据块和 SQL 区域 | 示例:会话内存、SQL 工作区 |

#### 问:解释在 PL-SQL 中 Merge with 语法的用法。

**答:** Merge 减少了表扫描的次数，如果需要的话还会执行并行操作。MERGE 有条件地将数据从一个表插入或更新到另一个表。举个例子，

```
MERGE INTO orders o
 USING customer c
 ON (o.cust_id = c.cust_id)
 WHEN MATCHED THEN
 UPDATE SET o.del_address = c.address
 WHEN NOT MATCHED THEN
 INSERT (cust_id, address)
VALUES (c.emp_id, c.address);
```

在这个例子中，如果找到了具有匹配条件的记录，则更新相同记录的地址，否则插入新的行。

#### **问题:解释 PL-SQL 包的好处。**

**回答:**使用 PL/SQL 包有很多好处:

*   更好的代码管理，因为包为子程序提供了一个容器
*   实现和规范分离的自顶向下的应用程序设计方法(接口)
*   如果子程序有任何改变，不需要改变依赖对象或重新编译整个包
*   可以指定可访问性(私有/公共)，从而维护代码的安全性
*   数据可以跨整个会话的事务进行维护，而无需存储在数据库中
*   在子程序的第一次调用中，加载整个包，因此后续调用不需要磁盘 I/O，从而提供更好的性能。

#### **问题:解释 ROLLBACK 和 ROLLBACK TO 语句的区别？**

**回答:** ROLLBACK 命令从事务开始处回滚所有的更改。在 ROLLBACK TO 中，事务仅回滚(或撤消)到一个称为保存点的点。保存点之前的事务不能撤消，即使给出了命令，事务仍保持活动状态。

#### **问题:解释过程和函数的区别。**

**答案:**

| **功能** | **程序** |
| The function is compiled every time它被要求执行。 | 程序是预先编译和保存的。只要被调用，它们就会执行预编译的代码。 |
| 可以从 SQL 语句中调用。 | 不能从 SQL 语句中调用。 |
| 该函数必须返回值。 | 不需要返回任何值。 |
| 通常用于计算目的。 | 用于执行复杂的业务逻辑。 |
| 可以使用其他方法返回多个值，否则，只返回一个值。 | 可以返回多个值 |
| 返回标量数据类型。 | 默认情况下返回一个整数。 |
| 不能从函数中调用存储过程 | 该程序可以调用任何函数 |
| 函数可以嵌入到 select 语句中 | 在 select 语句中，不能调用过程。 |
| 异常处理是不可能的 | Try/catch 块可以在过程内部定义 |

#### **问题:解释过程和触发器的区别。**

**答案:**

| **程序** | **触发** |
| 由用户、触发器或应用程序显式调用 | 每当数据库中发生事件时，由 DBMS 执行。 |
| 可以有参数 | 没有参数 |
| 不能处于非活动状态 | 可以根据需要启用或禁用 |
| 创建–创建程序 | 创建–创建触发器 |

#### **问题:PL/SQL 中有哪些不同类型的游标？**

**回答:**光标有两种类型——

*   隐式游标–PL/SQL 对返回单行的 INSERT、UPDATE、DELETE 和 SELECT 语句应用隐式游标。
*   显式游标–由程序员为返回多行的查询创建。语法–

```
CURSOR is
SELECT statement;
OPEN ;
FETCH INTO ;
CLOSE ;

```

#### 问:有哪些不同类型的约束？

**答案:**

*   不为空
*   独一无二的
*   主关键字
*   外键
*   支票

#### **问题:触发器和约束有什么区别？**

**答案:**

| **触发器** | **约束条件** |
| 作为单独的对象存储 | 表的约束与表定义一起存储 |
| 事件发生时触发触发器；因此，它们在约束后被触发 | Constraints are fired as soon as the这张桌子已经用过了。 |
| Perform table to table比较，因此更快 | 执行内存定位来比较表，这是缓慢的，导致低性能。 |
| 触发器适用于整个表 | 该约束针对表中的一列 |
| 它们只是自动执行的存储过程，因此不检查数据完整性。 | 防止重复和无效的数据条目 |

#### **问题:举例说明 PL/SQL 块。**

**答案:** PL/SQL 块由三个部分组成:声明、可执行和异常处理部分。可执行部分是必需的。有两种类型的块:命名的和匿名的。

命名块是存储在数据库服务器中并可以重用的函数和过程。匿名块仅供一次性使用，不存储在服务器中。示例:

```
DECLARE

 message VARCHAR2(255):= 'Welcome to PL/SQL';
 byzero NUMBER;

BEGIN

   DBMS_OUTPUT.put_line (message);
   byzero := 1/0;

   EXCEPTION

  WHEN ZERO_DIVIDE THEN
 DBMS_OUTPUT.PUT_LINE(SQLERRM);
END;
```

#### **问题:解释 PL/SQL 记录。**

**答案:**记录包含一组各种数据类型的数据，这些数据可以作为字段相互关联。PL/SQL 中支持的三种记录类型是基于表的记录、基于程序员的记录和基于游标的记录。

#### 问题:解释提交和保存点的区别。

**答案:**

提交–用于使数据库更改永久化。所有保存点被删除，交易结束。一旦提交，事务就不能回滚。

保存点–用于在事务期间设置点，程序员可以在以后回滚到该点。当有一系列事务可以分成具有保存点的组时，这是很有帮助的。

#### **问题:实参和形参有什么区别？**

**答:**用来调用一个过程的参数称为实参。示例–

```
get_student_details(stud_name, dob); -- here stud_name and dob are actual parameters.

```

在主体中使用的过程头中声明的变量称为形参。示例–

```
PROCEDURE get_student_details (dob DATE) IS – here stud_name is a formal parameter.

```

#### 问:如何使用 DECLARE 语句？

**答:** DECLARE 用作独立文件的第一条语句，这些文件由非存储过程、函数或触发器的匿名代码块组成。示例–

```
DECLARE
num1 NUMBER(2);
num2 NUMBER(3);
BEGIN
-- logic goes here
END;

```

#### **问题:给我们讲讲 SQLCODE 和 SQLERRM。**

**答案:** SQLCODE 和 SQLERRM 用于跟踪程序中没有显式处理的异常。这些是全局定义的变量。SQLCODE 返回错误代码，而 SQLERRM 返回相应的错误消息。

#### **问题:什么是回滚？与 rollback to statement 有何不同？**

**答:**回滚会擦除所有数据库更改，包括所有保存点。它结束一个交易。

“回滚到”将更改回滚到代码中提到的保存点。该事务仍将是活动的。

#### **问题:什么是 IN OUT 参数？**

**答:**在 OUT 参数模式下传递一个值给子程序，返回一个更新后的值。

#### 问题:在运行时可以接受用户输入吗？怎么会？

**回答:**是的，有可能。使用 ACCEPT 关键字接受用户的输入。示例–

接受年龄号码提示“输入您的年龄:”

#### **问题:给出一个更快运行查询的简单方法。**

**答案:**通过使用 ROWID。它不是物理列，而是行的逻辑地址。它包含块号、文件号和行号，从而减少 I/O 时间，使查询执行更快。

#### 问题:PL/SQL 中有哪些预定义的异常？

**答案:**零除、无数据发现、太多行、无效游标、DUP 有效索引等

#### 问:你如何追踪 PL/SQL 代码？

**回答:**您可以通过 DBMS_*方法进行跟踪，例如

*   数据库管理系统应用信息
*   DBMS_TRACE
*   数据库管理系统会话和数据库管理系统监视器

#### **问题:如何在 PL/SQL 中限制字符串长度？**

**答:**用 CHAR (NUMBER)获取一个变量的固定长度。示例–CHAR(10)。如果字符串的长度小于指定的数字，它将用空格填充。

#### **问题:PL/SQL 中 UTL _ 文件包的用途是什么？**

**回答:**通过使用这个包，开发者可以获得从计算机读写文件的代码。为此，开发人员需要 DBA 用户的访问授权。

#### **问题:DBMS_OUTPUT 和 DBMS_DEBUG 是什么？**

**回答:**两者都可以用来调试代码。DBMS_OUTPUT 将输出打印到控制台，而 DBMS_DEBUG 将输出打印到日志文件。

#### **问题:列出 PL/SQL 中的一些游标属性。**

**答案:**

*   %ISOPEN:检查光标是否打开
*   %ROWCOUNT:获取更新、删除或提取的行数。
*   %FOUND:检查游标是否提取了任何行，返回 Boolean。
*   %NOT FOUND:检查游标是否提取了任何行。返回布尔值。

#### 问:NVL 的目的是什么？

**回答:** NVL 让程序员用一个值代替一个空值。示例–

```
NVL (occupation, ‘default’)

```

#### **问题:在一个表上，可以应用多少个触发器？**

**回答:** 12 是最大数。

#### 问题:如何使用 PL/SQL 实现一致性？

**回答:**我们可以通过设置合适的隔离级别来达到一致性。例如，为了提供读一致性，可以将隔离级别设置为 READ COMMITTED。

#### **问题:** **写一个简单的程序，用一些参数从数据库中选择一些记录。**

**回答:**示例代码——

```
CREATE PROCEDURE get_customer_details @age nvarchar(30), @city nvarchar(10)
AS

BEGIN
SELECT * FROM customers WHERE age = @age AND city = @city;
END;

```

#### **问题:解释错误 ORA-03113。**

**回答:**通信通道 ORA-03113 上的错误文件尾表示客户端和服务器通道之间的连接断开。可能是超时导致连接丢失。您可以通过 ping 服务器并检查连通性来排除故障。

#### 问:你能在 SELECT 语句中使用 IF 语句吗？怎么会？

**回答:**是的，我们可以在版本 9 及以上版本中使用 DECODE 关键字来实现。示例–

```
SELECT day_of_week,
DECODE (number, 0, 'Sunday',
1, 'Monday',
2, 'Tuesday',
3, 'Wednesday',
4, 'Thursday',
5, 'Friday',
6, 'Saturday',
'No match') result FROM weekdays;
```

#### **问题:什么是 SYS。所有 _ 依赖关系？**

**答案:** SYS。ALL_DEPENDENCIES 描述当前用户可访问的包、过程、函数、触发器之间的所有依赖关系。它显示诸如名称、类型、依赖类型、引用所有者等列

## **结论**

在本文中，我们讨论了一些最重要的 pl/sql 面试问题，这些问题一定会让你通过最艰难的面试。如果您想深入学习这些概念并获得一些实践经验，请查看我们的 PL/SQL 教程。

这些面试问题将帮助您在 PL-SQL 面试中取得更好的成绩。在本课程中，我们还将介绍一些 PL/SQL 面试问题: [200+ PL/SQL 面试问题](https://click.linksynergy.com/deeplink?id=jU79Zysihs4&mid=39197&murl=https://www.udemy.com/course/plsql-interview-questions/)。

另外，这里有一本很棒的 [PL/SQL 面试问题](https://geni.us/ZoMyYgB)书，可以为即将到来的面试做准备。

如果你有一些其他的问题，我们没有在这个列表中，你想知道这些问题的答案，只需在下面评论。

**人也在读:**