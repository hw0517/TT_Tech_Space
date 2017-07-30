---
layout: post
category : datascience
tags : [bigdata,database,guide]
title: PostgreSQL Best Practice Note
---

PostgreSQL 应用案例 - 目录

作者

digoal


一、案例

1 任意维度实时圈人

1、《多字段，任意组合(0建模) - 毫秒级实时圈人》

2、《万亿级营销(圈人)迈入毫秒时代 - 实时推荐系统数据库设计》

3、用阿里云RDS varbitx支持万亿user_tags级实时圈人

《阿里云RDS for PostgreSQL varbitx插件与实时画像应用场景介绍》

《基于 阿里云RDS PostgreSQL 打造实时用户画像推荐系统》

2 时序数据实时处理

1、《时序数据合并场景加速分析和实现 - 复合索引，窗口分组查询加速，变态递归加速》

2、《PostgreSQL 证券行业数据库需求分析与应用》

3、ToB时序数据实时全文搜索实践

《行为、审计日志 (实时索引/实时搜索)建模 - 最佳实践 1》

《行为、审计日志 (实时索引/实时搜索)建模 - 最佳实践 2》

4、《PostgreSQL 海量时序数据(任意滑动窗口实时统计分析) - 传感器、人群、物体等对象跟踪》

3 时间、空间、业务 多维数据实时透视

1、《数据透视 - 商场(如沃尔玛)选址应用》

2、《时间+空间 实时多维数据透视》

3、《PostgreSQL\GPDB 毫秒级海量 多维数据透视 典型案例分享》

4、《PostgreSQL\GPDB 毫秒级海量 时空数据透视 典型案例分享》

4 独立事件相关性分析

1、《潘金莲改变了历史吗 - PostgreSQL舆情事件分析应用》

2、《为什么啤酒和纸尿裤最搭 - 用HybridDB/PostgreSQL查询商品营销最佳组合》

5 海量关系实时图式搜索

1、《金融风控、公安刑侦、社会关系、人脉分析等需求分析与数据库实现 - PostgreSQL图数据库场景应用》

2、《一场IT民工 与 人贩子 之间的战争 - 只要人人都献出一点爱》

6 社交业务案例

1、《PCC性能大赛 - facebook\微博 like场景 - 数据库设计与性能压测》

2、《facebook linkbench 测试PostgreSQL社交关系图谱场景性能》

7 流式数据实时处理案例

1、《流计算风云再起 - PostgreSQL携PipelineDB力挺IoT》

2、《(流式、lambda、触发器)实时处理大比拼 - 物联网(IoT)\金融,时序处理最佳实践》

3、《"物联网"流式处理应用 - 用PostgreSQL实时处理(万亿每天)》

4、《基于PostgreSQL的流式PipelineDB, 1000万/s实时统计不是梦》

5、《数据保留时间窗口的使用》

6、《实时数据交换平台 - BottledWater-pg with confluent》

8 物联网

1、《IoT(物联网)极限写入、消费 最佳实践 - 块级(ctid)扫描》

2、物联网数据有损压缩 - 旋转门压缩

《PostgreSQL 三角函数的用法举例 - 已知3点求夹角（旋转门续）》

《旋转门数据压缩算法在PostgreSQL中的实现 - 流式压缩在物联网、监控、传感器等场景的应用》

3、范围类型助力物联网

《PostgreSQL 黑科技 range 类型及 gist index 20x+ speedup than Mysql index combine query》

《PostgreSQL 黑科技 range 类型及 gist index 助力物联网(IoT)》

4、《PostgreSQL 物联网黑科技 - 瘦身几百倍的索引(BRIN index)》

5、《PostgreSQL 10 - JSON 内容全文检索》

9 海量全文检索

1、《PostgreSQL 文本数据分析实践之 - 相似度分析》

2、《PostgreSQL 如何高效解决 按任意字段分词检索的问题》

3、《PostgreSQL 全文检索加速 快到没有朋友 - RUM索引接口(潘多拉魔盒)》

4、《聊一聊双十一背后的技术 - 分词和搜索》

5、《PostgreSQL 行级 全文检索》

10 海量模糊、正则查询案例

1、《PostgreSQL 模糊查询最佳实践》

2、《中文模糊查询性能优化 by PostgreSQL trgm》

3、《聊一聊双十一背后的技术 - 毫秒分词算啥, 试试正则和相似度》

