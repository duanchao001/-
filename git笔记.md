## 想要让git对一个目录进行版本控制需要以下步骤：

- 进入要管理的文件夹

- 执行初始化命令

  ```
  git init
  ```

- 管理目录下的文件状态

  ```
  git status
  
  注：新增的文件和修改过后的文件都是红色
  ```

- 管理指定文件（红变绿）

  ```
  git add 文件名
  git add .
  ```

- 个人信息配置：用户名、邮箱 【一次即可】

  ```
    git config --global user.email "you@example.com"
    git config --global user.name "Your Name"
  ```

- 生成版本

  ```
  git commit -m '描述信息'
  ```

- 查看版本记录

  ```
  git log 
  ```

## 拓展新功能

```
git add 
git commit -m '短视频'
```

## 回滚至之前版本

```git log 
git log
git reset --hard 版本号
```

## 回滚之之后版本

```git reflog 
git reflog
git reset --hard 版本号
```

## 修复bug方案

- 查看分支

  ````
  git branch
  ````

- 创建分支

  ```
  git branch 分支名称
  ```

- 切换分支

  ```
  git checkout 分支名称
  ```

- 分支合并（可能产生冲突）

  ```
  git merge 要合并的分支
  
  注意：切换分支再合并
  ```

- 删除分支

  ```
  git branch -d 分支名称
  ```

## 第一次上传代码

```1. 给远程仓库起别名
1. 给远程仓库起别名	
	git remote add origin 远程仓库地址
2. 向远程推送代码
	git push -u origin 分支
```

## 第一次下载代码

```1. 切换到dev分支进行开发
1. 切换到dev分支进行开发	
	git checkout dev 
2. 把master分支合并到dev [仅一次]
	git merge master
3. 修改代码
4. 提交代码
	git add . 
	git commit -m 'xx'
	git push origin dev 
```

## 非第一次上传代码

```te
1. 切换到dev分支进行开发
	git checkout dev 
2. 拉代码
	git pull origin dev 
3. 继续开发

4. 提交代码
	git add . 
	git commit -m 'xx'
	git push origin dev 
```

## 非第一次下载代码

```tex
1. 切换到dev分支进行开发
	git checkout dev 
2. 拉最新代码(不必再clone，只需要通过pull获取最新代码即可)
	git pull origin dev 
3. 继续开发

4. 提交代码
	git add . 
	git commit -m 'xx'
	git push origin dev 
```

