一个文件的文件名最大是255 最后留一个给/0
文件的读写指针只有一个
APUE
2进制的3位对应8进制的一位	16进制是4位
%d 十进制 %o 8进制 %0x16
计算机按原码存储的弊端 
	0有2种表示方式 
	对减法运算出错
	
补码求原码
	补码
	补码的反码
	反码+1

switch里面的判断条件只能是整数

数组在定义时只能是常量 在使用时可以是常量或者变量

fork函数调用一次返回两次 在父进程返回子进程的pid 在子进程返回0

数组的名字是常量是不能修改的

如果是数组两个元素地址相减 得到的不是步长 是下标的差值

如果数组做函数形参参数 会退化为指针 需要把数组的的个数也传进去

信号是内核发出的

SFC/SCANNOW
STRACE 追踪程序

struck是关键字 struck stu 合起来才是类型名
如果是指针 引用要用->

desc +表名 显示数据表的结构
where 筛选 
as 别名
is NULL / is not NULL 判断是否为空
distinct 过滤重复 作用于后面的所有内容

单例模式（饿汉式）
1.构造函数和拷贝构造函数私有
2.提供静态成员变量指向一个对象
3.私有化静态成员函数
4.提供外部获得对象的函数 静态成员函数

删除光标后面的字符：ctrl +h
删除光标前面的字符：ctrl +u（全部）
删除光标前面的字符：ctrl +k （全部）
 
bin目录下都是可执行程序（命令）
etc系统/用户安装的软件用到的配置文件
	查看用户：etc/passwd
	查看用户组：etc/group
lib 系统运行的时候运行的时候调用的一些基本动态库
media 自动挂载外设 挂载到该目录下
mnt 收到挂载目录时候挂载到这里（默认）
root 超级用户家目录
usr user software resource 
	当前用户安装的一些应用程序
	用到的一些库文件
dev device 存放设备文件
home linux操作系统所有用户的家目录
tmp 文件每次启动的时候都会清空
var 存放在线安装的临时文件

文件类型
 d 目录
 - 普通文件
 l 符号链接
 s 套接字
 p 管道
 b 块设备
 c 字符设备

文件如果是一个目录代表的是自己不露的文件大小 不包括里面文件的大小

创建嵌套目录 mkdir /home/chen/a/c -p 添加参数 p 参数i 给用户提示 参数 f 强制删除

sudo apt-get install 

ctrl + g 快速定位行号

查看 linux下默认的编码格式 cat/etc/sysconfig/i18n 

嵌套创建目录 -p
嵌套删除目录 -r
添加提示 （删除时） -i 
强制删除 -f 

创建软连接 
	ls -s 创建软连接的文件名 快捷方式的名字
		必须要使用绝对路径
		目录也可以创建快捷方式
硬链接 
	ln 创建硬链接的文件名 快捷方式的名字
	硬链接文件不占用磁盘空间
	
挂载u盘
		mount +设备名 + 挂载的目录
	设备名 sudo fdisk -l 
	挂载到非空目录是里面的目录内容会被临时覆盖
	显示中文 -o uocharset=utf-8
	卸载 sudo umonut 挂载的目录
	注意事项 一定要在挂载的目录外卸载 
	
压缩/解压缩
	tar 
		j - 压缩/解压缩使用bzip2格式
		z - 压缩/解压缩使用gzip格式
		c - 创建压缩文件
		x - 释放
		v -信息提示
		f -指定压缩包的名字
	压缩 
		tar 参数 压缩包名 原材料 zcvf --xxx.tar.gz /jcvf  --xxx.tar.bz2
	
	解压 
		tar 参数 压缩包名
		xxx.tar.gz ----zxvf
		xxx.tar.bz2 ---jxvf
	.zip 格式用unzip命令解压 unzip xxxxx.zip
		
kill -l 查看所有的kill 命令

top 任务管理器
nslook +域名 查看域名对应的ip

ftp 服务器
	服务器端 
		安装软件 vsftpd 
		创建并且设置匿名用户根目录
			修改匿名用户根目录中子目录的权限
				777
				修改目录所有者为ftp用户
		修改配置文件
		重启ftp服务 
	客户端
		使用vstftp客户端
		实名用户登陆
			ftp +服务器ip
			服务器用户名
			密码
			操作.....
		匿名用户登陆
			lftp+服务器ip
			login
			操作 ....
		退出登陆 
			exit bye quit 
			
