# Minyi Jiang · Unity / C#

关注移动游戏开发、玩法系统、编辑器工具，以及异步任务与数据一致性。

## 近期工程演示

以下三个项目于 **2026-10-30** 独立新建，使用 AI 辅助实现，并通过可执行规格测试验证。代码、测试和示例数据为本次新编写；它们是工程演示，不是雇主生产代码或过去的商业交付。

| 项目 | 重点 | 从哪里开始 |
| --- | --- | --- |
| [offline-save-sync-lab](https://github.com/jiangminyi/offline-save-sync-lab) | 离线意图日志、CAS 冲突、幂等重试、多设备同步、过期响应隔离 | README 中的故障场景与规格测试 |
| [deterministic-puzzle-engine](https://github.com/jiangminyi/deterministic-puzzle-engine) | 不可变棋盘、确定性重放、撤销重做、有界最短路径搜索 | 720 个排列的独立参考模型对照 |
| [async-resource-lifecycle-lab](https://github.com/jiangminyi/async-resource-lifecycle-lab) | 并发请求合并、独立取消、引用租约、代际隔离与释放 | 取消／完成竞态及迟到结果回收规格 |

每个项目包含核心库、命令行演示、测试、设计取舍和已知限制。核心目标为 .NET Standard 2.1，演示与规格使用 .NET 9；当前未宣称完成 Unity 编辑器集成或生产部署。

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
