## 如何开始学习

1. 拉取项目
```bash
git clone git@github.com:wzp-coding/vben-admin-study.git
```

2. 新建自己的开发分支
```bash
# 基于master创建分支
# feat开头：表示这个分支新增一个特性功能
# xxx：简单描述功能
# wzp：最后以自己的名称缩写结尾
# eg: feat_add_antdvue_wzp
git checkout -b feat_xxx_wzp origin/master
```

3. 开发完成准备提PR的时候先rebase一下
```bash
# 前面基于master创建分支，则基于master作rebase操作
git rebase origin/master
```

## Git 提交规范

- 参考 [vue](https://github.com/vuejs/vue/blob/dev/.github/COMMIT_CONVENTION.md) 规范 ([Angular](https://github.com/conventional-changelog/conventional-changelog/tree/master/packages/conventional-changelog-angular))

  - `feat` 增加新功能
  - `fix` 修复问题/BUG
  - `style` 代码风格相关无影响运行结果的
  - `perf` 优化/性能提升
  - `refactor` 重构
  - `revert` 撤销修改
  - `test` 测试相关
  - `docs` 文档/注释
  - `chore` 依赖更新/脚手架配置修改等
  - `workflow` 工作流改进
  - `ci` 持续集成
  - `types` 类型定义文件更改
  - `wip` 开发中
  
```bash
# eg.
git commit -m 'feat: 新增xxx功能';
```
