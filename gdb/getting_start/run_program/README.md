### 使调试器与程序一切运行

对于GNU编译器GCC和大部分其他编译器, 进行调试的编译器标志是`-g`. 
用GCC编译factorial程序的方法如下:

```
> gcc -g -o factorial factorial.c
```

对于GDB调试器, 需要健入命令gdb, 并输入程序名称作为它的第一个参数.
运行程序的命令是run, 后跟要传递给程序的命令行参数. 例如:

```
> gdb factorial
<lots of copyright stuff..>
(gdb) run 1
<messages about Loaded symbols..>
factorial 1 = 1
Program exited normally
```


#### 参考资料:
《软件调试实战》: 3.3章节
