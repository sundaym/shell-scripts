# shell-scripts
Linux shell scripts

## TTY
1. TTY中多条命令一起执行
```shell
# &&前面的执行成功才执行后面的语句
git add . && git commit -m "xxxx" && git push
# ; 不管命令执行是否成功都往下执行
rm ./foo/bar; mv ./foo ./fooo; ls ./fooo
```
2. 修改bash配置

一般用户的配置文件在/home/[username]/.bashrc

对所有用户生效的配置文件在 /etc/.bashrc

root用户的配置文件在/root/.bashrc
3. 给命令取别名

alias 显示别名，unalias ll删除别名

在TTY中使用alias只对当前session有效，若要每次打开TTY别名都生效，需要在.bashrc文件中进行配置
```shell
alias ll='ls -alF'
```