4、《PostgreSQL 百亿数据 秒级响应 正则及模糊查询》

5、《PostgreSQL 全表 全字段 模糊查询的毫秒级高效实现 - 搜索引擎颤抖了》

6、《从难缠的模糊查询聊开 - PostgreSQL独门绝招之一 GIN , GiST , SP-GiST , RUM 索引原理与技术背景》

11 海量数组、图像特征数据 实时检索

1、《电商内容去重\内容筛选应用(实时识别转载\盗图\侵权?) - 文本、图片集、商品集、数组相似判定的优化和索引技术》

2、《文本(关键词)分析理论基础 - TF/IDF》

3、《smlar插件详解》

4、《rum, smlar应用场景分析》

5、《从相似度算法谈起 - Effective similarity search in PostgreSQL》

6、《PostgreSQL 在视频、图片去重，图像搜索业务中的应用》

7、《弱水三千,只取一瓢,当图像搜索遇见PostgreSQL(Haar wavelet)》

12 数据清洗、采样、脱敏、批处理、合并

1、数据采样和脱敏实践

《PostgreSQL 数据采样与脱敏》

《PostgreSQL 巧妙的数据采样方法》

2、数据清洗和去重实践

《PostgreSQL 数据去重方法大全》

《PostgreSQL 重复 数据清洗 优化教程》

3、《数据入库实时转换 - trigger , rule》

4、《PostgreSQL 如何实现批量更新、删除、插入》

5、《PostgreSQL upsert功能(insert on conflict do)的用法》

6、《PostgreSQL 如何实现upsert与新旧数据自动分离》

7、《PostgreSQL 数据rotate用法介绍 - 按时间覆盖历史数据》

13 空间数据应用案例

1、《geohash vs PostGIS》

2、《PostgreSQL 物流轨迹系统数据库需求分析与设计 - 包裹侠实时跟踪与召回》

3、《多点最优路径规划 - (商旅问题,拼车,餐饮配送,包裹配送,包裹取件,回程单)》

4、无人驾驶背后的数据库技术

《无人驾驶背后的技术 - PostGIS点云(pointcloud)应用 - 1》

《无人驾驶背后的技术 - PostGIS点云(pointcloud)应用 - 2》

5、《PostgreSQL 百亿地理位置数据 近邻查询性能》

6、GIS 近邻查询优化

《PostgreSQL 9.1 nearest-neighbor search use gist index》

《GIS 附近查找性能优化》

7、《空间复合索引加速空间搜索》

8、《聊一聊双十一背后的技术 - 物流、动态路径规划》

9、《SRID (空间引用识别号, 坐标系)》

14 金融业务

1、金融级可靠性

《PostgreSQL 10 - 任意wal副本数，金融级高可用与可靠性并存需求》

《PostgreSQL 金融行业高可用和容灾解决方案》

《PostgreSQL 9.6 同步多副本 与 remote_apply事务同步级别》

《PG多节点(quorum based), 0丢失 HA(failover,switchover)方案》

《数据库平滑switchover的要素 - 会话资源漂移》

《PostgreSQL 10 流式物理、逻辑主从 最佳实践》

2、线性回归与数据预测实践

《PostgreSQL 多元线性回归 - 1》

《在PostgreSQL中用线性回归分析 - 实现数据预测》

《PostgreSQL 一元线性回归 - 股价预测 1》

《PostgreSQL 一元线性回归 - 股价预测 2》

《PostgreSQL 多元线性回归 - 股价预测 3》

3、《PostgreSQL 金融类账务流水数据快照分析 案例分享》

15 异步消息应用案例

1、《[转载]postgres+socket.io+nodejs实时地图应用实践》

2、《从电波表到数据库小程序之 - 数据库异步广播(notify/listen)》

3、《从微信小程序 到 数据库"小程序"》

16 海量冷热数据分离

1、《ApsaraDB的左右互搏(PgSQL+HybridDB+OSS) - 解决OLTP+OLAP混合需求》

2、《海量数据 "写入、共享、存储、计算" 最佳实践》

3、《从人类河流文明 洞察 数据流动的重要性》

17 倒排索引案例

1、《宝剑赠英雄 - 任意组合字段等效查询, 探探PostgreSQL多列展开式B树 (GIN)》

2、《PostgreSQL 聚集存储 与 BRIN索引 - 高并发行为、轨迹类大吞吐数据查询场景解说》

