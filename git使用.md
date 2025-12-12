## ## 初始化

> 切换到 git 仓库目录,点击 `Git Bash Here`
>
> `git -h` 查看命令帮助
>
> `git [command] -h` 查看具体命令的帮助
>
> git绑定GitHub 
>
> ```shell
> # 1. 检查安装ssh
> ssh
> # 2. 生成密钥和公钥 -t 表示使用密钥类型 RSA、dss、ed25519
> # 				 -C 表示使用注释或者名称标识
> ssh-keygen -t rsa
> # 密钥生成位置 (Linux)~/.ssh	(MacOS)~/.ssh	(windows)C:\Users\username\.ssh\id_rsa
> # 3. 将生成公钥 id_rsa.pub 内容粘贴到 GitHub->Settings->SSH and GPG keys->SSH key
> # 4. 验证绑定是否成功
> ssh -T git@github.com
> # 出现 You've successfully authenticated. 表示成功
> ```
>
> **基本流程**
>
> pull 拉取远程仓库的更新 -> 本地修改 -> 使用add/commit提交仓库 -> push 到远程仓库
>
> 

## 常用命令

> **⭐查看当前仓库状态** `git status`
>
> **初始化 git 仓库** `git init`
>
> **添加目录下的文件** `git add <file>` 
>
> - 此命令并没有直接将文件提交到 git 仓库，而是存储到临时缓冲区，还需要 commit 才能将文件提交到 git 仓库中
>
> **⭐提交**  `git commit [options]` 
>
> - `-m "<text>"` 表示提交信息<text>
>
> **打印提交日志** `git log`
>
> **查看分支** `git branch`
>
> **切换到分支** `git checkout <branch_name>`
>
> ​	**切换到分支中的标签** `git checkout <tag_name>`
>
> **合并分支(到当前分支)** `git merge <branch_name>`
>
> **删除分支** `git branch -d <branch_name>` **强制删除** `git branch -D <branch_name>  `
>
> **为当前分支添加标签** `git tag <tag_name>` 
>
> **⭐⭐本地推送到远程 push** `git push origin master`
>
> **⭐⭐拉取远程同步 pull** `git pull origin master`
>
> **克隆仓库** `git clone <repository_URL>`

## 常见提示



