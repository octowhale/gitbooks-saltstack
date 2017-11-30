# 配置

+ https://docs.saltstack.com/en/latest/ref/configuration/master.html
+ https://docs.saltstack.com/en/latest/ref/configuration/minion.html


## multi-master

> 关键点: 所有 master 的 key 都必须一致。

1. 将 primary master 主机 `/etc/salt/pki/master` 目录下所有的所有内容复制到 secondary master 对应目录下。
1. secondary master 重启 `salt-master`。
1. secondary master 执行 `salt-key -L` 查看是否需要重新允许 minion。

> http://www.cnblogs.com/renolei/p/4584406.html