3、《PostgreSQL GIN 单列聚集索引 应用》

18 Greenplum 案例

1、《Greenplum 最佳实践 - 多维分析的使用(CUBE, ROLLUP, GROUPING SETS in GreenPlum and Oracle)》

2、节约98%的数据存储成本的方法

《PostgreSQL n阶乘计算, 排列组合计算 - 如何计算可变参数中有没有重复参数》

《PostgreSQL 计算 任意类型 字段之间的线性相关性》

《一个简单算法可以帮助物联网,金融 用户 节约98%的数据存储成本 (PostgreSQL,Greenplum帮你做到)》

3、《Greenplum 最佳实践 - 数据分布黄金法则 - 分布列与分区的选择》

4、《Greenplum 最佳实践 - 行存与列存的选择以及转换方法》

5、《Greenplum 最佳实践 - 估值插件hll的使用(以及hll分式聚合函数优化)》

6、《Greenplum 最佳实践 - 什么时候选择bitmap索引》

7、《PostgreSQL、Greenplum DML合并操作 最佳实践》

19 综合应用案例

1、《从天津滨海新区大爆炸、危化品监管聊聊 IT人背负的社会责任感》

2、《(AR虚拟现实)红包 技术思考 - GIS与图像识别的完美结合》

3、《从真假美猴王谈起 - 让套牌车、克隆x 无处遁形的技术手段思考》

4、《为了部落 - 如何通过PostgreSQL基因配对，产生优良下一代》

5、《用PostgreSQL描绘人生的高潮、尿点、低谷 - 窗口/帧 or 斜率/导数/曲率/微积分?》

6、《想挑战AlphaGO吗？先和PostgreSQL玩一玩?? PostgreSQL与人工智能(AI)》

7、《PostgreSQL 特性故事汇》

8、《AI(OtterTune)引波澜 - AI会洗牌数据库行业吗? DBA如何转变思想》

9、《门禁广告销售系统需求剖析 与 PostgreSQL数据库实现》

10、《PostgreSQL 与 12306 抢火车票的思考》

20 数据订阅

1、《PostgreSQL 逻辑订阅 - 给业务架构带来了什么希望？》

2、《PostgreSQL 10 - 逻辑订阅端worker数控制参数》

3、《PostgreSQL 10 - 备库支持逻辑订阅, 订阅支持主备漂移》

4、《PostgreSQL 10 - 逻辑订阅支持并行COPY初始化数据》

5、《PostgreSQL 10 - 逻辑订阅原理与最佳实践》

6、《使用PostgreSQL逻辑订阅实现 multi-master》

21 读写分离

1、《PostgreSQL 读写分离 proxy 1》

2、《PostgreSQL 读写分离 proxy 2 - 待编辑》

3、客户端高可用和读写分离

《PostgreSQL 10 - libpq支持多主机连接(failover,LB)让数据库HA和应用配合更紧密》

22 水平扩展

1、sharding 实践 1 - postgres_fdw + inherit

《PostgreSQL 10 - 支持分布式事务》

《PostgreSQL 10 - 索引扫描、子查询、VACUUM、fdw/csp钩子》

《PostgreSQL 10 - mergesort(Gather merge)》

《PostgreSQL 10 - pushdown 增强》

《PostgreSQL 10 - 支持Append节点并行》

《PostgreSQL 10 - postgres_fdw 多节点异步并行执行》

2、sharding 实践 2 - postgres_fdw + pg_pathman

《PostgreSQL 9.6 sharding based on FDW & pg_pathman》

《PostgreSQL 9.5+ 高效分区表实现 - pg_pathman》

《PostgreSQL 9.6 sharding + 单元化 (based on postgres_fdw) 最佳实践 - 通用水平分库场景设计与实践》

《PostgreSQL 9.6 单元化,sharding (based on postgres_fdw) - 内核层支持前传》

3、sharding 实践 3 - plproxy

《PostgreSQL 最佳实践 - 水平分库(基于plproxy)》

《A Smart PostgreSQL extension plproxy 2.2 practices》

《使用Plproxy设计PostgreSQL分布式数据库》

《阿里云ApsaraDB RDS for PostgreSQL 最佳实践 - 4 水平分库 之 节点扩展》

《阿里云ApsaraDB RDS for PostgreSQL 最佳实践 - 3 水平分库 vs 单机 性能》

《阿里云ApsaraDB RDS for PostgreSQL 最佳实践 - 2 教你RDS PG的水平分库》

