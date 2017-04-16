## git 命令使用

 检出仓库两种方式：

* 创建本地仓库的克隆版本 ：<pre>git clone /path/to/repository</pre>
* 克隆远端服务器： <pre>git clone （具体远程仓库的地址,浏览器URL）</pre>

添加和提交：

* 将新增的文件添加到缓存区(和svn一样) <pre>git add <filename> /  git add * </pre>
* 提交代码到head <pre>git commit -m "描述信息"，团队开发中，还是有必要写下改了什么东东的</pre>

推送：

* 将本地代码提交到远端仓库 <pre>git push origin master</pre>

分支：

* 创建分支 <pre>git checkout -b [branchName]</pre> 
* 切换主分支 <pre>git checkout master</pre>
* 删除分支 <pre>git branch -d [branchName]</pre>

更新&合并

* 从远程仓库拉下代码到本地仓库，即更新 <pre>git pull</pre>
* 对比差异  <pre>git diff [source_branch] [target_brach] </pre>
* 合并 <pre>git merge [target_brach]</pre>

替换本地改动
* 一不小心改坏了别人的代码又半天没察觉到改了哪块，还原下 <pre>git checkout --[flieName]</pre>
* 强推 获取最新版本，强行指定本地主分支 <pre>git fetch origin ; git reset --hard origin/master</pre>