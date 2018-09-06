Docker Run "uname --all" Demo
=============================

```
docker build -t docker-run-uname-all-demo .
docker run docker-run-uname-all-demo
```

将会输出：

```
Linux 11ec3bc810d0 4.4.0-128-generic #154-Ubuntu SMP Fri May 25 14:15:18 UTC 2018 x86_64 GNU/Linux
```

注意点
---

1. `uname`：也可以写完整路径`/bin/uname`
2. `["uname", "--all"]`：这种数组形式是推荐的形式。如果写成`"uname --all"`，会报错，会把后面的`--all`当作一个单独的命令。