4、sharding 实践 4 - citus - 待编辑

https://www.citusdata.com/

二、问题诊断、性能分析与优化

1、《索引顺序扫描引发的堆扫描IO放大背后的统计学原理与解决办法》

2、UUID的IO问题与实践

《PostgreSQL sharding有序UUID最佳实践 - serial global uuid stored in 64bit int8》

《PostgreSQL 优化CASE - 无序UUID性能问题诊断》

3、《自动选择正确索引访问接口(btree,hash,gin,gist,sp-gist,brin,bitmap...)的方法》

4、《优化器里的概率学 - 性能抖动原理分析》

5、《PostgreSQL 数据访问 offset 的质变 case》

6、《PostgreSQL 大行优化》

7、优化器成本因子调试

《优化器成本因子校对 - 1》

《优化器成本因子校对(disk,ssd,memory IO开销精算) - 2》

8、HINT

《PostgreSQL SQL HINT的使用(pg_hint_plan)》

《阿里云 PostgreSQL pg_hint_plan插件的用法》

《PostgreSQL 特性分析 Plan Hint》

《关键时刻HINT出彩 - PG优化器的参数优化、执行计划固化CASE》

9、《PostgreSQL 操作符与优化器详解》

10、《PostgreSQL 优化器逻辑推理能力 源码解析》

11、《聊一下PostgreSQL优化器 - in里面有重复值时PostgreSQL如何处理?》

12、《PostgreSQL SSL链路压缩例子》

13、《PostgreSQL 大表自动 freeze 优化思路》

14、《PostgreSQL的"天气预报" - 如何预测Freeze IO风暴》

15、《PostgreSQL 函数调试、诊断、优化 & auto_explain》

16、性能优化案例

《PostgreSQL性能优化综合案例讲解 - 1》

《PostgreSQL性能优化综合案例讲解 - 2》

17、《数据库界的华山论剑 tpc.org》

三、原理

1、《PostgreSQL 逻辑结构 和 权限体系 介绍》

2、数据库统计学

《PostgreSQL数据库监控中的统计学 - 对象SIZE的数据分布图》

《用PostgreSQL了解一些统计学术语以及计算方法和表示方法 - 1》

《population & sample covariance, standard deviation Aggregate in PostgreSQL》

《PostgreSQL 统计信息之 - 逻辑与物理存储的线性相关性》

3、聚合函数知识

《PostgreSQL aggregate function 1 : General-Purpose Aggregate Functions》

《PostgreSQL aggregate function 2 : Aggregate Functions for Statistics》

《PostgreSQL aggregate function 3 : Aggregate Functions for Ordered-Set》

《PostgreSQL aggregate function 4 : Hypothetical-Set Aggregate Functions》

4、数据库聚合函数运算原理

《PostgreSQL aggregate function customize》

5、分布式聚合函数运算原理

《Postgres-XC customized aggregate introduction》

6、《PostgreSQL 聚合代码优化 - OP复用浅析》

7、函数稳定性

《函数稳定性讲解 - 1》

《函数稳定性讲解 - 2》

《函数稳定性讲解 - 3》

8、《PostgreSQL nestloop/hash/merge join讲解》

9、《PostgreSQL bitmapAnd, bitmapOr, bitmap index scan, bitmap heap scan》

10、《PostgreSQL 10 - 间接索引(secondary index)》

11、《PostgreSQL 10 - 不完整索引支持复合排序》

12、《PostgreSQL 10 - 唯一约束+附加字段组合功能索引》

13、《深入浅出PostgreSQL B-Tree索引结构》

14、《PostgreSQL GIN索引实现原理》

15、《PostgreSQL GIN multi-key search 优化》

16、《懒人推动社会进步 - 多列聚合, gin与数据分布(选择性)》

17、《索引扫描优化之 - GIN数据重组优化(按元素聚合) 想象在玩多阶魔方》

18、《从一维编排到多维编排，从平面存储到3D存储 - 数据存储优化之路》

19、《列存优化(shard,大小块,归整,块级索引,bitmap scan) - (大量数据实时读写)任意列搜索》

20、字符集知识

《PostgreSQL Server Encoding sql_ascii attention》

《PostgreSQL SQL_ASCII encoding introduce》

21、数据库动态库介绍

《PostgreSQL 加载动态库详解》

《如何加快PostgreSQL结巴分词加载速度》

