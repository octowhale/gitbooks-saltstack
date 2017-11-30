# No Top file or master_tops data matches found

```
base:
  '*'   # <- 这里少了一个冒号
    - init.dns
    - init.audit
    - init.history
```

抄漏一个 冒号， 但是 salt 的报错不是语法错误。因此需要多注意标点符号。

> [top.sls 参考文档](https://docs.saltstack.com/en/latest/ref/states/top.html#a-basic-example)