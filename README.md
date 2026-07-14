# Hello-GitHub
This project help you to use GitHub

## 📚 学习目录

#### 第一阶段：基础核心 (必学)

**1. 起步与概念**
*   **版本控制是什么**：理解为什么需要版本控制，以及集中式（SVN）与分布式（Git）的区别。
*   **Git 安装与配置**：安装 Git，设置用户名、邮箱 (`git config`)，理解配置文件优先级。
*   **帮助系统**：学会使用 `git help` 和 `git <命令> --help` 获取文档。

**2. 日常基本操作**
*   **创建仓库**：`git init` 初始化仓库，`git clone` 克隆现有项目。
*   **记录变更**：理解工作区、暂存区、本地仓库的关系；掌握 `git add`、`git commit`、`git status`、`git log` 查看提交历史。
*   **差异对比**：`git diff` 查看工作区和暂存区的差异，`git diff --staged` 查看暂存区与上次提交的差异。

**3. 撤销与修正**
*   用 `git checkout -- <file>` 丢弃工作区修改。
*   用 `git reset` 撤销暂存 (`git reset HEAD <file>`)。
*   用 `git commit --amend` 修改最后一次提交信息或内容。

#### 第二阶段：分支与合并 (进阶核心)

**4. 分支管理**
*   **分支本质**：理解 Git 分支是基于指针的轻量级特性。
*   **基本操作**：创建 (`git branch`)、切换 (`git checkout`/`git switch`)、删除分支。
*   **合并**：`git merge`，理解快进合并 (`Fast-forward`) 和三方合并 (`3-way merge`)，以及合并冲突的处理。

**5. 变基 (Rebase)**
*   理解 `git rebase` 与 `git merge` 的区别：变基产生线性历史，合并保留分支历史。
*   使用交互式变基 (`git rebase -i`) 整理、合并、重排提交历史。

#### 第三阶段：协作与远程 (团队必备)

**6. 远程仓库**
*   `git remote` 管理远程仓库，`git remote -v` 查看链接。
*   `git push` 推送本地分支到远程，`git pull` (等于 `git fetch` + `git merge`) 拉取远程更新。
*   **跟踪分支**：理解本地分支与远程跟踪分支的关系 (`origin/branch`)。

**7. 工作流模型**
*   **Git Flow**：经典的分支管理模型 (Master/Develop/Feature/Release/Hotfix)。
*   **GitHub Flow**：更简单的模型，主打功能分支加Pull Request。
*   **Pull Request / Merge Request**：理解协作流程，进行代码审查。

#### 第四阶段：高级工具与故障排查 (专家之路)

**8. 修改历史与恢复**
*   `git reflog`：查看所有历史操作，用于恢复丢失的提交或重置。
*   `git reset` 深入：理解 `--soft`、`--mixed`、`--hard` 的区别。
*   `git cherry-pick`：将其他分支的特定提交应用到当前分支。

**9. 调试与二分查找**
*   `git bisect`：通过二分查找定位引入 bug 的提交。
*   `git blame`：查看文件的每一行是谁、在什么时间修改的。

**10. 子模块与子树**
*   `git submodule`：在仓库中引用其他仓库（有独立性）。
*   `git subtree`：另一种管理嵌套仓库的方式（更适合简化依赖管理）。

**11. Git Hooks**
*   理解 Git 钩子（客户端钩子如 `pre-commit`，服务端钩子如 `pre-receive`）。
*   用于自动化检查、格式化代码、生成文档等。

**12. 其他主题**
*   **Git LFS (Large File Storage)**：处理大文件。
*   **Git 性能优化**：浅克隆 (`git clone --depth`) 等。
*   **迁移**：从 SVN (`git svn`) 或其他 VCS 迁移到 Git。

### 📖 推荐学习资源

| 类型 | 推荐 | 说明 |
| :--- | :--- | :--- |
| **必读教程** | **Pro Git (中文版)** | 官方推荐，内容最权威，覆盖上述所有目录，**免费在线阅读**。 |
| **在线交互** | **Learn Git Branching** | 可视化和交互式学习分支与合并，效果极佳。 |
| **速查手册** | **GitHub Git Cheat Sheet** | 官方命令速查表。 |
| **模拟练习** | **Oh My Git!** | 一个用游戏学习 Git 的开源项目。 |

### 💡 学习建议
*   **理论结合实践**：每学一个章节，都在终端或 IDE 里亲手敲一遍命令。
*   **先掌握核心命令**：初期应重点掌握 `add`、`commit`、`push`、`pull`、`branch`、`merge` 和 `rebase` 这 7 个核心操作。
*   **敢于尝试**：Git 几乎所有的操作都是可撤销的，不用害怕弄坏。可以建一个测试仓库，安全地试错。
