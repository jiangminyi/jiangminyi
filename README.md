# Minyi Jiang · Unity / C#

关注移动游戏开发、玩法系统、编辑器工具，以及异步任务与数据一致性。

## 近期工程演示

以下十个项目于 **2026-10-30** 独立新建，使用 AI 辅助实现，并通过可执行规格测试验证。代码、测试和示例数据为本次新编写；它们是工程演示，不是雇主生产代码或过去的商业交付。

| 项目 | 重点 | 从哪里开始 |
| --- | --- | --- |
| [offline-save-sync-lab](https://github.com/jiangminyi/offline-save-sync-lab) | 离线意图日志、CAS 冲突、幂等重试、多设备同步、过期响应隔离 | README 中的故障场景与规格测试 |
| [deterministic-puzzle-engine](https://github.com/jiangminyi/deterministic-puzzle-engine) | 不可变棋盘、确定性重放、撤销重做、有界最短路径搜索 | 720 个排列的独立参考模型对照 |
| [async-resource-lifecycle-lab](https://github.com/jiangminyi/async-resource-lifecycle-lab) | 并发请求合并、独立取消、引用租约、代际隔离与释放 | 取消／完成竞态及迟到结果回收规格 |
| [event-sourced-workflow-lab](https://github.com/jiangminyi/event-sourced-workflow-lab) | 事件溯源、CAS 追加、命令幂等、快照和事件版本升级 | 并发命令与快照／完整历史对照规格 |
| [rate-limit-scheduler-lab](https://github.com/jiangminyi/rate-limit-scheduler-lab) | 注入时钟、令牌桶、漏桶、优先级公平调度 | 限流边界、调度顺序与取消规格 |
| [incremental-dependency-graph](https://github.com/jiangminyi/incremental-dependency-graph) | 拓扑排序、环检测、脏节点传播和值缓存 | 随机 DAG 与全量求值参考对照 |
| [spatial-query-engine](https://github.com/jiangminyi/spatial-query-engine) | 动态空间索引、范围／邻域查询和坐标边界 | 随机增删改查与暴力模型对照 |
| [transactional-state-store](https://github.com/jiangminyi/transactional-state-store) | 乐观可串行化事务、读写冲突、墓碑版本、幻读验证 | 写偏斜、ABA 与并发转账规格 |
| [deterministic-simulation-lab](https://github.com/jiangminyi/deterministic-simulation-lab) | 整数固定步长、输入日志、状态哈希和有界回滚 | 迟到输入重模拟与直接运行对照 |
| [binary-protocol-framing-lab](https://github.com/jiangminyi/binary-protocol-framing-lab) | 流式分帧、CRC32C、内存边界与终止错误语义 | 随机分片、全部截断和逐位损坏规格 |

每个项目包含核心库、命令行演示、测试、设计取舍和已知限制。核心目标为 .NET Standard 2.1 或 .NET 9，以各仓库为准；演示与规格使用 .NET 9，未完成 Unity 编辑器集成或生产部署验证。

建议从一个具体失效场景开始阅读：先看设计中的约束，再定位实现和对应测试。并发与数据一致性可从存档同步、资源生命周期、事务存储入手；算法与运行时可从依赖图、空间查询、回滚模拟入手；网络与服务端基础可从协议解析、限流调度、事件溯源入手。

## 其他公开项目

- [IDRPG3D](https://github.com/jiangminyi/IDRPG3D)：闲置类 3D RPG 项目，包含 Unity 客户端、服务端与协议目录；所依赖框架见该仓库说明。
- [RPGIDLE](https://github.com/jiangminyi/RPGIDLE)：包含 Game Framework / Star Force 示例说明的 Unity 学习项目，保留上游归属与许可。
- [KongEt](https://github.com/jiangminyi/KongEt)：ET 框架学习与实践，框架能力与原作者贡献按上游文档区分。

较早的 Unity 实验保留在仓库列表中，运行条件以各自记录的编辑器版本为准；未在本次重新构建验证。

## 商业作品

参与开发的公开手游作品：

- [Screw Away](https://apps.apple.com/us/app/id6547835725)
- [Cube Out 3D](https://apps.apple.com/us/app/cube-out-3d-jam-puzzle/id6670752130)
- [Diamond Flow / Gems Match](https://apps.apple.com/us/app/id6758003426)

此处仅提供公开商店页面；上述商业产品的源码与资源不包含在工程演示仓库中。
