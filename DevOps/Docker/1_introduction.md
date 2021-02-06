# Docker介绍

## 1 引言
实际开发中，我们常常碰到以下问题
1. 开发和测试环境不一致
2. 多用户操作系统下，会相互影响
3. 运维成本高
4. 安装软件成本高

## 2 由来
美国一家做PAAS的公司将核心技术进行了开源

## 3 思想
1. 集装箱
  - 会将所有需要内容放到不同集装箱中，需要这些环境的时候直接拿这个集装箱就可以了
2. 标准化
  - 运输的标准化：所有的集装箱都放在“码头”上
  - 命令的标准化：Docker提供了一系列的命令帮助获取集装箱
  - 提供了REST API：衍生出了很多图形化界面，比如Rancher
3. 隔离性
  - Docker在运行集装箱内容的时候，会在Linux内核中单独开辟一片空间，这片空间不会影响到其它程序

其它：
- 注册中心：超级码头，用于放集装箱
- 镜像：集装箱
- 容器：运行起来的镜像