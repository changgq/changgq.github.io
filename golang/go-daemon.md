# GO-DAEMON - 怎么样为Go程序创建守护进程？

最近在编写开发Go程序，编写启动脚本时，遇到一个问题：怎么样为Go程序创建守护进程？

1. nohup

```
nohup ./myApp &
```

2. supervise
3. Cgo deamon函数
4. go通过syscall调用fork实现(这个和第3条原理一样)
5. [go-daemon](https://github.com/fiorix/go-daemon) 

