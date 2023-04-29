### 1. 按字典排序

```c
char* arr[3] ={"ax","AX","a"}

void sort(char** strs,int n);
```

```c
/**
 * @todo 比较两个C风格的字符串
 * @param a 是第一个字符串的地址
 * @param b 是第二个字符串的地址
 * @return if a>b 返回值大于0; if a=b ,返回值小于0； if a<b 返回值小于0
 */
int compare(char* a,char* b){
	int i=0;
	while(a[i]!='\0'||b[i]!='\0'){
		int temp = a[i] -b[i];
		if(0!=temp) return temp;
		i++;
	}
	if(a[i]='\0'&&b[i]='\0') return 0;
	if(a[i]='\0') return 1;
	if(b[i]="\0") return -1;
	return 0;
}

// 测试用例

```

```

```

