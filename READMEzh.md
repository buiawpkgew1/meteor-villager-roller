
# Meteor 村民滚筒

![检查](https://github.com/wsdfafw/meteor-villager-roller/actions/workflows/checks.yml/badge.svg) ![开发构建](https://github.com/wsdfafw/meteor-villager-roller/actions/workflows/devbuild.yml/badge.svg)

附加组件该改变村民专业，直到找到所需的交易

## 版本

| 我的世界        | 流星               | 支持服务         | 下载                                                                                                                                      |
| ----------- | ---------------- | ------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| 1.19.2      | 0.5.1-dev >1573  | 是吗？          | [1.3.3](https://github.com/maxsupermanhd/meteor-villager-roller/releases/download/1.3.3/villager-roller-1.3.3+mc1.19.2-rev.b66ca6d.jar) |
| 1.19.1      | 0.5.1-dev >1570  | 在这一点上我不知道    | [1.3.2](https://github.com/maxsupermanhd/meteor-villager-roller/releases/download/1.3.2/villager-roller-1.3.2+mc1.19.1-rev.bd5aa5e.jar) |
| 1.19        | 0.5.0-dev >=1563 | 谁知道此时        | [1.3.1](https://github.com/maxsupermanhd/meteor-villager-roller/releases/download/1.3.1/villager-roller-1.3.1+mc1.19-build.34.jar)      |
| 1.19        | 0.5.0-dev <1563  | Ask seasnail | [1.3](https://github.com/maxsupermanhd/meteor-villager-roller/releases/download/1.3/villager-roller-1.3+mc1.19-rev.b16e705.jar)         |
| 1.18.2      | 0.4.9            | Ask seasnail | [1.3](https://github.com/maxsupermanhd/meteor-villager-roller/releases/download/1.3/villager-roller-1.3+mc1.18.2-rev.3d6f694.jar)       |
| 1.18.1      | ?                | 自己编译         | [1.2.1](https://github.com/maxsupermanhd/meteor-villager-roller/releases/download/1.2.1/villager-roller-1.2.1.jar)                      |
| 1.18        | ?                | 自己编译         | No                                                                                                                                      |
| 1.17.1      | ?                | 自己编译         | No                                                                                                                                      |
| 1.17        | ?                | 自己编译         | No                                                                                                                                      |
| 1.16 1.16.x | ?                | 自己编译         | No                                                                                                                                      |
| < 1.16      | ?                | 不支持          | No                                                                                                                                      |

\* 导入因流星重新排列而需要的修改 (可以在提交 252e479中找到)

### 旧版本警告

我会尝试将jars存档在发布部分，但我强烈建议使用最新的开发构建和必要时使用viafabric。

## 解决用例

附加组件是针对那些在服务器上玩耍并试图在图书管理员上寻找附魔的无情人的。 没有其他行业/职业的功能，您可以拉取请求，如果您真的想要的话。

## 如何？

1. 获取村民(不是尼威特)
2. 获取 *一些* 个讲师(32个讲师很好)
3. (推荐, 不需要) 获取轴, 更好的质量- 更快的滚动速度
4. 定义你自己和村民在没有自由移动的实体和区块的空间第1步(村民和你除外)
5. 阻止村民在四周行驶(平板、方块、楼梯、 *不是陷阱* 因为那些没有路径的人)
6. 放置一个讲师，村民可以使用它，并确保可以手动做专业工作
7. 根据您的需要配置模块并启用它
8. 从聊天消息中关注方块和村民的选择
9. 单独运行模块(切换窗口焦点可能打开暂停菜单， *暂停滚动* 如果启用了“暂停屏幕”选项， 如果你知道你在做什么，请禁用它)
10. Profit!

## 常见问题

- 它说过两次"我们见到你的村民"，停止 \
  附加组件是为了在服务器上运行。 单人播放器和插件可以干扰商人屏幕的行为方式，不能做任何事情。
- 我不能再与村民交互 \
  查看上面的屏幕异步可以通过重新连接的服务器来修复。 没有任何事情可以做到。
- 它不会将讲座重新放置 \
  它确实会将讲座重新放置起来。 如果失败，则意味着无法放置方块，因为玩家、村民、其他实体或方块已经占领了该方块。 由于这个原因，滚动过程将会中断，但将在手动布局后恢复。
- 滚动 \
  时关闭聊天/叠加层/屏幕。 是，因为没有办法不： 当请求与村民互动时，客户端将强制打开商家屏幕(将替换当前屏幕)，并打开该屏幕以从村民获取交易列表。 切换“暂停屏幕”将防止任何屏幕打开时的新交互(至于强制关闭), 当你完成了你想要的操作后，你可以与村民手动交互来恢复滚动。
- 它不收集讲师，当他们耗尽 \
  搜索时无法安放他们， 在实地寻找和搬到特定物品是困难的和有误的， 那里总是有机会让所有讲师从玩家身边飞走，最终会有空手。 如果你真的想要的话，你可以通过设定希望者或流水来优化它。 如果你想要，可以自由地执行非破坏性的向丢弃物品的移动。
- 它总是滚动到最好的附魔水平 \
  将村民滚刀更新到1.2
