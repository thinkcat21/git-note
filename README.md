# git使用笔记

- 通过文件名搜索提交记录，filename需包含相对路径
```bash
git log --follow -- <filename>  #当前分支搜索
git log --all --follow -- <filename>   #全部分支搜索
'''

- 通过commitID搜索提交所在分支
```bash
git branch --contains <commitID>  #本地分支
git branch -r --contains <commitID>  #远程分支
git branch -a --contains <commitID>  #本地和远程
'''
