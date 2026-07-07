# 发布

## `publish`命令

正式版的预期是总结预发布的所有更新，而非简单地和上一个版本比较。

## `audit`命令

AI特别喜欢绕过预设的Skill和CLI自己乱跑。所以audit需要能够发现和契约不符合的地方。

常见的问题有：
- 只有tag和release，没有CHANGELOG
- 只有CHANGELOG和tag，没有release

从反脆弱的角度考虑，还需要audit根据contract约定给一些建议。比如说，如果缺失了CHANGELOG，修改tag就会改变事实源。缺失了GithHub release，似乎可以直接补充。

目前的根本原因是，devops-release命令和cli无法面对AI制造的海量不遵守流程随意跳过去的混乱。

## 服务端

当前的命令已经超过了本地的处理能力，需要考虑到云端修复海量的release问题。类似地也可以逐渐把全过程的修复都移到云端，并且在限定的智能体环境内运行。