22、《PostgreSQL FSM 原理》

23、《PostgreSQL 如何精确计算表膨胀(fsm,数据块layout讲解) - PostgreSQL table exactly bloat monitor use freespace map data》

24、《PostgreSQL 逻辑备份一致性讲解》

25、《PostgreSQL 共享事务快照功能》

26、《PostgreSQL 事务快照功能》

27、《PostgreSQL 并行逻辑备份与一致性讲解》

28、《异步流复制模式如何保证不丢数据》

29、《执行计划选择算法 与 绑定变量》

30、《生成泊松、高斯、指数、随机分布数据》

31、《PostgreSQL 事件触发器 - PostgreSQL 9.3 Event Trigger》

32、《PostgreSQL 隐藏参数详解》

33、《PostgreSQL 9种索引的原理和应用场景》

四、数据库发展方向、数据库选型

1、《数据库任督二脉 - 数据与计算的生态融合》

2、HTAP

《PostgreSQL 10 - 推出JIT开发框架(朝着HTAP迈进)》

《PostgreSQL 10 - OLAP增强 向量聚集索引(列存储扩展)》

《PostgreSQL 10 - OLAP提速框架, Faster Expression Evaluation Framework(含JIT)》

《PostgreSQL 向量化执行插件(瓦片式实现) 10x提速OLAP》

《分析加速引擎黑科技 - LLVM、列存、多核并行、算子复用 大联姻 - 一起来开启PostgreSQL的百宝箱》

《100TB+, 日增量1TB的OLTP OLAP混合场景数据库设计方向》

3、多核并行

《PostgreSQL 10 - 控制集群并行度》

《PostgreSQL 10 - tuplesort 多核并行创建索引》

《PostgreSQL 9.6 并行计算 优化器算法浅析》

《PostgreSQL 9.6 引领开源数据库攻克多核并行计算难题》

4、《数据库选型之 - 大象十八摸 - 致 架构师、开发者》

5、《数据库选型思考》

6、《PostgreSQL 前世今生》

7、《论云数据库编程能力的重要性》

8、《Oracle业务适合用PostgreSQL去O的一些评判标准》

五、开发技巧

1、递归应用

《PostgreSQL : WITH Queries use case》

《PostgrSQL 递归SQL的几个应用 - 极客与正常人的思维》

《PostgreSQL 递归查询CASE - 树型路径分组输出》

《PostgreSQL Oracle 兼容性之 - WITH 递归 ( connect by )》

《用PostgreSQL找回618秒逝去的青春 - 递归收敛优化》

《distinct xx和count(distinct xx)的变态递归优化方法 - 索引收敛(skip scan)扫描》

《PostgreSQL 使用递归SQL 找出数据库对象之间的依赖关系》

《PostgreSQL 递归死循环案例及解法》

《PostgreSQL 递归查询一例 - 资金累加链》

《递归优化CASE - group by & distinct tuning case : use WITH RECURSIVE and min() function》

《递归优化CASE - performance tuning case :use cursor\trigger\recursive replace (group by and order by) REDUCE needed blockes scan》

《PostgreSQL 树状数据存储与查询(非递归) - Use ltree extension deal tree-like data type》

《PostgreSQL Oracle 兼容性之 - connect by》

2、advisory lock应用

《PostgreSQL 使用advisory lock实现行级读写堵塞》

《PostgreSQL 无缝自增ID的实现 - by advisory lock》

《PostgreSQL 使用advisory lock或skip locked消除行锁冲突, 提高几十倍并发更新效率》

3、《PostgreSQL 如何创建不等于索引》

4、《PostgreSQL update returning NEW|OLD column value 在对账|购票|防纂改|原子操作中的妙用》

5、《如何防止数据库雪崩》

6、《随机记录并发查询与更新(转移、删除)的"无耻"优化方法》

7、《PostgreSQL 随机查询优化》

8、《论count与offset使用不当的罪名 和 分页的优化》

9、《聊一聊双十一背后的技术 - 不一样的秒杀技术, 裸秒》

10、《PostgreSQL 聚合表达式 FILTER , order , within group 用法》

11、《PostgreSQL schemaless 的实现 (类mongodb collection)》

12、《行列变换》

13、可变参数函数开发

《variable number of arguments function》

《PostgreSQL plpgsql variadic argments , parameters - 可变参数个数》

14、触发器开发

《PostgreSQL 触发器 用法详解 1》

