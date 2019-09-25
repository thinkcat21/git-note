# git使用笔记

### 通过文件名搜索提交记录

    git log --follow -- <filename>  #当前分支搜索
    git log --all --follow -- <filename>   #全部分支搜索
    #注：filename需包含相对路径

### 通过commitID搜索提交所在分支

    git branch --contains <commitID>  #本地分支
    git branch -r --contains <commitID>  #远程分支
    git branch -a --contains <commitID>  #本地和远程

### 通过代码内容搜索提交记录

    git log -S<code>
    git log -S<code> --oneline  #单行输出
    #<code>为要搜索的代码，如：git log -SOrderModel --oneline

### 通过comment关键词搜索提交记录

    git log --grep <comment>
    git log --grep <comment> --online  #单行输出
    #<comment>为关键词，如：git log --grep 订单列表优化 --oneline
    
### reset / revert / checkout的区别
https://segmentfault.com/a/1190000009126517
