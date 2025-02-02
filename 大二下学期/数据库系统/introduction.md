# 数据库系统原理与实践 —— 课程信息与学习建议

> **主教材**  
> 党德鹏主编《数据库系统原理与实践》

---

## 一、课程评分标准

- **平时成绩与期末成绩比例**：4.5 : 5.5  
  - **平时成绩** 主要依据：
    - **平时作业**：包括课堂作业和上机作业  
      - 注意：课堂作业偶尔出错会对平时成绩产生一定影响  
      - 上机作业要求认真完成，**报告格式尤为重要**：每次上机报告必须包含详细截图、心得说明，SQL 语句需要单独以代码块形式插入到文档中。
    - **线上 MOOC**：线上试题（答案可在网上找到）出错同样会影响成绩。
- **期末考试**  
  - 由以下两部分组成：
    - **选择题**：30 道题，每题 1 分，共 30 分；
    - **综合题**：共 70 分。
  - 考题难度总体不高，但题量较大。从去年的情况来看，第八章“查询与性能优化”部分出现过一道较难题目（涉及内存块分配，需深入理解），得分不理想。  
  - **注意**：复习时需重点关注关系代数运算、触发器代码及 MOOC 网课内容。

---

## 二、授课目录（课程内容概要）

1. **绪论** (3+0 学时)  
   - 主要内容：综述数据库系统的性质和目标；介绍数据库系统的发展历程；讲解三层模式、两级映射、数据逻辑独立性与数据物理独立性。  
   - 教学要求：通过实例说明数据库的优势及标准三级模式思想。

2. **关系数据库** (6+4 学时)  
   - 主要内容：关系模型基本概念（关系结构、数据库模式、码）；关系操作（关系代数、关系演算）；实际操作：通过 ACCESS 中的 QBE 示例、PostgreSQL 入门操作（图形化建库、备份与还原）。
   - 教学要求：通过数据模型的发展，帮助学生理解数据抽象、关系查询与更新的集合性质和代数表达式。

3. **SQL 数据定义与操作** (6+6 学时)  
   - 主要内容：SQL 的基本语法、数据定义、单表及多表查询、嵌套、聚集和集合查询；SQL 数据的插入、删除与修改。  
   - 教学要求：不仅讲解 SQL 语句的语法和语义，还强调其书写形式对执行性能的影响。

4. **SQL 数据安全** (3+6 学时)  
   - 主要内容：数据保护、视图的创建与更新、访问控制、约束、触发器以及事务。  
   - 教学要求：通过例子说明触发器中触发事件、条件和触发体动作的关系，讨论访问控制和视图更新的限制。

5. **应用环境中的 SQL** (3+4 学时)  
   - 主要内容：数据库应用系统体系结构；SQL 混合编程；JDBC/ODBC 及存储函数的使用。  
   - 教学要求：着重讲述 SQL 与编程语言混合使用时的技术问题（如语句区分、数据交换、阻抗不匹配等）。

6. **数据库设计与概念模型** (3+2 学时)  
   - 主要内容：数据库设计过程概要；采用实体关系（ER）模型进行数据库设计；从概念模型转换到逻辑关系模式的方法。  
   - 教学要求：强调概念模式的语义和逻辑模式实现时的具体差异，通过案例解析捕获应用中的语义信息。

7. **关系数据库设计** (6+0 学时)  
   - 主要内容：函数依赖、属性闭包、范式（3NF、BCNF）、无损连接与依赖保持；讨论各种范式提出的动机及其对应用性能的影响。  
   - 教学要求：通过大量实例讲解抽象概念，帮助学生掌握关系模式选择与设计的原则。

8. **数据存储与组织** (3+2 学时)  
   - 主要内容：数据库存储与检索的内部机制，包括存储设备、文件结构、索引和散列等；通过磁盘块组织介绍索引的原理（如聚集索引、B+树索引）。
   - 教学要求：重视记录在磁盘中的组织方式，讲解不同索引类型的特点。

9. **查询处理与优化** (6+2 学时)  
   - 主要内容：查询优化总体思路；关系代数等价变换；操作实现算法（如选择、连接）；并行化优化及基于代价估算的优化。  
   - 教学要求：通过实例讲解查询处理过程，比较不同执行策略的性能差异。

10. **事务处理** (6+2 学时)  
    - 主要内容：事务的 ACID 特性；调度与并发；锁机制与时间戳并发控制；备份、日志、恢复操作及检查点技术。  
    - 教学要求：利用正反例说明事务的重要性，讲解并发控制与故障恢复算法。

11. **大数据技术** (3+2 学时)  
    - 主要内容：大数据存储管理、大数据编程及典型应用案例；跟踪大数据管理趋势与新技术。  
    - 教学要求：结合实际案例，通俗易懂地讲解大数据管理的关键概念与容错性。

---

## 三、课程教学大纲

**课程名称**：数据库系统 (英文名称：Database Systems)  
**课程性质**：专业必修（专业核心课）  
**学分数**：3  
**适用专业**：计算机科学与技术  
**学时数**：每周 3 理论学时 + 2 实验学时  
**开设学期**：秋季、大三上学期  
**授课教师**：党德鹏 教授 (Email: ddepeng@bnu.edu.cn)  
**先修课程**：高级语言程序设计、数据结构、计算机组成原理等  

---

## 四、课程学习建议

