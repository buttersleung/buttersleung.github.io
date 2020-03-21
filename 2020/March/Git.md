# Git

## Git 初始化及仓库创建和操作

### 基本信息设置

- 设置用户名：`git config --global user.name 'buttersleung'`
- 设置用户名邮箱：`git config --global user.email 'buttersleung@gmail.com'`
- ls: 文件目录   pwd: 工作目录  clear: 清除界面

### 初始化一个新的git仓库

1. 创建文件夹`mkdir folder_name`
2. 在文件内初始化git（创建git仓库）`cd floder_name` >>>`git init`

### 向仓库添加文件

1. 创建文件`touch demo.py`
2. 将文件添加到暂存区`git add demo.py`
3. 将文件提交到仓库`git commit -m 'add demo.py'`

### 修改仓库文件

1. 修改文件
2. `git add demo.py`
3. `git commit -m 'modified'`

### 删除仓库文件

1. `rm demo.py`
2. 从暂存区删除`git rm demo.py`
3. `git commit -m 'remove demo.py'`

## Git 管理远程仓库

- 复制远程仓库 `git clone 仓库地址`

- 将本地仓库同步到git远程仓库中`git push`

出现错误`The requested URL returned error:403 Forbidden while accessing`，解决方式：
`vi .git/config`
`将[remote 'origin']  url=https://github.com/username/reponame.git`
`修改为url=httpss://username:passward@github.com/username/remoname.git`

