git pull：拉取git上最新的代码；
　　编辑代码，准备提交时，git stash：将自己编辑的代码暂存起来，防止git pull时与库中的代码起冲突，否则自己的代码就白敲了；
　　然后，git pull：拉取一下代码，与库中代码，做到同步，有冲突则解决冲突，如果省了这一步，别人有提交的代码，没有更新，自己提交就会报错，再走这一步，就会把别人的代码拉取出来，然后一起提交，就相当于你提交了自己的代码，也提交了别人的代码；还有，有时这样会使库中代码乱掉，别人的心血也会丢失，你就是罪魁祸首了；
　　然后，git stash apply:将暂存在缓存区的代码下载到本地，如果和git上的代码有冲突就要解决冲突（这种冲突是在本地解决，保障git仓储的代码稳定）；
　　然后，git status：查看文件状态，红色表示未提交已修改的文件，绿色为提交过已修改的文件，可以省略，初期用建议查看提交前后对比；
　　然后，git add：添加提交的文件，可以全部添加git add . 也可以单个或多个添加，git add 后面跟文件名称，不知道名称可以参考git status罗列出来的修改文件；
　　然后，git commit -m "提交文件的修改说明" 养成好的习惯，把说明写清楚，方便检查与版本恢复；
　　然后，git status ：查看文件是否提交，特别适合单个文件提交，查看遗漏提交的文件，可以省略；
　　最后，git push ：推送代码到git库中；
