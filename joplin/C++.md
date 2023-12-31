# 基础语法

### 基础语法框架
```c++
#include (iostream)
using namespace std;

int main(){
	system("pause");
	
	return 0;
}
```
***
#### 1.2注释
单行注释:`//描述信息`
多行注释(整体说明):`/*描述信息*/`

#### 1.3变量
语法:数据类型 变量名=初始值(可不赋初始值);

#### 1.4常量
1. #define 宏常量: `define 常量名 常量值`
==通常在文件上方定义==
2. const修饰变量: `const 数据类型 常量名=常量值`
===通常在变量定义前加关键词const==

#### 1.5关键词

#### 1.6 标识符命名规则
1. 非关键词
2. 仅限字母,数字,下划线
3. 字母区分大小写
***
### 2.数据类型
#### 2.1整型
>1字节(Byte)=8bit

|数据类型|占用空间\字节|
|:---|:---|
|int(整型)(大约三万)|4|
|short(短整型)|2|
|long(长整型)|4|
|long long(长长整型)|8|
#### sizeof关键字
作用:统计数据类型所占内存大小
语法:`sizeof(数据类型/变量)`
eg.`sizeof(short);//short类型所占空间内存`
整型大小比较:short< int<= long<= long long

#### 2.3实型(浮点型)
作用:表示小数
1. 单精度float(**4**字节|**7**位有效数字)
3. 双精度double(**8**字节 **15~16**位有效数字)

`float f1=3.14f;//系统默认数字3.14为双精度,此赋值过程要进行一次类型转换,加后缀f可直接将初始值定义为float`
补充说明:目前无外加配置情况下float 与double显示小数均为六位有效数字

科学计数法:
eg.
1. 3e2 =$3*10^2$
2. 3e2=$3*0.1^2$
   

#### 2.4字符型
作用:显示单个字符
语法:`char ch='a'`
>用单引号将字符括出
>单引号内仅能有一个字符

占用内存:==一个字节==
存储方式:ASCII编码形式存入`(int)字符变量名`即可得到该字符变量中所存字符的ASCII码值(a--97;A--65)

#### 2.5转义字符
作用:表示一些不能显示出来的ASCII字符
1. \n:换行
2. \\:表示一个反斜杠字符"\"
3. \t:水平制表(左对齐 八位) `aaa\thelloworld`输出:aaa(五个空位)helloworld
4. \":代表一个双引号字符

#### 字符串型
语法:`string 变量名="字符串值"`
注意:包含一个头文件 #include < string >


#### 2.7布尔类型
作用:代表真或假的值
bool类型只有两个值:
- true--真(本质是1)
- false--假(本质是0)
占用空间:==一个字节==
语法:`bool flag=true;`

#### 2.8数据的输入
作用:从键盘获取数据
语法:`cin>>变量`

### 3.运算符
***
### 4.程序流程结构
 
 
大致与C语言类似

### 5.数组