《PostgreSQL 触发器 用法详解 2》

15、《PostgreSQL 事务，会话 GUC 变量 妙用 - 获取并跟踪事务结束时间》

16、《在PostgreSQL中实现update | delete limit》

17、《在PostgreSQL中实现按拼音、汉字、拼音首字母搜索的例子》

18、《PostgreSQL 数组忽略大小写匹配》

19、《PostgreSQL 中如何找出记录中是否包含编码范围内的字符，例如是否包含中文》

20、《如何判断字符串是否为合法数值、浮点、科学计数等格式》

21、《如何按拼音排序 - 数据库本土化特性(collate, ctype, ...)》

22、《PostgreSQL 中生成随机汉字》

23、《PostgreSQL全角、半角互相转换》

24、《聊聊between and的坑 和 GEEK的解法》

25、《如何在PostgreSQL中调试plpgsql存储过程(pldebugger, pldbgapi)》

26、《如何优雅的修改被视图引用的表字段》

27、《采用 部分索引、表达式索引 提高搜索效率》

28、《PostgreSQL 表达式索引 - 语法注意事项》

29、《PostgreSQL UDF实现IF NOT EXISTS语法》

30、《PostgreSQL 9.6 黑科技 bloom 算法索引，一个索引支撑任意列组合查询》

31、《找对业务G点, 体验酸爽 - PostgreSQL内核扩展指南》

32、《一张表有且只有一条记录(续) - 支持插入，并且更新、删除都只作用在最后一条记录上, 查询也只时间最大的记录。》

33、《人分九等，数有阶梯 - PostgreSQL 阶品（颗粒）分析函数width_bucket, kmean应用》

34、《advisory lock 实现高并发非堵塞式 业务锁》

35、《云端海量任务调度数据库最佳实践 - 阿里云RDS PostgreSQL案例》

六、备份恢复

1、逻辑备份与恢复

《PostgreSQL Logical Backup's TOC File》

《PostgreSQL 最佳实践 - 在线逻辑备份与恢复介绍》

2、基于全量数据文件和归档的增量备份与恢复

《PostgreSQL recovery target introduce》

《PostgreSQL PITR THREE recovery target MODE: name,xid,time USE CASE - 1》

《PostgreSQL PITR THREE recovery target MODE: name,xid,time USE CASE - 2》

《PostgreSQL standby recover的源码分析 (walreceiver唤醒时机？ 为什么standby crash后walreceiver不会立即被唤醒?)》

《PostgreSQL 最佳实践 - 在线增量备份与任意时间点恢复》

3、基于ZFS快照和归档的增量备份与恢复

《PostgreSQL 最佳实践 - 块级增量备份(ZFS篇)方案与实战》

《PostgreSQL 最佳实践 - 块级增量备份(ZFS篇)备份集自动校验》

《PostgreSQL 最佳实践 - 块级增量备份(ZFS篇)单个数据库采用多个zfs卷(如表空间)时如何一致性备份》

《PostgreSQL 最佳实践 - 块级增量备份(ZFS篇)双机HA与块级备份部署》

《PostgreSQL 最佳实践 - 块级增量备份(ZFS篇)验证 - recovery test script for zfs snapshot clone + postgresql stream replication + archive》

4、基于数据文件块级增量和归档的增量备份与恢复

《PostgreSQL 最佳实践 - 块级别增量备份(pg_rman baseon LSN)源码浅析与使用》

《PostgreSQL 最佳实践 - pg_rman 以standby为源的备份浅析》

《PostgreSQL 最佳实践 - pg_rman 数据库恢复示例 与 软件限制解说》

5、误操作闪回

《PostgreSQL 回收站功能 - 基于HOOK的recycle bin pgtrashcan》

《PostgreSQL 闪回 - flash back query emulate by trigger》

6、误操作恢复

《PostgreSQL 使用pg_xlogdump找到误操作事务号》

7、灾难恢复

《异版本pg_resetxlog后导致的控制文件差异问题处理》

《使用pg_resetxlog修复PostgreSQL控制文件的方法》

《PostgreSQL 数据文件灾难恢复 - 解析与数据dump》

8、《Gitlab从删库到恢复 - 数据库备份恢复容灾HA的靠谱姿势》

七、安全、审计

1、《PostgreSQL 密码安全指南》

2、《PostgreSQL 数据库安全指南》

