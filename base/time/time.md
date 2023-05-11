### 1.  获取当前时间

#### 1.1 获取秒数

```c
time_t current_time =time(NULL);//获取秒数
struct tm* tm=localTime(&cuurent_time);
tm->tm_year+1970; // 年
tm->tm_mon+1;//月
tm->tm_mday;//日
tm->tm_hour;//时
tm->tm_min;//分
tm->tm_sec;//秒
tm->tm-wday//星期几
```

#### 1.2 获取毫秒数

暂未找到相关api ,可以通过操作系统api获取

##### 1.2.1 window

```c
#include<windows.h>
GetTickCount()//获取操作系统启动后的毫秒数
//获取格林威治时间
SYSTEMTIME currentTime;
GetSystemTime(&currentTime);
```

