## 初始化

git .init

## 基本步骤   工作区→暂存区→仓库

## 先进行文件跟踪

添加到工作区就是进行了文件跟踪

## 到暂存区

git add 文件名

git add . (添加所有文件到暂存区)

## 到仓库

git commit -m "自我标识的修改信息" 

## 查看文件当前状态

git status  || git status -s (精简模式)

## 撤销当前修改（到上一个仓库内的状态）

git checkout -- 文件名   （慎用）

## 取消文件的暂存

git reset HEAD 要移除暂存的文件名 

git reset HEAD .    移除所有文件的暂存

## 跳过暂存区（直接提交到仓库内）

git commit -a -m   ''自我标识的修改信息''

##移除文件 

移除仓库和工作区中的文件 ：  git rm -f 文件名

只移除仓库中的文件 ： git rm --cached 文件名

## 查看修改历史

git log (最近的提交历史 展示在最上方) 

## 退回到指定修改历史处 

第一步 ：git log --pretty =oneline   (打印所有修改的历史)

第二步 ：git reset --hard (要退回地方的ID)

(若想要再跳转回最新修改处的地方

第三步 ：git reflog --pretty=onelone  (查看所有修改历史

第四步 ：git reset --hard (要退回地方的ID)



