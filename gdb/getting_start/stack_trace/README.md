### 学习在程序崩溃时执行栈跟踪

GDB调试器通过编号来引用栈帧, 其中当前栈帧的编号为0, main()函数的栈帧编号最高.
GDB的栈跟踪命令是`bt`, `backtrace`或`where`. 例如:

```
(gdb) backtrace
#0 <..> in factorial (n=-105582) at factorial.c:9
<lots of frames..>
#103581 <..> in factorial (n=-2) at factorial.c:9
#103582 <..> in factorial (n=-1) at factorial.c:9
#103583 <..> in main (argc=2, argv=0x761ce8) at factorial.c:20
```

#### 参考资料:
《软件调试实战》: 3.4章节
