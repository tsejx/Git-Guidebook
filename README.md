﻿# Git 面对不同的场景的命令使用

Tags: git

---

 - 初始化
   - git init
 - 克隆项目
  - git clone
 - 长期保存密码
   - git config --global credential.helper store
 - 获取分支
   - git fetch origin
 - 合并分支
   - git merge
 - 获取并且合并分支
   - git pull origin
 - 切换分支
   - git checkout
 - 新建并切换分支
   - git checkout -d
 - 删除分支
   - git branch -d
 - 查看修改状态
   - git status
 - 查看所有的修改内容
   - git diff
 - 查看指定文件修改内容
   - git diff <file>
 - 添加指定文件到暂存区
   - git add
 - 添加所有文件到暂存区
   - git add all
 - 查看已经在提交区（即已经add了的）所有修改内容
   - git diff --cached
 - 提交暂存区修改到本地
   - git commit -m 'description'
 - 修改刚才提交的描述
   - git commit --amend -m ''
 - 提交本地版本到远端
   - git push origin
 - 其他分支有紧急问题，需要马上切过去处理，但当前分支只改了一半，又不想commit
   - git stash
 - 处理完其他分支的紧急问题以后，回到原先分支继续修改
   - git stash pop
 - 清除所有没有add了得修改
   - git checkout .
 - 清除指定没有add了的文件的修改
   - git checkout
 - 清除untracked的文件
  - git clean -fd
 - 清除git ignore了的文件
  - git clean -x
 - commit了修改到本地，想放弃这个commit
  - git reset HEAD~
 - commit了修改到本地，想放弃这个commit，并清空修改
  - git reset --hard HEAD~
 - commit了修改到本地，想恢复特定文件成指定的历史版本
  - git checkout --
 - 打标签
  - git tag -a v1.0 -m 'somthing message'
 - 删除标签
  - git tag -d v1.0
 - 列出所有标签
  - git tag
 - 推送特定标签到远端
  - git push origin v1.0
 - 推送所有标签
  - git push origin --tags
 - 删除远端tag
  - git push origin -d tag v1.0
 - 远程仓库
  - git remote
 - 添加远程仓库
  - git remote add
 -  查看过去版本的历史记录
  - git log
 - 查看命令历史
  - git relog
 - 回退版本
  - git reset
   