nfs服务器
	 安装软件
		nfs-kernel-server
	 创建并设置共享目录
	 修改配置文件
	 重启服务器
	客户端
		挂载	
			sudo mount 服务器ip ： 共享目录/mnt
		取消挂载
			sudo umonnt/mnt

ssh 服务器
	 安装软件
	 远程登陆
		ssh服务器用户名@服务器ip
		服务器密码
	 退出登陆
		logout

		
vim 	
		移动光标
			上 k  
			下 j 
			左 h 
			右 l 
		移动光标到文章开头 gg
		移动光标到文章结尾 G
		移动光标到行首    0
		移动光标到行尾巴  $
		行跳转 12G
		复制 yy 
		粘贴 p
		vim下其实没有删除 只是剪切 
		可视模式 v 用来选中一句话中的一部分 
		查找 ？+要查找的  或者/ +要查找的
		替换 在字符上按r
		查找所有 在字符上按 #
		末行模式 在命令模式下输入 ：
		垂直分屏 vsp +文件的名称 
			在屏幕见切换 ctrl +w +w 
			vsp 对当前的文件分屏
			水平分屏 sp
		：！ +命令 （ls）暂时看一下 按其他键退出


which ls 查看ls命令存放在哪里 

alias 对命令进行一个重新的指定 

静态库 .c 
动态库 .so 

gcc -g 添加调试信息
	gdb 调试 
	run 运行到断点
	退出 quit 
	添加断点 b 15 b+行号 b+函数名
	断点之后在继续执行 直到下个断点  c
	往下执行一步 n 不会进入到函数体内部
	打印变量的值 p+变量名
	自动追踪变量的值 display +变量名 
	取消追踪 undisplay +断点的编号 
	查看断点信息 i 
	跳出当前的循环 finsh 
	获取变量的类型 type =变量名
	进入函数体的内部 step 
	设置变量值 set var +变量名 （i=20）
	删除断点 d+断点编号 
	
	查看其他文件 （具体到行）l+文件名 +行号 
	查看指定行 l+行号 l+函数名 查看函数行
	执行一行停止 start
	查看文件里的内容 l 
	
makefiel
	一个规则 两个函数 三个自动变量
	命名规则 makefile Makefile 只有这两种
		依赖：	app：main。capp：main。c add。c sub。c 如果头文件在同级目录里面可以不用写 因为会自动搜索
		命令：	 gcc main.c  add。c sub。c -o app 
		
	1。创建makefile vi makefile
		依赖：	app：main。capp：main。c add。c sub。c 如果头文件在同级目录里面可以不用写 因为会自动搜索
			命令：	 gcc main.c  add。c sub。c -o app 
	2.clean
		clean：
			rm main。o

explicit 禁止通过构造函数的隐式转换 声明为explicit的构造函数泵在隐式转换中使用

			
运算符重载		要重载的符号
	int   operator[](int index)
	返回类型 关键字	   参数 
		{
		return  this->xxxx;   重载操作 
		}	
	
纵向扩容 不是容量的扩容 而是保证数据的安全性
对外提供的最大容量取决与最小的storage 
横向扩容里面的每个group里面都是一个纵向扩容
	
	
ldd 命令 查看程序运行所需的动态库

添加动态库的方法
	1 export LD_LIBRARY_PATH=/usr/lib64/（so所在路径）
		只对当前用户的终端生效， 其他用户没用。
	2. sudo vim /etc/ld.so.conf
	   将/uer/lib64 加进来
		sudo ldconfig -v 更新 动态库配置文件。
	3、无论什么动态库，Linux操作系统， /usr/lib/
		cp /usr/lib64/ libcommom.so  --> /usr/lib (X)
		/usr/lib/libcommon.so  ------> /usr/lib64/libcommon.so
		
查看端口是否呗占用 
	netstat - ano 
	netstat - ano |grep 80  查看80端口是否被占用


关闭linux下防火墙	
		service iptables stop