3、《PostgreSQL数据库在上市公司重要应用中的SOX审计》

4、《DBA专供 冈本003系列 - 数据库安全第一,过个好年》

5、《DBA一族九阳神功秘籍，标准和制度(含重大节日)》

6、《PostgreSQL 10 - SASL认证方法 之 scram-sha-256 安全认证机制》

7、《PostgreSQL 10 - 可配置是否允许执行不带where条件的updatedelete》

8、《PostgreSQL views privilege attack and security with security_barrier(视图攻击)》

10、《固若金汤 - PostgreSQL pgcrypto加密插件》

11、审计

《PostgreSQL 事件触发器 - DDL审计 , DDL逻辑复制 , 打造DDL统一管理入口》

《PostgreSQL 触发器应用 - (触发器WHEN)前置条件过滤跟踪目标记录》

《PostgreSQL 触发器应用 - use trigger audit record which column modified, insert, delete.》

《PostgreSQL 跟踪谁动了你的记录 - 1》

《PostgreSQL 跟踪谁动了你的记录 - 2》

《USE hstore store table's trace record》

10、《PostgreSQL 转义、UNICODE、与SQL注入》

八、DBA技巧

1、《DBA不可不知的操作系统内核参数》

2、《从PostgreSQL支持100万个连接聊起》

3、《PostgreSQL on Linux 最佳部署手册》

4、《Linux 性能诊断 perf使用指南》

5、《PostgreSQL 源码性能诊断(perf profiling)指南》

6、《PostgreSQL 锁等待监控 珍藏级SQL - 谁堵塞了谁》

7、《PostgreSQL 如何查找TOP SQL (例如IO消耗最高的SQL)》

8、《PostgreSQL 清理redo(xlog,wal,归档)的机制 及 如何手工清理》

9、《PostgreSQL物理"备库"的哪些操作或配置，可能影响"主库"的性能、垃圾回收、IO波动》

10、《从redo日志分析数据库的profile》

11、《MySQL 增量同步到 PostgreSQL》

12、《PostgreSQL 收缩膨胀表或索引 - pg_squeeze or pg_repack》

13、《PostgreSQL relcache在长连接应用中的内存霸占"坑"》

14、《PostgreSQL 老湿机图解垃圾回收的"坑"》

15、《论数据库redo/data存储规划与SSD写倾斜》

16、垃圾回收相关

16.1、数据库DATA BLOCK剩余空间跟踪原理

《PostgreSQL Free Space Map Principle》

16.2、如何计算对象膨胀

《PostgreSQL 如何精确计算表膨胀(fsm,数据块layout讲解) - PostgreSQL table exactly bloat monitor use freespace map data》

16.3、为什么长事务可能会导致膨胀

《PostgreSQL 垃圾回收代码分析 - why postgresql cann't reclaim tuple is HEAPTUPLE_RECENTLY_DEAD》

16.4、如何防止膨胀

《PostgreSQL 垃圾回收原理以及如何预防膨胀 - How to prevent object bloat in PostgreSQL》

《PostgreSQL snapshot too old补丁, 防止数据库膨胀》

《PostgreSQL 老湿机图解平安科技遇到的垃圾回收"坑"》

16.5、为什么需要FREEZE，如何防止FREEZE风暴

《PostgreSQL 的"天气预报" - 如何预测Freeze IO风暴》

《PostgreSQL 大表自动 freeze 优化思路》

《PostgreSQL 9.6 vacuum freeze大幅性能提升 代码浅析》

16.6、如何优雅的处理膨胀对象

《PostgreSQL 收缩膨胀表或索引 - pg_squeeze or pg_repack》

16.7、如何监控垃圾回收进程的开销

《PostgreSQL 10.0 preview 功能增强 - SQL执行剩余时间 - 垃圾回收过程可视pg_stat_progress_vacuum》

《PostgreSQL 10.0 preview 功能增强 - 新增数十个IO等待事件监控》

16.8、如何优化GIN索引的VACUUM锁

《PostgreSQL 10.0 preview 性能增强 - GIN索引vacuum锁降低》

16.9、备库为什么可能影响主库的垃圾回收

《PostgreSQL 物理"备库"的哪些操作或配置，可能影响"主库"的性能、垃圾回收、IO波动》

16.10、影响或控制垃圾回收的参数或因素

《影响或控制PostgreSQL垃圾回收的参数或因素》

九、更多实时文章请参考

digoal github