- **上课与作业**  
  虽然老师讲解较为一般，但课上内容不能落下，因为课堂作业、上机作业和 MOOC 测验都将直接影响平时成绩。
  
- **复习与考试准备**  
  - 平时认真完成所有作业和实验，注意报告格式要求；  
  - 期末考试侧重选择题和综合题，建议重点复习第八章“查询与性能优化”部分、关系代数运算和触发器代码。
  - 2024 春季在讲完第1、2章后曾组织小测，难度不大，可作为复习参考。

- **参考材料**  
  - MOOC 选择题全套（期末前冲刺复习使用）；  
  - 往年数据库系统考试题（帮助熟悉题型，注意重复出现的情况较少）。

- **成绩录入**  
  成绩录入较快，请及时关注成绩更新。

---

# Database Systems: Principles and Practice – Course Overview & Study Tips

> **Primary Textbook**  
> *Database Systems: Principles and Practice* (Edited by Depeng Dang)

---

## Grading Policy

- **Coursework vs. Final Exam Ratio**: 4.5 : 5.5  
  - **Coursework** is based on:
    - In-class assignments (both classroom and lab assignments)  
      - Note: Occasional mistakes in classroom assignments can affect your coursework grade.
    - Online MOOC tests (answers are available online; errors will negatively impact your score).
  - **Final Exam**:
    - Comprises 30 multiple-choice questions (1 point each) and comprehensive questions worth 70 points.
    - Although the exam is not very difficult, the large volume of questions requires thorough review.
    - Special attention should be paid to the “Query and Performance Optimization” section (e.g., memory block allocation), relational algebra, and trigger code.

---

## Syllabus Overview

1. **Introduction** (3 theory hours)  
   - Overview of database system properties, objectives, and development.
   - Explanation of the three-schema architecture, two-level mapping, and data independence (logical vs. physical).

2. **Relational Databases** (6 theory + 4 lab hours)  
   - Fundamentals of the relational model: structure, schema, keys.
   - Relational operations: relational algebra and calculus.
   - Practical exercises using QBE in ACCESS and an introduction to PostgreSQL.

3. **SQL Data Definition and Manipulation** (6 theory + 6 lab hours)  
   - Basic SQL concepts, data definition, and various types of queries (single-table, multi-table, nested, aggregate, set queries).
   - Insertion, deletion, and update operations and their impact on performance.

4. **SQL Data Security** (3 theory + 6 lab hours)  
   - Concepts of data protection, views, access control, constraints, triggers, and transactions.
   - Emphasis on understanding trigger events, conditions, and actions.

5. **SQL in Application Environments** (3 theory + 4 lab hours)  
   - Database application architectures; mixed SQL programming; JDBC/ODBC and stored functions.
   - Discussion of technical issues in mixed-language programming such as statement differentiation and data exchange.

6. **Database Design and Conceptual Modeling** (3 theory + 2 lab hours)  
   - Overview of the database design process using the Entity-Relationship (ER) model and converting conceptual models to relational schemas.

7. **Relational Database Design** (6 theory hours)  
   - Functional dependencies, attribute closure, normalization (3NF, BCNF), lossless decomposition, and dependency preservation.
   - Use of examples to explain abstract concepts and design principles.

8. **Data Storage and Organization** (3 theory + 2 lab hours)  
   - Internal mechanisms for storage and retrieval, including storage devices, file structures, indexing, and hashing.
   - Focus on how data is organized on disk and different index types (e.g., clustered indexes, B+ trees).

9. **Query Processing and Optimization** (6 theory + 2 lab hours)  
   - Overall ideas of query optimization, equivalence transformations in relational algebra, algorithm analysis (selection, join, etc.), and cost estimation.
   - Comparative discussion of execution strategies.

10. **Transaction Processing** (6 theory + 2 lab hours)  
    - Transaction properties (ACID), scheduling and concurrency control, locking and timestamp methods, logging, recovery techniques, and checkpointing.
    - Real examples to illustrate the necessity of proper transaction management.

11. **Big Data Technologies** (3 theory + 2 lab hours)  
    - Big data storage management, programming, and case studies; discussion of emerging trends.
    - Emphasis on fault tolerance in big data systems.

---

## Course Details 

- **Course Name**: Database Systems  
- **Course Nature**: Core required course for Computer Science  
- **Credits**: 3  
- **Weekly Hours**: 3 theory + 2 lab  
- **Offered In**: Fall semester, 3rd year  
- **Instructor**: Prof. Depeng Dang (Email: ddepeng@bnu.edu.cn)  
- **Prerequisites**: Programming in a high-level language, Data Structures, Computer Organization, etc.


---

## Study Tips

- **Class Participation**: Although the lectures are average, do not miss class because assignments are based on in-class content.
- **Consistent Effort**: Pay attention to all assignments—classroom, lab, and MOOC—as they significantly impact your coursework score.
- **Exam Preparation**:  
  - Thoroughly review the “Query and Performance Optimization” section, relational algebra, and trigger code.
  - Use the mini-test (conducted after Chapters 1 and 2 in Spring 2024) as a reference for exam preparation.
- **Supplementary Materials**:  
  - MOOC multiple-choice questions set for last-minute review;  
  - Past exam papers for familiarizing yourself with question formats (note: few questions from Spring 2024 are likely to be repeated).

- **Grade Posting**: Grades are posted quickly; keep an eye on updates.

---