防止头文件重复
	1.#ifndef XXXXX_H随便定义一个名字 但是最好和类名或者项目名一样
	#define XXXXX 
	。。。。。。
	。。。。。。
	#endif
	2. #pragma once
	

class<派生类名>:<继承方式><基类名>
{
	<派生类新定义成员>
};
继承	
	公有继承(public)
		公有继承的特点是基类的公有成员和保护成员作为派生类的成员时，它们都保持原有的状态，而基类的私有成员仍然是私有的，不能被这个派生类的子类所访问。
	私有继承(private)
		私有继承的特点是基类的公有成员和保护成员都作为派生类的私有成员，并且不能被这个派生类的子类所访问。
	保护继承(protected)
		保护继承的特点是基类的所有公有成员和保护成员都成为派生类的保护成员，并且只能被它的派生类成员函数或友元访问，基类的私有成员仍然是私有的。
构造函数和析构函数不能够被继承


yum


多态
	父类指针指向子类对象 
	
	
虚函数
	vitual 关键字使其在编译的时候不确定 在执行的时候才确定

	
数组和指针的区别	
	数组名是一个常量指针 不能加加

指针指向类成员变量的指针
	<数据类型><类名>::*<指针名>
	int A ::*pPram;
	
指针指向类成员函数
	<返回类型>(<类名>::*<指针名>) =&<类名>::<非静态数据函数>
	void (A::pFunc)(int,int)=&A::func;

只对当前函数的下一个函数有效
泛型编程(函数模板)//不允许类型自动转换
	//template<typename T> 里面是class和typelate是一样的
	template<class T>
	void MySwap(T& a,T& b)
	{
	T temp =a;
	a=b;
	b=temp;
	}
	调用 1.显示指定MySwap<int>(a,b)
		2.自动推导 MySwap(a,b) 
		
异常处理
	throw x 
	try
	{
	可能出错的语句
	}
	catch (x的数据类型 （int e）)
	{
	如果try出错指向这里的代码 如果try没有出错 跳过这里继续执行
	}
	catch (...)//
	{
	其他异常
	}
	
栈解旋
	异常被抛出后，从进入try开始到异常被抛掷前，这期间在栈上的多有对象，都会被自动析构。析构的顺序与构造的顺序相反，这一过程被成为栈的解旋
	
进入公司可以先看概要文档 

STL标准模板库
	stl6大组件
		容器	算法	迭代器	仿函数 适配器 空间适配器
		              迭代器名称
	容器             ---------
		vector<int>::iterator begin =v.begin();//vector首先就是一个容器 和string一样
		 ----------  ------   ------
		 仿照模板int是类型	  类似与变量名称
					迭代器
		 迭代器首地址指向容器第一个元素的地址 end指向最后一个元素的下一个地址
		 
		 
string容器
	用哪个容器就导入那个容器的头文件 #include “string”
	然后和函数类似 都要初始化 初始化和赋值之后可以正常的做各种操作了就 
	初始化和函数一样 也有
	
vector容器
	相当于一个单向开口的数组
	可以动态的分配空间 
	
depue容器
	是一个双向开口的连续性存储空间
		 
stack容器
	stack容器没有迭代器 必须要先进后出
	
queue容器
	没有迭代器 先进先出
	
	
set容器
	可读不可写 因为底层是用的二叉树 修改一个数值 可能会改变整个树的规则
	set的iterator是一种const_iterator
	
	
find命令
	 find ~ -name "*.txt" -print 在根目录下查找格式为.txt的文件
	 
	 
git操作
	1 在github上 创建一个git仓库
	2 回到本地， 初始化当前 git环境（此步骤只需要一次）
		git init	（会在当前出现一个.git隐藏文件 ）
	3 将本地路径 跟远程的git路径 相关联（此步骤只需要一次）
		git remote add origin https://github.com/aceld/0706_test.git
	4 配置git的用户名和密码（此步骤只需要一次）
		$ git config --global user.name "wirelessqa"
		$ git config --global user.email wirelessqa.me@gmail.com
	5 如果是红帽 git 低版本
		修改.git/config
		https://username@giturl 加上用户名@
		需要在终端执行unset SSH_ASKPASS
