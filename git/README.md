##Git

#merge

1. 会产生一个新的commit
2. 历史保存完整

#rebase

1. 不会产生一个新的commit
2. 会影响已经有的commit
3. 相当于改变了分支创建节点
4. The golden rule of git rebase is to never use it on public branches.

#改变上一个commit
git commit --amend

#改变多个commit
git rebase -i HEAD~3

#生成patch

1. git format-patch xxxxxxxxxxxxx(commit id)
2. git format-patch -n
3. git format-patch commit-id-1 commit-id-2