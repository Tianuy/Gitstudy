### 三种状态
已提交（committed）、已修改（modified） 和 已暂存（staged）
* 已修改表示修改了文件，但还没保存到数据库中。
* 已暂存表示对一个已修改文件的当前版本做了标记，使之包含在下次提交的快照中。
* 已提交表示数据已经安全地保存在本地数据库中。

Git项目拥有三个阶段：工作区， 暂存区， Git目录
Working Directory->git add->Staging Area-> git commit ->.git directory ->Working Directory

如果 Git 目录中保存着特定版本的文件，就属于已提交状态。 如果文件已修改并放入暂存区，就属于已暂存状态。 如果自上次检出后，作了修改但还没有放到暂存区域，就是已修改状态

gitconfig 文件：包含系统上每一个用户及他们仓库的通用配置，在执行git config 时带上--system选项时，就会读写该文件中的配置变量。 

.gitconfig 文件: 只针对当前用户。 传递 --global 选项让git读写此文件,这会对你系统上的所有仓库生效。
--local > --global > --system优先级从大到小.gitconfig 会覆盖gitconfig中的配置变量

查看所有配置以及它们所在的文件用命令 <br>
`git config --list --show-origin`
#### 用户信息 
安装完Git之后，第一件是配置好自己的用户名和邮件地址，否则git不知道你是谁，没法执行提交(commit)

配置整个系统的用--global选项，只作用当前仓库用--local选项也可以不带任何选项，命令如下：
`git config --global user.name "Tianuy"`<br>
`git config --global user.email "Tianuy-git@outlook.com"`

如果使用了--global选项，那么该命令只需要运行一次，以后你在该系统上做任何事，都会使用这些信息，如果要针对特定的项目使用不同的用户名和邮件地址时，可以运行不带--global选项的命令来配置。

