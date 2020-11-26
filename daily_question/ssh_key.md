一、打开 vim（terminal.app）查看本地是否存在 SSH-Key

# ls -al ~/.ssh

> > 如果 vim 输出的是如下内容：证明本地没有生成的 SSH Key，请执行第二步。

# No such file or directory

> > 如果 vim 输出的是如下内容： 证明本地已经存在 SSH Key 文件，请执行第四步。

# id_rsa id_rsa.pub

二、如果没有，生成新的 SSH Key

#ssh-keygen -t rsa -C"you_email"

your_email：这里填写你在 GitLab 或者 GitHub 注册时的邮箱。

后面的提示直接敲回车，一路完成。

三、生成并添加 SSH Key

# ssh-add ~/.ssh/id_rsa

四、查看 SSH Key

# cat /Users/xiedawen/.ssh/id_rsa.pub

xiedawen 是你的电脑用户名，例如：howieMacBook-Pro:~ howie\$中的 howie 关键字。

复制生成好的 SSH Key 添加到 GitLab 或者 GitHub 中的 SSH Key 中即可。
