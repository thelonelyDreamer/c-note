### 1. 元数据

- 官网:**http://gcc.gnu.org/**



### 2. 编译指令

#### 2.1 编译周期

##### 2.1.1 单文件

```bash
#1 预处理
 gcc -E hello.c -o hello.i
#2 编译
gcc -S hello.i -o hello.s
#3 汇编
gcc -c hello.s -o hello.o
#4 链接
gcc hello.o -o hello
#5 运行
./hello
```

##### 2.1.2 多文件

#### 2.2 其他配置

```bash
#指定源代码字符编码(若不指定，默认为utf-8)
-finput-charset UTF-8 

```

