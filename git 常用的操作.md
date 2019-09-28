常用操作:

1、首次提交一个项目
```
git init
git add WanAndroidClient-master/
git commit -m "首次提交"
git remote add origin git@github.com:shenshizhong/WanAndroidClientssz.git
git push -u origin master
```
2、克隆一个远程项目
```
git clone git@github.com:shenshizhong/git.git
```
3、查看所有本地分支和远程分支
```
git branch -a      
```
4、检出一个分支
```
git checkout -b dev remotes/origin/dev    创建一个本地分支
```
5、上传分支
```
git push origin  feature/mipush_optimize

git push -u origin  feature/mipush_optimize（比较全面的上传）

```
6、删除一个分支
```
git branch -d  dev  

git branch -D  dev  （强制删除）  
```
7、版本的备份
```
1、git tag   检查历史tag
2、git checkout -b branch_name v1.4     检出tag代码
3、git tag -a v1.4  -m 'my version 1.4' 
4、git push origin v1.4                 上传tag
```
8、回滚：
```
commit 047d6f3e4ecd4cedce086d23f433e34cd5744440 (origin/my_develop) //要回滚的位置
 git reset --hard 047d6f3e4ecd4cedce086d23f433e34cd5744440
```
9、临时缓存：
```
缓存：git stash 
取出：git stash pop
查看：git stash list 
```


